---
unit: FIT1008
parent: "[[Abstract Data Type (ADT)]]"
tags: [CS/DataStructures, OOP/Python, CS/Abstraction]
---
# [[Iterable]]

**Context:** [[FIT1008_MOC]] · a collection that can produce an [[Iterator]] · makes [[List (ADT)|LinkList]] work with `for` · enables [[List Comprehension]]

> [!abstract] Quick Revision
> - **🎯 Objective:** any object you can loop over ➔ produces a fresh [[Iterator]] on demand via __iter__.
> - **📦 Core Components:** the **Iterator design pattern** — separate *what to traverse* from *how*.
> - **⚡ Critical Bottleneck:** `__iter__` is $O(1)$; traversal is the iterator's $O(n)$ — and can be **lazy/infinite**.

## 📝 Core
### 1. The Iterable (`__iter__`)
- **Produces** ➔ a **fresh [[Iterator]]** each `__iter__` call ➔ invoked by `for`, `iter()`, comprehensions, `max`, `in`.
- **Encapsulation** ➔ traverse a [[List (ADT)|LinkList]] with `for item in a_list` without touching `head`/`link`.
- **Pattern** ➔ the **Iterator pattern** (GoF) — separates *what to traverse* from *how*.

### 2. Iterable vs Iterator
- **Iterable** ➔ has `__iter__` (yields a *new* iterator, re-iterable).
- **Iterator** ➔ has `__iter__` **and** `__next__` (holds position, single-use).
- **One-way** ➔ every iterator is iterable, but **not** conversely — a LinkList is iterable, not an iterator (no `__next__`).
- **Laziness** ➔ iterator mediation lets an iterable be **lazy/infinite** (`itertools.count()`, a file, a [[Generator Expression]]).

## ⚙️ Core Implementation
### 🔹 `__iter__` returns a fresh iterator
> [!code]- making a LinkList iterable
> ```python
> class LinkList(List[T]):
>     def __iter__(self) -> LinkListIterator[T]:
>         return LinkListIterator(self.head)     # a FRESH iterator at the head
>
> for item in a_list: ...      # Python calls __iter__ once, then next() until StopIteration
> [x for x in a_list]; max(a_list); 5 in a_list   # all consume an iterable
> ```
> 💡 **Exam Pitfall:** **`__iter__` must return a fresh iterator** ➔ so two loops don't interfere — *unless* the object is itself an iterator, in which case `__iter__` returns the same (exhausting) object.

## ⚖️ Core Decision Matrix
| Property | Iterable | [[Iterator]] |
| :--- | :--- | :--- |
| methods | `__iter__` | `__iter__` **+** `__next__` |
| holds position? | no | yes |
| re-iterable? | yes (fresh each call) | no (single-use) |
| can be lazy/infinite? | yes (via its iterator) | yes |
| example | LinkList, str, range | LinkListIterator, generator |

> [!NOTE] **Crossover Invariant:** encapsulation (traverse without internals) + uniformity (one syntax over lists, strings, ranges, trees, custom classes). Because elements come from the iterator's `__next__` on demand, an iterable can represent an unbounded sequence in $O(1)$ memory.

## 📊 Exam Execution Trace

### Manual Execution Trace
What `for x in a_list` does:

| Step / State | Call |
| :--- | :--- |
| **0 (Init)** | — |
| 1 | `it = a_list.__iter__()` (fresh iterator) |
| 2..n | `x = it.__next__()` until... |
| end | `StopIteration` → loop ends |

### Applied Exercise
**Problem:** Show iterable ⊇ iterator but not conversely.
**Derivation Proof / Hand-Calculation Walkthrough:**
$$
\begin{aligned}
\text{Iterator} &\Rightarrow \text{Iterable (has }\texttt{\_\_iter\_\_}\text{)} \\
\text{Iterable} &\not\Rightarrow \text{Iterator (LinkList has no }\texttt{\_\_next\_\_}\text{)}
\end{aligned}
$$
**Final Extracted Output:** iterators are a strict subset of iterables — holding a cursor is the extra requirement.

## 🧠 Active Recall
> [!FAQ]- Distinguish an iterable from an iterator precisely, and why is a `LinkList` one but not the other?
> - **Core Insight Requirement:** `__iter__` vs `__iter__`+`__next__`.
> > [!SUCCESS]- Answer
> > - **Direct Criterion:** Iterable has `__iter__` (fresh iterator, re-loopable); iterator adds `__next__` (holds position, single-use).
> > - **Technical Justification:** **No `__next__`** ➔ LinkList returns a new `LinkListIterator` each call, so multiple independent loops run over one list.

> [!FAQ]- How does the iterator protocol let an iterable be infinite or lazy?
> - **Core Insight Requirement:** On-demand production.
> > [!SUCCESS]- Answer
> > - **Direct Criterion:** Elements come from the iterator's `__next__` only when asked, so nothing materialises.
> > - **Technical Justification:** **$O(1)$ memory** ➔ `itertools.count()`, a file, a generator expression represent unbounded sequences a list could not.

> [!FAQ]- What design pattern does making a class iterable implement, and what does it decouple?
> - **Core Insight Requirement:** What vs how.
> > [!SUCCESS]- Answer
> > - **Direct Criterion:** The **Iterator pattern** (GoF) — decouples what a collection holds from how it's traversed.
> > - **Technical Justification:** **Representation-agnostic** ➔ clients depend only on `__iter__`/`__next__`, so array/linked/tree internals can change without breaking loops.
