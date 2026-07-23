---
unit: FIT1058
parent: "[[Summation Notation]]"
tags: [Math/Discrete, Math/Sequences, Monash/CS_DS]
---
# [[Geometric Series]]

**Context:** [[FIT1058_MOC]] · the sum of a [[Arithmetic, Geometric, and Harmonic Sequences|geometric sequence]] · finite closed form + convergent infinite case · companion to [[Arithmetic Series]]

> [!abstract] Quick Revision
> - **🎯 Objective:** sum $a+ar+\dots+ar^{n-1}$ ➔ $S_n=a\frac{r^n-1}{r-1}$ ($r\neq1$).
> - **📦 Core Components:** finite closed form ➔ infinite $\frac{a}{1-r}$ if $|r|<1$.
> - **⚡ Critical Bottleneck:** converges **iff** $|r|<1$; $r=1$ handled separately ($S_n=na$).

## 📝 Core
### 1. The Series
- **Definition** ➔ first term $a$, ratio $r$: $S_n=\sum_{i=0}^{n-1}ar^i$.
- **Closed form** ➔ $S_n=a\frac{r^n-1}{r-1}$ ($r\neq1$); $S_n=na$ if $r=1$.

### 2. Finite Sum Trick
- **Multiply by $r$** ➔ $rS_n=S_n-a+ar^n$ ⟹ $(r-1)S_n=a(r^n-1)$.
- **Check** ➔ $a=1,r=2$: $1+2+\dots+2^n=2^{n+1}-1$.

### 3. Infinite Sum
- **$|r|<1$** ➔ $r^n\to0$ ⟹ $S_\infty=\frac{a}{1-r}$.
- **$|r|\ge1$** ➔ diverges ($|r|>1$/$r=1$) or no limit ($r=-1$).

**Key identities:**

$$S_n=a\cdot\frac{r^n-1}{r-1}\ (r\neq1),\qquad S_\infty=\frac{a}{1-r}\ (|r|<1)$$

> [!NOTE] **Crossover Invariant:** vs [[Arithmetic Series]] — arithmetic always diverges in size (terms don't shrink); geometric converges exactly when terms decay ($|r|<1$). For $r>1$, $S_n=\Theta(r^n)$ — the node count $\sum 2^i=2^{k+1}-1$ of a perfect [[Binary Tree]].

## 📊 Exam Execution Trace

### Manual Execution Trace
$a=3,r=2$, 5 terms:

| Step / State | $i$ | term | running $S$ |
| :--- | :--- | :--- | :--- |
| **0 (Init)** | 0 | 3 | 3 |
| 1 | 1 | 6 | 9 |
| 2 | 2 | 12 | 21 |
| 3 | 3,4 | 24,48 | 45,93 |

## ⚠️ Pitfalls
- 💡 **$r=1$ breaks the formula** ➔ the denominator $r-1=0$; then every term is $a$ so $S_n=na$. Infinite sum needs the *strict* $|r|<1$.

## 🧠 Active Recall
> [!FAQ]- Derive the finite geometric sum $S_n=a\frac{r^n-1}{r-1}$ and when it needs different handling.
> - **Core Insight Requirement:** Multiply and subtract.
> > [!SUCCESS]- Answer
> > - **Direct Criterion:** $rS_n=S_n-a+ar^n$ ⟹ $(r-1)S_n=a(r^n-1)$; requires $r\neq1$ (else $S_n=na$).
> > - **Technical Justification:** **Shift** ➔ multiplying by $r$ shifts terms by one.

> [!FAQ]- When does an infinite geometric series converge, and why does an arithmetic one never?
> - **Core Insight Requirement:** Term decay.
> > [!SUCCESS]- Answer
> > - **Direct Criterion:** Converges iff $|r|<1$ (then $\frac{a}{1-r}$); arithmetic terms $a+id$ don't decay.
> > - **Technical Justification:** **$r^n\to0$** ➔ only decaying terms give a finite limit.
