---
unit: FIT1043
type: MOC
tags:
  - Monash/CS_DS
  - 2025/S2
---
# 📘 FIT1043: Introduction to Data Science

> [!INFO] Map of Content
> Index for **FIT1043 Introduction to Data Science**. Each link below is a standalone atomic note. Start with [[Data Science]] and follow the links. Week 1 is conceptual — *what* data science is, the process, and how it relates to neighbouring disciplines.

## 📊 Assessment Map

- **Written Assignment (40%)** ➔ applied wrangling/analysis — the 🧰 cheatsheets + 🧪 pattern notes are the working surface.
- **Test (10%)** + **Examination (50%)** ➔ concept-explainable material: lifecycle, models, Big Data, ethics (Weeks 1–11 LOs below).

## 🧰 Toolkit Cheatsheets (pinned — pre-lab / pre-exam single re-reads)
- 📌 [[FIT1043 Unit Cheatsheet]] — whole-unit exam crib — the CONCEPT half; pairs with the code toolkits below
- [[Pandas Toolkit (Cheatsheet)]] -> integrates Weeks 3–4: audit → clean → groupby/agg → plot
- [[Sklearn Workflow (Cheatsheet)]] -> integrates Weeks 6–7: one estimator skeleton + metrics
- [[R Toolkit (Cheatsheet)]] -> integrates Week 8: syntax → data frames → plots → lm
- [[Shell Toolkit (Cheatsheet)]] -> integrates Weeks 9–10: navigate → inspect → grep/sort/cut/awk → pipes → shell→R handoff

## 📅 Knowledge Index

### Week 1 — Data Science & the Data Science Process
- [[Data Science]] -> Parent Framework: [[Data Science Process (Standard Value Chain)]]
- [[Machine Learning]] -> Parent Framework: [[Data Science]]
- [[Data Science Process (Standard Value Chain)]] -> Parent Framework: [[Data Science]]
- [[Data Science vs Related Disciplines]] -> Parent Framework: [[Data Science]]

### Week 2 — Roles & Skills, Impact, Business Models, Python
- [[Data Scientist Roles and Skills]] -> Parent Framework: [[Data Science vs Related Disciplines]]
- [[Impact of Data Science]] -> Parent Framework: [[Data Science]]
- [[Data Business Models]] -> Parent Framework: [[Data Science]]
- [[Python for Data Science]] -> Parent Framework: [[Data Science]]

### Week 3 — Data Sources & Data Wrangling
- [[Data Sources and Open Data]] -> Parent Framework: [[Data Science Process (Standard Value Chain)]]
- [[APIs for Data Collection]] -> Parent Framework: [[Data Sources and Open Data]]
- [[Data Wrangling]] -> Parent Framework: [[Data Science Process (Standard Value Chain)]]
- [[Data Quality Problems]] -> Parent Framework: [[Data Wrangling]]
- [[Data Auditing in Pandas]] -> Parent Framework: [[Data Wrangling]]

### Week 4 — Visualisation, Descriptive Statistics & Aggregation
- [[Types of Data (Numeric and Categorical)]] -> Parent Framework: [[Data Science Process (Standard Value Chain)]]
- [[Data Visualisation (Chart Types)]] -> Parent Framework: [[Types of Data (Numeric and Categorical)]]
- [[Measures of Centrality]] -> Parent Framework: [[Types of Data (Numeric and Categorical)]]
- [[Measures of Spread and Boxplots]] -> Parent Framework: [[Measures of Centrality]]
- [[Association Between Variables]] -> Parent Framework: [[Measures of Centrality]]
- [[Groupby-Aggregate Pipeline (Pandas)]] -> Parent Framework: [[Python for Data Science]]
- [[Plotting with Matplotlib (Pandas)]] -> Parent Framework: [[Data Visualisation (Chart Types)]]

### Week 5 — Models & Machine Learning
- [[Predictive Models]] -> Parent Framework: [[Data Science Process (Standard Value Chain)]]
- [[Machine Learning Styles (Supervised vs Unsupervised)]] -> Parent Framework: [[Machine Learning]]
- [[Learning Theory and Loss Functions]] -> Parent Framework: [[Machine Learning]]
- [[Linear and Polynomial Regression]] -> Parent Framework: [[Machine Learning Styles (Supervised vs Unsupervised)]]
- [[Machine Learning]] -> Parent Framework: [[Data Science]] *(extended in Week 5: development workflow, Wikipedia/Emerj definitions)*

