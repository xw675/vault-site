---
unit: [FIT1058, FIT2014]
parent: "[[Theorem and Proof]]"
tags: [Math/Logic, Math/Proof, Math/Theory, Monash/CS_DS]
aliases: [quantifier, forall, exists, universal quantifier, existential quantifier, bound variable, quantifier order]
---
# [[Quantifiers (Existential and Universal)]]

**Context:** [[FIT1058_MOC]], [[FIT2014_MOC]] · $\exists$ "there exists" and $\forall$ "for all" · bind a [[Predicate|predicate's]] variable · each shape dictates a [[Proof Techniques|proof strategy]]

> [!abstract] Quick Revision
> - **🎯 Objective:** state how many of a domain satisfy a predicate ➔ $\exists$ = at least one, $\forall$ = every one.
> - **📦 Core Components:** bind a variable ➔ open predicate becomes a single proposition ➔ domain can change the truth value.
> - **⚡ Critical Bottleneck:** $\exists$ proven by one witness; $\forall$ needs every case; **restriction** pairs $\exists$ with $\wedge$, $\forall$ with $\Rightarrow$.

## 📝 Core
### 1. The Quantifiers (Bind a Variable)
- **Existential** ➔ $\exists x\in S,\ P(x)$ ➔ at least one element satisfies $P$.
- **Universal** ➔ $\forall x\in S,\ P(x)$ ➔ every element does.
- **Binding** ➔ quantifying a variable turns an open predicate into a proposition; applies to **variables only** ($\exists 5$ meaningless); the **domain** matters.

### 2. Proving Each Shape
- **$\exists$** ➔ exhibit **one witness** ([[Proof Techniques|construction]]) — one example finishes it.
- **$\forall$ finite** ➔ **exhaustion** (check every element).
- **$\forall$ infinite** ➔ **arbitrary element** (general unnamed $x$, argue via shared properties).
- **Disprove $\forall$** ➔ one **counterexample** ($\neg P(x)$).

### 3. Restriction Trap ($\exists\wedge$, $\forall\Rightarrow$)
- **$\exists$ uses $\wedge$** ➔ $\exists X:\text{computer}(X)\wedge\text{human}(X)$ (something that *is* a computer and human).
- **$\forall$ uses $\Rightarrow$** ➔ $\forall X:\text{computer}(X)\Rightarrow\text{human}(X)$ (if a computer, then human).
- **Analogy** ➔ $\exists$ ≈ (infinite) disjunction; $\forall$ ≈ conjunction over the domain.

### 4. Multiple Quantifiers — Order Matters (FIT2014)
- **Order changes meaning** ➔ with $\mathrm{adj}(X,Y)$ = "$X$ and $Y$ are adjacent":
  - $\exists X\,\exists Y:\neg(X=Y)\wedge\neg\mathrm{adj}(X,Y)$ ➔ *some two vertices are non-adjacent*.
  - $\forall X\,\forall Y:\neg(X=Y)\Rightarrow\mathrm{adj}(X,Y)$ ➔ *every pair is adjacent*.
  - $\exists X\,\forall Y:\neg(X=Y)\Rightarrow\mathrm{adj}(X,Y)$ ➔ *some vertex is adjacent to **all** others* (one $X$ works for every $Y$).
  - $\forall X\,\exists Y:\mathrm{adj}(X,Y)$ ➔ *every vertex has **a** neighbour* ($Y$ may depend on $X$).
- **$\exists\forall$ vs $\forall\exists$** ➔ the key distinction: $\exists X\forall Y$ demands **one** $X$ serving all $Y$; $\forall X\exists Y$ lets $Y$ **vary with** $X$. Swapping them is a classic exam error.
- **Distinctness must be stated** ➔ add $\neg(X=Y)$ explicitly; quantified variables may otherwise take the same value.
- **Restriction connective carries over** ➔ inside multiple quantifiers, $\forall$ still pairs with $\Rightarrow$ and $\exists$ with $\wedge$.

### 5. Reasoning With Quantifiers
- **Universal instantiation** ➔ $(\forall X\,\text{blah}(X))\Rightarrow\text{blah}(\mathrm{obj})$ for any specific $\mathrm{obj}$ in the domain.
- **Existential generalisation** ➔ $\text{blah}(\mathrm{obj})\Rightarrow(\exists X\,\text{blah}(X))$.
- **Distribution (only these two hold)** ➔ $\forall$ distributes over $\wedge$, $\exists$ over $\vee$:
$$\forall X\,(p(X)\wedge q(X))\equiv(\forall X\,p(X))\wedge(\forall X\,q(X)), \qquad \exists X\,(p(X)\vee q(X))\equiv(\exists X\,p(X))\vee(\exists X\,q(X))$$
- **⚠ The mixed pairings fail** ➔ $\forall X(p(X)\vee q(X))$ is **not** equivalent to $(\forall X\,p(X))\vee(\forall X\,q(X))$ (the left allows each $X$ to satisfy a different disjunct).

**Key identities:**

$$\exists x\in S,\ P(x): \text{ one witness (e.g. palindrome } \texttt{rotator}\text{) suffices}$$
$$\neg(\forall x\,P(x)) \equiv \exists x\,\neg P(x), \qquad \neg(\exists x\,P(x)) \equiv \forall x\,\neg P(x)$$
$$\neg\forall X\,(\mathrm{dog}(X)\Rightarrow\mathrm{happy}(X))\;=\;\exists X\,(\mathrm{dog}(X)\wedge\neg\mathrm{happy}(X))$$

## ⚖️ Core Decision Matrix
| Task | $\exists x\,P(x)$ | $\forall x\,P(x)$ |
| :--- | :--- | :--- |
| prove | one witness | exhaustion / arbitrary element |
| disprove | show $P$ fails for all | one counterexample |
| restriction connective | $\wedge$ | $\Rightarrow$ |
| connective analogy | $\vee$ (disjunction) | $\wedge$ (conjunction) |

> [!NOTE] **Crossover Invariant:** effort is asymmetric — $\exists$ needs one example to prove, a full argument to disprove; $\forall$ needs a full argument to prove, one counterexample to disprove. Finite vs infinite domain decides exhaustion vs arbitrary-element.

## 📊 Exam Execution Trace

### Manual Execution Trace
$S=\{2,3,4,5,6\}$, $P(x)=$ "$x$ prime":

| Step / State | $x$ | $P(x)$ | Effect |
| :--- | :--- | :--- | :--- |
| **0 (Init)** | — | — | — |
| 1 | 2 | T | witness ⟹ $\exists$ True |
| 2 | 3, 5 | T | more witnesses |
| 3 | 4 | F | counterexample ⟹ $\forall$ False |
| 4 | 6 | F | — |

## ⚠️ Pitfalls
- 💡 **Wrong restriction connective** ➔ using $\Rightarrow$ for $\exists$ is satisfied by any non-computer (too weak); using $\wedge$ for $\forall$ claims *everything* is a computer (too strong).

## 🧠 Active Recall
> [!FAQ]- Contrast proving an existential vs a universal, and why a single example differs in each.
> - **Core Insight Requirement:** Witness vs every-case.
> > [!SUCCESS]- Answer
> > - **Direct Criterion:** $\exists$ = one witness; $\forall$ = exhaustion (finite) or arbitrary element (infinite).
> > - **Technical Justification:** **Illustrate vs prove** ➔ one example proves $\exists$ but only illustrates $\forall$; one counterexample disproves $\forall$.

> [!FAQ]- How do you negate $\forall x\,P(x)$ and $\exists x\,P(x)$?
> - **Core Insight Requirement:** Swap quantifier, push negation.
> > [!SUCCESS]- Answer
> > - **Direct Criterion:** $\neg\forall x\,P(x)\equiv\exists x\,\neg P(x)$; $\neg\exists x\,P(x)\equiv\forall x\,\neg P(x)$.
> > - **Technical Justification:** **Disproof form** ➔ disprove a universal with a counterexample; disprove an existential by failing $P$ everywhere.

> [!FAQ]- Why does "some computer is human" use $\wedge$ but "every computer is human" use $\Rightarrow$?
> - **Core Insight Requirement:** Restriction asymmetry.
> > [!SUCCESS]- Answer
> > - **Direct Criterion:** $\exists$ needs something that *is* a computer **and** human; $\forall$ needs "*if* computer *then* human".
> > - **Technical Justification:** **Too weak / too strong** ➔ $\Rightarrow$ under $\exists$ is satisfied by any non-computer; $\wedge$ under $\forall$ claims everything is a computer.
