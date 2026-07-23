---
unit: FIT2094
parent: "[[Normalisation]]"
tags: [CS/Databases, SWE/Design, Monash/CS_DS]
aliases: [1NF]
---
# [[First Normal Form (1NF)]]

**Context:** [[FIT2094_MOC]] · a valid [[Relation (Database)|relation]] with a PK and **no repeating groups** · the first [[Normalisation]] step · partial dependencies listed here

> [!abstract] Quick Revision
> - **🎯 Objective:** a valid relation with a PK and no repeating groups ➔ the first normalisation step.
> - **📦 Core Components:** unique PK ➔ atomic cells ➔ all attributes depend on all/part of the PK.
> - **⚡ Critical Bottleneck:** still leaves **partial** and **transitive** dependencies — list partial dependencies here.

## 📝 Core
### 1. The 1NF Conditions
- **Unique PK** ➔ identified for each tuple.
- **Valid relation** ➔ entity integrity (no part of PK NULL), atomic cells (no repeating groups).
- **Dependence** ➔ all attributes functionally depend on all or part of the PK.

### 2. UNF → 1NF Steps
- **Identify PK** ➔ for the main relation.
- **Remove repeating group** ➔ into a new relation, bringing the original PK.
- **New PK** ➔ usually composite (original PK + repeating group's identifier).

### 3. List Partial Dependencies
- **Definition** ➔ non-key depends on **part** of a composite key.
- **Example** ➔ $\text{vendor\_no}\to\text{vendor\_name}$ in RESTOCK.
- **Removed at** ➔ [[Second Normal Form (2NF)|2NF]].

> [!NOTE] **Crossover Invariant:** if the UNF had no repeating group (ENROLMENT), 1NF creates **no** new relation — only a PK is added. 1NF *is* the valid-relation requirement ([[Relation Properties]]) plus a PK; anomalies persist until 2NF/3NF.

## 📊 Exam Execution Trace

### Manual Execution Trace
UNF → 1NF for PART:

| Step / State | Action | Result |
| :--- | :--- | :--- |
| **0 (Init)** | UNF PART | bracketed group |
| 1 | identify PK | part_no |
| 2 | remove repeating group | RESTOCK |
| 3 | new PK | (part_no, vendor_no, restock_date) |

## ⚠️ Pitfalls
- 💡 **Move the repeating group, never flatten** ➔ a multivalued cell breaks atomicity; 1NF removes only repeating groups, leaving partial/transitive dependencies.

## 🧠 Active Recall
> [!FAQ]- State the conditions for 1NF and the UNF→1NF steps.
> - **Core Insight Requirement:** PK + atomic + remove repeating group.
> > [!SUCCESS]- Answer
> > - **Direct Criterion:** Unique PK, entity integrity, atomic cells; move the repeating group to a new relation carrying the original PK.
> > - **Technical Justification:** **Composite new PK** ➔ usually original PK + repeating group's identifier.

> [!FAQ]- What must you list at 1NF, and why is 1NF still anomaly-prone?
> - **Core Insight Requirement:** Partial dependencies remain.
> > [!SUCCESS]- Answer
> > - **Direct Criterion:** List all partial dependencies; 1NF removes only repeating groups.
> > - **Technical Justification:** **2NF/3NF** ➔ partial and transitive dependencies remain until removed later.