### Week 6 — Regression Analysis (Fitting, Bias–Variance, Ensembles)
- [[Linear and Polynomial Regression]] -> Parent Framework: [[Machine Learning Styles (Supervised vs Unsupervised)]] *(extended in Week 6: terminology, MSE, when-to-use)*
- [[Bias-Variance Tradeoff (Underfitting vs Overfitting)]] -> Parent Framework: [[Linear and Polynomial Regression]]
- [[No Free Lunch Theorem]] -> Parent Framework: [[Machine Learning]]
- [[Ensemble Models]] -> Parent Framework: [[Machine Learning]]

### Week 7 — Classification & Clustering
- [[Classification Evaluation (Confusion Matrix and Metrics)]] -> Parent Framework: [[Predictive Models]]
- [[Decision Trees and Regression Trees]] -> Parent Framework: [[Predictive Models]]
- [[Random Forest]] -> Parent Framework: [[Ensemble Models]]
- [[k-means Clustering]] -> Parent Framework: [[Machine Learning Styles (Supervised vs Unsupervised)]]

### Week 8 — Introduction to R
- [[R for Data Science]] -> Parent Framework: [[Data Science]]
- [[R Basics (Syntax, Types, Control Flow)]] -> Parent Framework: [[R for Data Science]]
- [[R Vectors]] -> Parent Framework: [[R Basics (Syntax, Types, Control Flow)]]
- [[R Data Frames and IO]] -> Parent Framework: [[R Vectors]]
- [[R Visualisation (base graphics)]] -> Parent Framework: [[R for Data Science]]
- [[R Modelling (lm and Decision Trees)]] -> Parent Framework: [[R for Data Science]]

