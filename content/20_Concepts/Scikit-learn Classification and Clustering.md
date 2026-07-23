---
unit: FIT1043
parent: "[[Predictive Models]]"
tags: [DataScience/Tools, ML/Classification, Python/Sklearn, Monash/CS_DS]
type: pattern
aliases: [sklearn, scikit-learn, DecisionTreeClassifier, RandomForestClassifier, KMeans, train_test_split]
---
# [[Scikit-learn Classification and Clustering]]

**Context:** [[FIT1043_MOC]] · the applied form of [[Decision Trees and Regression Trees|trees]] / [[Random Forest|forests]] / [[k-means Clustering|k-means]] · one common fit/predict API · labs: `30_Projects/FIT1043_Labs/Week7-Classification-sklearn.ipynb`, `Week7-Clustering-KMeans.ipynb`
**Task signature:** train a classifier on labelled data and evaluate it, or cluster unlabelled data with k-means.

> [!abstract] Quick Revision
> - **🎯 Trigger:** build a model in Python ➔ pick an estimator, then fit(X, y) (supervised) or fit(X) (unsupervised), then predict.
> - **⚡ Critical Bottleneck:** every sklearn estimator shares the **fit → predict** API; supervised needs a train/test **split**, and only **fit the scaler on train** (`fit_transform` train, `transform` test).

## 🔧 Minimal Working Example
```python
import pandas as pd
from sklearn.model_selection import train_test_split
from sklearn.preprocessing import StandardScaler
from sklearn.tree import DecisionTreeClassifier
from sklearn.metrics import confusion_matrix

dataset = pd.read_csv('TravelInfo.csv')
X = dataset.iloc[:, [0, 1]].values      # features (Age, Income)
y = dataset.iloc[:, 2].values           # label (Travelled?)

X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.25, random_state=0)
sc = StandardScaler()
X_train = sc.fit_transform(X_train)     # fit on TRAIN
X_test  = sc.transform(X_test)          # only transform TEST

clf = DecisionTreeClassifier(criterion='entropy', random_state=0).fit(X_train, y_train)
y_pred = clf.predict(X_test)
confusion_matrix(y_test, y_pred)        # evaluate on held-out test
```
**Expected output:** a fitted tree; predictions for the test set; a 2×2 [[Classification Evaluation (Confusion Matrix and Metrics)|confusion matrix]].

- **Feature/label split** ➔ `X = df.iloc[:, [cols]].values`, `y = df.iloc[:, col].values`.
- **Train/test split** ➔ `train_test_split(X, y, test_size=0.25, random_state=0)` — `random_state` makes it reproducible.
- **Scale** ➔ `StandardScaler()`; `fit_transform(X_train)` then `transform(X_test)` — never fit on test.
- **Fit/predict** ➔ `clf.fit(X_train, y_train)` → `clf.predict(X_test)`.

## 🔀 Variations
- **Random forest** ➔ `from sklearn.ensemble import RandomForestClassifier; RandomForestClassifier(n_estimators=20, criterion='entropy', random_state=0).fit(X_train, y_train)` — `n_estimators` = number of [[Random Forest|trees]].
- **k-means (unsupervised)** ➔ no labels:
```python
from sklearn.cluster import KMeans
km = KMeans(n_clusters=2).fit(df[['Distance_Feature','Speeding_Feature']])
km.cluster_centers_      # the k centroids
km.labels_               # cluster id per point
plt.scatter(df['Distance_Feature'], df['Speeding_Feature'], c=km.labels_)
```

## 🥋 Kata 
> [!QUESTION]- Kata 1: Cluster drivers into 4 groups on two features, then colour the scatter by cluster and mark the centroids.
> > [!SUCCESS]- Reference solution
> > ```python
> > km = KMeans(n_clusters=4, init='random').fit(df[['Distance_Feature','Speeding_Feature']])
> > plt.scatter(df['Distance_Feature'], df['Speeding_Feature'], c=km.labels_)
> > plt.plot(km.cluster_centers_[:,0], km.cluster_centers_[:,1], 'k*', markersize=20)
> > plt.show()
> > ```
> > - **Key move:** `KMeans(n_clusters=k).fit(X)`; `.labels_` colours points, `.cluster_centers_` gives the centroids.

## ⚠️ Pitfalls
- 💡 **Never fit the scaler on test data** ➔ `fit_transform` the train set, `transform` (only) the test set — otherwise test info leaks into training.
- 💡 **k must be chosen for k-means** ➔ `n_clusters=k` is set in advance; `init='random'` seeds are volatile (see [[k-means Clustering]]).
- 💡 **Set `random_state`** ➔ without it, splits/forests differ every run, making results irreproducible.
