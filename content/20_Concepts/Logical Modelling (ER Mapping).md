---
unit: FIT2094
parent: "[[Conceptual vs Logical Model]]"
tags: [CS/Databases, SWE/Design, Monash/CS_DS]
---
# [[Logical Modelling (ER Mapping)]]

**Context:** [[FIT2094_MOC]] · transform a [[Conceptual Model|conceptual ER model]] into a relational schema · entity→relation, key→PK, relationship→FK · database-type-dependent

> [!abstract] Quick Revision
> - **🎯 Objective:** transform a conceptual ER model to a relational schema ➔ Step 2 of design.
> - **📦 Core Components:** entity→relation ➔ identifier→PK ➔ relationship→FK.
> - **⚡ Critical Bottleneck:** relationships are **not** relations; database-type-dependent (vendor-free).

## 📝 Core
### 1. The Mapping
- **Step 2** ➔ choose a database type (relational) and transform.
- **Rules** ➔ entity → [[Relation (Database)|relation]]; identifier → [[Primary Key]]; relationship → [[Foreign Key and Referential Integrity|FK]] (PK/FK pair).

### 2. Three-Level Terminology
- **Conceptual** ➔ entity / attribute / instance / identifier / relationship.
- **Logical** ➔ relation / attribute / tuple / PK / **FK**.
- **Physical** ➔ table / column / row / PK / FK (vendor-dependent).

### 3. Preserved Characteristics
- **Unique relation name + PK** ➔ each relation.
- **Atomic attributes** ➔ one [[Domain (Relational Model)|domain]] each, order immaterial.
- **Logical links** ➔ PK/FK pairs, no physical pointers.

## ⚖️ Core Decision Matrix
| Level | Dependence | Output |
| :--- | :--- | :--- |
| conceptual | model-independent | ER diagram |
| logical | DB type (vendor-free) | relational schema |
| physical | vendor-specific | schema file |
| relationship | — | FK, not a relation |

> [!NOTE] **Crossover Invariant:** bottom-up [[Normalisation|3NF]] relations integrate with this top-down ER mapping (unify attribute names). The relationship **line is kept** even after the FK — it carries optionality developers need. Surrogate keys may now be introduced ([[Surrogate Key]]).

## 📊 Exam Execution Trace

### Manual Execution Trace
Mapping CUSTOMER places ORDER:

| Step / State | Conceptual | Logical |
| :--- | :--- | :--- |
| **0 (Init)** | — | — |
| 1 | CUSTOMER entity | CUSTOMER relation, PK custno |
| 2 | ORDER entity | ORDERS relation, PK orderno |
| 3 | places | ORDERS.custno FK |

## ⚠️ Pitfalls
- 💡 **Relationships are not relations** ➔ realised by placing the parent's PK as an FK in the child; only entities become relations.

## 🧠 Active Recall
> [!FAQ]- Give the conceptual→logical→physical terminology, and the general ER-to-relational rule.
> - **Core Insight Requirement:** Entity→relation, relationship→FK.
> > [!SUCCESS]- Answer
> > - **Direct Criterion:** Entity→Relation→Table; Attribute→Attribute→Column; Instance→Tuple→Row; Key→PK; Relationship→FK.
> > - **Technical Justification:** **Not relations** ➔ relationships become FKs (parent PK in child).

> [!FAQ]- After mapping a relationship to a PK/FK pair, why keep the relationship line?
> - **Core Insight Requirement:** Optionality info.
> > [!SUCCESS]- Answer
> > - **Direct Criterion:** The PK/FK gives connectivity, but the line conveys optionality/cardinality.
> > - **Technical Justification:** **Business rules** ➔ e.g. a customer may exist without orders.