### Week 9 — Characterising & Big Data + Unix Shell
- [[Big Data and the Vs]] -> Parent Framework: [[Relational Model]] *(shared with FIT2094; extended with Laney's V-taxonomy)*
- [[Metadata]] -> Parent Framework: [[Data Sources and Open Data]]
- [[Growth Laws (Moore, Koomey, Bell, Zimmerman)]] -> Parent Framework: [[Big Data and the Vs]]
- [[Unix Shell for Data Science]] -> Parent Framework: [[Data Wrangling]]

### Week 10 — Databases & Big Data Processing
- [[SQL vs NoSQL Databases]] -> Parent Framework: [[Big Data and the Vs]]
- [[Distributed Processing and Map-Reduce]] -> Parent Framework: [[Big Data and the Vs]]
- [[Hadoop and Spark]] -> Parent Framework: [[Distributed Processing and Map-Reduce]]

### Week 11 — Data Management & Data Governance
- [[Data Management and Data Governance]] -> Parent Framework: [[Data Science Process (Standard Value Chain)]]
- [[Privacy, Confidentiality, and Security]] -> Parent Framework: [[Data Management and Data Governance]]
- [[Data Compliance and Regulations (PDPA, GDPR)]] -> Parent Framework: [[Data Management and Data Governance]]

### 🧪 Applied / Lab Pattern Notes (code)
*(Lab notebooks & solutions live in `30_Projects/FIT1043_Labs/`; these notes store the reusable patterns.)*
- [[Python Basics (Syntax, Types, Control Flow)]] -> Parent Framework: [[Python for Data Science]] *(Week 1)*
- [[Pandas DataFrame Basics]] -> Parent Framework: [[Python for Data Science]] *(Weeks 2 & 4)*
- [[Groupby-Aggregate Pipeline (Pandas)]] -> Parent Framework: [[Python for Data Science]] *(Week 3; multi-index flatten)*
- [[Plotting with Matplotlib (Pandas)]] -> Parent Framework: [[Data Visualisation (Chart Types)]] *(Week 4)*
- [[Linear Regression in Python (scipy)]] -> Parent Framework: [[Linear and Polynomial Regression]] *(Week 5)*
- [[Scikit-learn Classification and Clustering]] -> Parent Framework: [[Predictive Models]] *(Week 7; trees/forest/k-means)*
- [[Data Auditing in Pandas]] -> Parent Framework: [[Data Wrangling]] *(Week 3/4)*
- [[Unix Shell for Data Science]] -> Parent Framework: [[Data Wrangling]] *(Weeks 9 & 10; awk/grep/cut/pipes)*
- [[R Modelling (lm and Decision Trees)]] / [[R Visualisation (base graphics)]] *(Week 8 R lab)*

## 🧭 Suggested Reading Order

1. [[Data Science]] — the spectrum of definitions (from the circular "what a data scientist does" to the broad "extraction of value from data across the lifecycle"), Hal Varian's framing, and **Drew Conway's Venn diagram** (hacking skills ∩ maths/stats ∩ substantive expertise; the machine-learning, traditional-research, and danger-zone regions).
2. [[Machine Learning]] — the widely-agreed definition (algorithms that let computers learn, grounded in statistics) and the six situations where ML earns its keep (no human expertise, tacit expertise, automatic adaptation, changing conditions, large data, humans too expensive).
3. [[Data Science Process (Standard Value Chain)]] — the 10 illustrative project tasks and the unit's model: Collection → Engineering → Governance → Wrangling → Analysis → Visualisation → Operationalize.
4. [[Data Science vs Related Disciplines]] — how data science differs from data engineering, data analysis, and data management, and the data-scientist / chief-data-scientist / chief-scientist roles.
5. [[Data Scientist Roles and Skills]] — the analyst / scientist / engineer distinction (by primary output), the five skill groups, the four styles (businesspeople, creatives, developers, researchers), and the *Data Analytics Handbook* lessons (communication, curiosity, collection & wrangling as the hardest steps).
6. [[Impact of Data Science]] — societal impact across three lenses (life in the cloud / datafication, social good, futurology in healthcare and self-driving cars), always weighing benefit against privacy/ethics.
7. [[Data Business Models]] — traditional IT models (SaaS, consulting, CRM) vs the four data-specific models (information brokering, information-based differentiation, information-based delivery network, information provider), with Amazon as the worked case.
8. [[Python for Data Science]] — why Python (readable, flexible, library-rich, IEEE top language) and the Anaconda environment manager; data types and libraries are covered in the video lectures and lab.
9. [[Data Sources and Open Data]] — the data landscape (databases, files, web/crowd, IoT, mobile), open data and its World Bank benefits, CSV, and Linked Open Data (subject–verb–object triples, DBpedia).
10. [[APIs for Data Collection]] — accessing new data sources programmatically; the consumer/provider split, REST APIs, and examples (OpenWeather, Twitter/X, Google Maps).
11. [[Data Wrangling]] — transforming raw data into tidy, analysable data (raw → wrangling → tidy → analysis → knowledge; Data + Wrangling + Analysis = Data Product).
12. [[Data Quality Problems]] — the common issues (interpretability, format, inconsistency/misspelling, irregularities, integrity violations, missing values, outliers, duplicates) each with a detect → fix strategy, including the IQR and 3σ outlier rules.
13. [[Data Auditing in Pandas]] — the initial audit workflow (`shape`, `head`/`tail`, `info`, `describe`, `corr`, `unique`/`value_counts`) to profile a new dataset and surface quality problems.
14. [[Types of Data (Numeric and Categorical)]] — numeric (discrete/continuous) vs categorical (nominal/ordinal); the classification that dictates chart and statistic choices.
15. [[Data Visualisation (Chart Types)]] — purpose and the chart-per-type map (histogram/boxplot/motion for numeric; frequency table/bar/pie for categorical), histogram binning maths, and motion (bubble) charts.
16. [[Measures of Centrality]] — the statistic $s(y)$, descriptive vs inferential, mean/median/mode, mean-vs-median robustness, and reading skew from (mean − median).
17. [[Measures of Spread and Boxplots]] — range, variance/standard deviation, percentiles/quartiles, the IQR, and the five-number-summary boxplot with its outlier rule.
18. [[Association Between Variables]] — Pearson correlation (linear only; $r\approx0$ ≠ independence; correlation ≠ causation) and the visual test per type pair (scatter, side-by-side bars, side-by-side boxplots).
19. [[Groupby-Aggregate Pipeline (Pandas)]] — split-apply-combine `groupby`, multi-aggregation with `.agg({...})`, and custom lambda aggregators.
20. [[Plotting with Matplotlib (Pandas)]] — `plt`/`df.plot` for bar, pie, line, scatter, histogram, and boxplot, matched to the data type.
21. [[Predictive Models]] — models (understand + predict), predictive-model output types, classifier vs regression, learning from examples in a feature space, and evaluating on held-out test data.
22. [[Machine Learning]] *(extended)* — the ML definition (patterns/inference, no explicit instructions) and the four-step development workflow (measure of success → evaluation protocol → benchmark → better model + hyperparameter tuning).
23. [[Machine Learning Styles (Supervised vs Unsupervised)]] — supervised (labelled → classification/regression; linear regression, random forest, SVM) vs unsupervised (unlabelled → clustering/association; k-means, Apriori).
24. [[Learning Theory and Loss Functions]] — learning theory and the unknowable "true model", quality/loss/gain/error, and loss functions (absolute, square, hinge) that turn error into quality.
25. [[Linear and Polynomial Regression]] — fitting $\hat y = a_0 + a_1 x$ (and higher-order polynomials) by minimising squared-residual loss / MSE, regression terminology (independent/dependent variables, observations), when to use it (relate variables, forecast), residuals, and learning curves.
26. [[Bias-Variance Tradeoff (Underfitting vs Overfitting)]] — how model complexity trades bias against variance (underfit = high bias, overfit = high variance), and the train/test split used to detect it.
27. [[No Free Lunch Theorem]] — Wolpert & Macready: no universally best algorithm with finite data; match and evaluate algorithms per problem.
28. [[Ensemble Models]] — a collection of reasonable models whose averaged predictions capture the realistic range and improve performance.
29. [[Classification Evaluation (Confusion Matrix and Metrics)]] — the confusion matrix (TP/FP/FN/TN) and the metrics (accuracy, sensitivity/recall, specificity, false-positive rate, precision), plus choosing the right metric by error cost (spam vs fraud).
30. [[Decision Trees and Regression Trees]] — reading a tree as rules, recursive partitioning of the feature space, leaf prediction (mode vs mean), and split/stop criteria (entropy/information gain; ID3/C4.5/CART).
31. [[Random Forest]] — an ensemble of decision trees whose votes/averages reduce a single tree's overfitting.
32. [[k-means Clustering]] — unsupervised grouping by similarity: $k$, centroids as means, the assign↔move iteration to convergence, initialisation sensitivity, and choosing $k$.
33. [[R for Data Science]] — why R (statistics-first, interpreted, open-source) and R vs Python.
34. [[R Basics (Syntax, Types, Control Flow)]] — `<-` assignment, data types (numeric/integer/complex/logical/character), `class`/`as`/`is`, operators, and `if`/`for`/`while`/`break`/`next`.
35. [[R Vectors]] — `c()`, positive/negative/range indexing, element-wise arithmetic, and `anyNA`/`is.na`.
36. [[R Data Frames and IO]] — `data.frame`, auditing (`str`/`summary`/`dim`), `[row, col]`/`$` extraction, `order` sorting, `merge`/`rbind`, `aggregate`, and CSV/working-directory/library I/O.
37. [[R Visualisation (base graphics)]] — `barplot` (via `table`), `hist`, `boxplot` (formula + `$out` outliers), and `plot` scatter.
38. [[R Modelling (lm and Decision Trees)]] — `lm(y ~ x)` (coefficients, `summary`, R²) and `ctree` decision trees.
39. [[Big Data and the Vs]] — characterising data by Laney's V's (Volume/Velocity/Variety = bigness; Veracity/Variability = problems; Visualisation/Value = aspirations) and the "moving target" definition of Big Data.
40. [[Metadata]] — structured data about data (descriptive/structural/administrative) and why it matters for discovery, reuse, and governance.
41. [[Growth Laws (Moore, Koomey, Bell, Zimmerman)]] — the exponential trends behind Big Data: Moore (transistors), Koomey (energy efficiency), Bell (new computer classes), Zimmerman (surveillance vs privacy).
42. [[Unix Shell for Data Science]] — inspecting and wrangling large files from the CLI (`cd`/`ls`/`cp`, `less`/`cat`/`head`/`tail`, `grep`/`wc`, `sort`, pipes `|`, redirects `>`, wildcards, `awk`), and why buffered pipes scale.
43. [[SQL vs NoSQL Databases]] — the database landscape (RDBMS/NoSQL/graph) and the five SQL-vs-NoSQL differences (relational, schema, scaling, model, transactions) with suitability.
44. [[Distributed Processing and Map-Reduce]] — processing modes (interactive/streaming/batch), the distributed-computing concepts, and the Map-Reduce paradigm (map → sort → reduce) via word count.
45. [[Hadoop and Spark]] — Hadoop (disk-based batch Map-Reduce) vs Spark (in-memory, real-time, much faster), and which suits real-time.
46. [[Data Management and Data Governance]] — data management (the internal DAMA lifecycle) vs data governance (external usage/value: access, protection, compliance, accountability), and the conflicting business/legal objectives.
47. [[Privacy, Confidentiality, and Security]] — the three distinct protection concepts, and implicit vs explicit data (inference as the confidentiality threat).
48. [[Data Compliance and Regulations (PDPA, GDPR)]] — ethics and compliance, PCI, the PDPA's nine obligations, and how GDPR goes further (72-hour breach notice, up to 4% turnover / €20M).

## 🎯 Learning Outcomes

After Week 1 you should be able to: explain what data science is and articulate Drew Conway's Venn diagram (including the "danger zone"); comprehend the usefulness of machine learning and the situations that motivate it; explain the components of a data science process (the standard value chain from collection through to operationalisation); differentiate data science from related disciplines (data engineering, data analysis, data management) and the associated roles; and (in the lab) install and start coding in Python with Jupyter Notebook.

After Week 2 you should be able to: comprehend the essentials for coding in Python for data science (why Python, the Anaconda environment) and explain/interpret given Python code; explain the different data science roles and skills and the differences between them — data analyst (insights), data scientist (models/products), data engineer (infrastructure), the five skill groups and four styles from *Analyzing the Analyzers*; explain the impact of data science (data in the cloud/datafication, social good, futurology) and its privacy/ethics trade-offs; and explain the data business models organisations use (traditional IT models plus the four data-specific ones, e.g. how Amazon uses data to compete).

After Week 3 you should be able to: explain open data and linked open data (machine-readable, publicly available; the World Bank benefits; CSV; subject–verb–object triples as in DBpedia); explain how to access new data sources through APIs and identify how different APIs work (consumer vs provider, REST APIs, keys, examples such as OpenWeather and Twitter/X); inspect data-quality problems in a dataset and recommend fixes (interpretability, format, inconsistency/misspelling, irregularities, integrity-constraint violations, missing values, outliers via the IQR/3σ rules, and duplicates — each with a detection method and an impute/remove/standardise fix that must be justified); and use data-wrangling and auditing operations in Python/pandas (`df.shape`, `head`/`tail`, `info`, `describe` for numeric and object columns, `corr`, `unique`, `value_counts`).

After Week 4 you should be able to: comprehend more sophisticated group-by operations and graphing in Python (`groupby` split-apply-combine, `.agg` with multiple/custom aggregators, and matplotlib/pandas plotting); comprehend the power of data visualisation as preliminary analysis; differentiate visualisation approaches and where each is appropriate (histogram vs bar chart, pie charts for ≤6 categories, boxplots, motion/bubble charts, and the scatter/side-by-side-bar/side-by-side-boxplot choices for association) based on the data type (numeric discrete/continuous, categorical nominal/ordinal); and explain and differentiate descriptive-statistics concepts — a statistic $s(y)$, measures of centrality (mean/median/mode, robustness, skew), measures of spread (range, variance/standard deviation, percentiles, IQR, the five-number-summary boxplot), and association (Pearson correlation, its linear-only limitation, and correlation ≠ causation).

After Week 5 you should be able to: explain what models and predictive models are and analyse them across examples (classifier vs regression, prediction output types, learning from examples in a feature space); understand how to evaluate predictive models (train vs held-out test, and how more data/features affect performance); explain machine learning (learning from patterns/inference without explicit instructions) and its development workflow, and differentiate supervised (classification/regression) from unsupervised (clustering/association) learning styles with their example algorithms; understand learning theory and the role of loss functions (absolute/square/hinge) in turning error into a measure of quality; and analyse how to estimate a linear-regression model — $\hat y = a_0 + a_1 x$ fitted by minimising squared-residual loss — extending to polynomial regression, and apply both in Python (in tutorials).

After Week 6 you should be able to: fit linear and polynomial regression models to a dataset (in tutorials), using the correct terminology (independent/dependent variables, observations) and knowing when to use regression (relating variables, forecasting), fitting by minimising the squared-residual loss/MSE; explain underfitting and overfitting of different models and how model complexity drives them; comprehend the bias–variance trade-off (high bias = underfitting/inaccuracy, high variance = overfitting/instability) and the role of a non-overlapping train/test split; comprehend the importance of the No Free Lunch theorem (no universally best algorithm with finite data); and explain what ensemble models are (a collection of reasonable models whose averaged predictions improve performance and express prediction variability).

After Week 7 you should be able to: differentiate classification from regression models; analyse a confusion matrix and calculate prediction accuracy, and differentiate the classification metrics (accuracy, sensitivity/recall, specificity, false-positive rate, precision) and when each matters (spam filter vs fraud detector vs Covid test); explain how decision trees and regression trees work (recursive partitioning of the feature space, reading a tree as rules, predicting the region's mode vs mean, and the split/stop criteria); explain how a random forest works (an ensemble of decision trees aggregated by vote/average to cut overfitting); and explain how k-means clustering works (choose $k$, iterate cluster-assignment and centroid-move to convergence, and the sensitivity to initial centroids).

After Week 8 you should be able to: comprehend the essentials for coding in R for data science (why R, the RStudio environment, and how R compares with Python); explain and interpret given R commands — assignment with `<-`, the basic data types and conversions, operators, and control flow (`if`, `for`, `while`, `break`, `next`); and apply R commands for data wrangling, exploration and analysis (vectors with `c()` and indexing, data frames with auditing/extraction/sorting/merging/aggregation, CSV read/write and libraries), for visualisation (`barplot`, `hist`, `boxplot`, scatter `plot`), and for analysis (`lm` linear regression and `ctree` decision trees).

After Week 9 you should be able to: characterise the data sets used to assess a data science project (the V's, metadata, dimensions of data, growth laws); explain what Big Data is (a moving target beyond the reach of common tools) and understand the V's (Laney's Volume/Velocity/Variety plus Veracity, Variability, Visualisation and Value); understand and analyse the growth laws — Moore's (transistor count), Koomey's (energy efficiency), Bell's (new computer classes) and Zimmerman's (surveillance vs privacy); and analyse and use shell commands to read and manipulate big data (navigation, `less`/`cat`/`head`/`tail`, `grep`/`wc`, `sort` with flags, pipes, redirects, wildcards, and `awk`).

After Week 10 you should be able to: characterise different database types (RDBMS, NoSQL, graph) and differentiate SQL from NoSQL databases across the five key differences (relational vs non-relational, fixed vs dynamic schema, vertical vs horizontal scaling, table vs document/key-value/graph/wide-column, multi-row transactions vs unstructured data) with their suitability; define distributed processing (parallel/distributed/data-parallel, in-memory vs disk, scalability) and the processing modes (interactive, streaming, batch); analyse the Map-Reduce framework (divide → map to key-value → sort/merge → reduce, on fault-tolerant commodity hardware); differentiate Hadoop (disk-based batch) from Spark (in-memory, real-time, faster); and apply R/shell commands to read and manipulate big data files.

After Week 11 you should be able to: differentiate data-management requirements from an internal (data-lifecycle) perspective and an external (data-value-chain/governance) perspective; understand the conflicting business and legal objectives (extracting value vs meeting regulations); and explain the relationship between ethics, privacy, storage, security and analysis — distinguishing privacy, confidentiality and security, recognising implicit vs explicit data, and knowing the compliance regimes (PCI, the PDPA's nine obligations, and the stricter GDPR with its 72-hour breach notification and turnover-based penalties).
