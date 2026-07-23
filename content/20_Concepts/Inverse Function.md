---
unit: FIT1058
parent: "[[Function (Mathematics)]]"
tags: [Math/Functions, Math/Discrete, Monash/CS_DS]
---
# [[Inverse Function]]

**Context:** [[FIT1058_MOC]] · reverses a [[Function (Mathematics)|function]] · exists only for a [[Injection, Surjection, Bijection|bijection]] · undoes/redoes via [[Function Composition]]

> [!abstract] Quick Revision
> - **🎯 Objective:** run a function backwards: given $y$, return the $x$ that produced it ➔ $f^{-1}(y)=$ the unique preimage.
> - **📦 Core Components:** swap graph pairs ➔ $f^{-1}\circ f=i_A$, $f\circ f^{-1}=i_B$.
> - **⚡ Critical Bottleneck:** exists **iff** $f$ is a bijection (injective → uniqueness, surjective → existence).

## 📝 Core
### 1. The Inverse (Reverse the Map)
- **Definition** ➔ $f^{-1}(y)$ = the unique $x$ with $f(x)=y$.
- **Requires** ➔ every $y$ has exactly one preimage ⟹ $f$ a [[Injection, Surjection, Bijection|bijection]].
- **Graph** ➔ swap each pair: $f^{-1}=\{(y,x):(x,y)\in f\}$.

### 2. Cancellation
- **Both ways** ➔ $f^{-1}(f(x))=x$, $f(f^{-1}(y))=y$.
- **Composition** ➔ $f^{-1}\circ f=i_A$, $f\circ f^{-1}=i_B$.

### 3. Why Bijectivity
- **Injective** ➔ removes **non-uniqueness** (several inputs share an output).
- **Surjective** ➔ removes **non-existence** (some value never produced).
- **Both** ➔ each $y$ has one and only one preimage.

**Key identities:**

$$f^{-1}=\{(y,x):(x,y)\in f\},\qquad f^{-1}\circ f=i_A,\ f\circ f^{-1}=i_B$$
$$(g\circ f)^{-1}=f^{-1}\circ g^{-1}\ (\text{socks-and-shoes})$$

## ⚖️ Core Decision Matrix
| Obstacle | Blocked by | Ensures |
| :--- | :--- | :--- |
| several inputs share output | injectivity | uniqueness |
| some value never produced | surjectivity | existence |
| both removed | bijectivity | $f^{-1}$ is a function |
| non-bijective $f$ | — | only an inverse *relation* |

> [!NOTE] **Crossover Invariant:** encryption must be bijective so decryption $=f^{-1}$ exists ([[Cryptosystem]]); $x\mapsto x^2$ on $\mathbb R$ has no inverse (not injective, not surjective). $f^{-1}$ is itself a bijection $B\to A$.

## 📊 Exam Execution Trace

### Manual Execution Trace
$f=\{(1,b),(2,c),(3,a)\}$:

| Step / State | Pair of $f$ | Swapped ($f^{-1}$) | Check |
| :--- | :--- | :--- | :--- |
| **0 (Init)** | — | — | — |
| 1 | $(1,b)$ | $(b,1)$ | $f^{-1}(f(1))=1$ |
| 2 | $(2,c)$ | $(c,2)$ | $f^{-1}(f(2))=2$ |
| 3 | $(3,a)$ | $(a,3)$ | $f^{-1}(f(3))=3$ |

## ⚠️ Pitfalls
- 💡 **Inverse *relation* always exists** ➔ swapping pairs works for any relation; it's a *function* only if $f$ was bijective (else not single-valued or not total).

## 🧠 Active Recall
> [!FAQ]- Exactly when does $f:A\to B$ have an inverse function, and why each condition?
> - **Core Insight Requirement:** Bijection = uniqueness + existence.
> > [!SUCCESS]- Answer
> > - **Direct Criterion:** Iff $f$ is a bijection; injectivity gives a unique preimage, surjectivity guarantees one exists.
> > - **Technical Justification:** **Exactly one preimage** ➔ makes $f^{-1}(y)$ well-defined.

> [!FAQ]- How is $f^{-1}$ obtained from the graph, and what equations show it undoes $f$?
> - **Core Insight Requirement:** Swap pairs.
> > [!SUCCESS]- Answer
> > - **Direct Criterion:** $f^{-1}=\{(y,x):(x,y)\in f\}$; $f^{-1}(f(x))=x$ and $f(f^{-1}(y))=y$.
> > - **Technical Justification:** **Composition** ➔ $f^{-1}\circ f=i_A$, $f\circ f^{-1}=i_B$.

> [!FAQ]- A function is not bijective — does it still have an inverse *relation*?
> - **Core Insight Requirement:** Relation vs function.
> > [!SUCCESS]- Answer
> > - **Direct Criterion:** Yes — swapping pairs always yields an inverse relation, just not necessarily a function.
> > - **Technical Justification:** **Fails single-valued/total** ➔ non-injective ⟹ multiple preimages; non-surjective ⟹ missing preimages.
