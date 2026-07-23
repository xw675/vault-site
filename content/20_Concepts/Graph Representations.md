---
unit: FIT1058
parent: "[[Graph]]"
tags: [Math/GraphTheory, CS/DataStructures, Monash/CS_DS]
---
# [[Graph Representations]]

**Context:** [[FIT1058_MOC]] · symbolic ways to store a [[Graph]] in memory · edge list, adjacency matrix, adjacency list, incidence matrix · trade space against access

> [!abstract] Quick Revision
> - **🎯 Objective:** store a [[Graph]] symbolically for algorithms ➔ four standard encodings.
> - **📦 Core Components:** edge list ➔ adjacency matrix ➔ adjacency list ➔ incidence matrix.
> - **⚡ Critical Bottleneck:** matrix = $n^2$ bits, $O(1)$ test; list = compact for **sparse** graphs.

## 📝 Core
### 1. The Four Representations
- **Edge list** ➔ set of edges (+ $V$, else isolated vertices vanish).
- **Adjacency matrix** ➔ $n\times n$ bit array, $A_{vw}=1$ iff $v\sim w$; symmetric, zero diagonal.
- **Adjacency list** ➔ per vertex, its neighbours ($c:a,b,d$; $e:$ empty).
- **Incidence matrix** ➔ $v\times e$ bit array, $1$ iff vertex is an endpoint; each column has two $1$s.

### 2. What the Structure Encodes
- **Row sum** ➔ $\deg(v)$ ([[Degree and the Handshaking Lemma]]).
- **Total $1$s** ➔ $2m$.
- **"Matrix"** ➔ algebraic operations reveal structure.

## ⚖️ Core Decision Matrix
| Representation | Space | Adjacency test | Best for |
| :--- | :--- | :--- | :--- |
| adjacency matrix | $n^2$ | $O(1)$ | dense |
| adjacency list | $O(m)$ | $O(\deg)$ | sparse |
| edge list | $O(m)$ + $V$ | scan | compact |
| incidence matrix | $v\times e$ | — | proofs |

> [!NOTE] **Crossover Invariant:** the adjacency matrix is the [[Binary Relation]]'s $0/1$ matrix over $V\times V$; row/column sums are degrees, total $1$s $=2m$. Sparse real graphs favour the list; the incidence matrix is mostly theoretical.

## 📊 Exam Execution Trace

### Manual Execution Trace
Rows for $a,c,e$ (order $a$–$g$):

| Step / State | Vertex | Row | Degree |
| :--- | :--- | :--- | :--- |
| **0 (Init)** | — | — | — |
| 1 | $a$ | $0110000$ | 2 |
| 2 | $c$ | $1101000$ | 3 |
| 3 | $e$ | $0000000$ | 0 |

## ⚠️ Pitfalls
- 💡 **Edge list needs $V$** ➔ isolated vertices ($e$) have no edges; matrix is $n^2$ bits regardless, list stores only actual edges.

## 🧠 Active Recall
> [!FAQ]- Describe the adjacency matrix and adjacency list, and when each is preferable.
> - **Core Insight Requirement:** Dense vs sparse.
> > [!SUCCESS]- Answer
> > - **Direct Criterion:** Matrix = $n\times n$ bits, $O(1)$ test, $n^2$ space; list = neighbours per vertex, $O(m)$ space.
> > - **Technical Justification:** **Sparse wins list** ➔ real graphs store no empty entries.

> [!FAQ]- Why must an edge list include the vertex set, and what does an incidence matrix encode?
> - **Core Insight Requirement:** Isolated vertices; endpoints.
> > [!SUCCESS]- Answer
> > - **Direct Criterion:** Edge list omits isolated vertices, so $V$ is needed; incidence matrix marks vertex-endpoint pairs (two $1$s per column).
> > - **Technical Justification:** **Theoretical** ➔ incidence matrix is used mainly for proofs.
