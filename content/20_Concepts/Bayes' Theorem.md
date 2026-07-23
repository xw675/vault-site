---
unit: FIT1058
parent: "[[Conditional Probability]]"
tags: [Math/Probability, DS/MachineLearning, Monash/CS_DS]
---
# [[Bayes' Theorem]]

**Context:** [[FIT1058_MOC]] · reverses a [[Conditional Probability|conditional]] · updates a prior belief into a posterior given evidence · denominator from the [[Law of Total Probability]]

> [!abstract] Quick Revision
> - **🎯 Objective:** convert $\mathrm{Pr}(B\mid A)$ into $\mathrm{Pr}(A\mid B)$ ➔ $\frac{\mathrm{Pr}(B\mid A)\mathrm{Pr}(A)}{\mathrm{Pr}(B)}$.
> - **📦 Core Components:** prior ➔ likelihood ➔ posterior; denominator via total probability.
> - **⚡ Critical Bottleneck:** $\mathrm{Pr}(A\mid B)\neq\mathrm{Pr}(B\mid A)$ — confusing them is the base-rate fallacy.

## 📝 Core
### 1. The Theorem
- **Formula** ➔ $\mathrm{Pr}(A\mid B)=\frac{\mathrm{Pr}(B\mid A)\mathrm{Pr}(A)}{\mathrm{Pr}(B)}$.
- **Belief updating** ➔ prior $\mathrm{Pr}(A)$ → posterior $\mathrm{Pr}(A\mid B)$ after observing $B$.

### 2. Proof & Extended Form
- **Proof** ➔ two expressions for $\mathrm{Pr}(A\cap B)$; equate and divide by $\mathrm{Pr}(B)$.
- **Extended** ➔ over a partition, denominator $=\sum_i\mathrm{Pr}(B\mid A_i)\mathrm{Pr}(A_i)$ ([[Law of Total Probability]]).

### 3. Prior → Posterior
- **Can rise/fall/hold** ➔ observing Heads: DoubleHead $\tfrac13\to\tfrac23$, DoubleTail $\tfrac13\to0$, Fair unchanged.
- **Normalisation shortcut** ➔ posteriors over a partition sum to 1.

> [!NOTE] **Crossover Invariant:** posteriors over a partition sum to 1, so a missing one can be found by subtraction. Bayesian updating underpins statistics and machine learning; if $A,B$ independent the posterior equals the prior.

## 📊 Exam Execution Trace

### Manual Execution Trace
Three coins, observe Heads:

| Step / State | Hypothesis | prior | likelihood | posterior |
| :--- | :--- | :--- | :--- | :--- |
| **0 (Init)** | — | — | — | — |
| 1 | Fair | $\tfrac13$ | $\tfrac12$ | $\tfrac13$ |
| 2 | DoubleHead | $\tfrac13$ | 1 | $\tfrac23$ |
| 3 | DoubleTail | $\tfrac13$ | 0 | 0 |

## ⚠️ Pitfalls
- 💡 **Direction matters** ➔ $\mathrm{Pr}(A\mid B)\neq\mathrm{Pr}(B\mid A)$; Bayes is the correction factor $\mathrm{Pr}(A)/\mathrm{Pr}(B)$ (base-rate fallacy).

## 🧠 Active Recall
> [!FAQ]- State and prove Bayes' Theorem.
> - **Core Insight Requirement:** Two forms of $\mathrm{Pr}(A\cap B)$.
> > [!SUCCESS]- Answer
> > - **Direct Criterion:** $\mathrm{Pr}(A\mid B)=\frac{\mathrm{Pr}(B\mid A)\mathrm{Pr}(A)}{\mathrm{Pr}(B)}$.
> > - **Technical Justification:** **Equate** ➔ $\mathrm{Pr}(B)\mathrm{Pr}(A\mid B)=\mathrm{Pr}(A)\mathrm{Pr}(B\mid A)$, divide.

> [!FAQ]- What are prior and posterior, and how does the extended form get its denominator?
> - **Core Insight Requirement:** Before/after + total probability.
> > [!SUCCESS]- Answer
> > - **Direct Criterion:** Prior = before evidence, posterior = after; denominator $=\sum_i\mathrm{Pr}(B\mid A_i)\mathrm{Pr}(A_i)$.
> > - **Technical Justification:** **Normalise** ➔ the total-probability sum makes posteriors sum to 1.
