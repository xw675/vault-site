---
unit: FIT2094
parent: "[[Entity (Conceptual Modelling)]]"
tags: [CS/Databases, SWE/Design, Monash/CS_DS]
---
# [[Attribute (Conceptual Modelling)]]

**Context:** [[FIT2094_MOC]] · a property of an [[Entity (Conceptual Modelling)|entity]] · key vs non-key · types: simple/composite, single/multi-valued, derived

> [!abstract] Quick Revision
> - **🎯 Objective:** a property describing an entity ➔ key attributes identify, non-key describe.
> - **📦 Core Components:** simple/composite ➔ single/multi-valued ➔ derived.
> - **⚡ Critical Bottleneck:** a multivalued attribute has no Crow's Foot symbol → becomes a separate (weak) entity.

## 📝 Core
### 1. The Attribute
- **Definition** ➔ a property of an [[Entity (Conceptual Modelling)|entity]].
- **Key** ➔ uniquely identifies instances (`custno`); flagged `Key` in the first column.
- **Non-key** ➔ describes but doesn't identify (`custname`, `custaddress`).

### 2. Three Classification Axes
- **Simple vs composite** ➔ indivisible (`age`) vs subdividable (`address`→street/city/postcode).
- **Single vs multi-valued** ➔ one value (`tax_file_number`) vs several (`degrees`).
- **Derived** ➔ computed from others (`age` from `date_of_birth`; order total from lines).

### 3. Multivalued → Weak Entity
- **No symbol** ➔ Crow's Foot lacks a multivalued marker (unlike Chen).
- **Resolution** ➔ store as a separate (usually weak) entity (`CAR_COLOR`).

**Key identities:**

$$\text{CUSTOMER}(\underline{\text{custno}}, \text{custname}, \text{street}, \text{city}, \text{postcode})$$
$$\text{ORDER}(\underline{\text{orderno}}, \text{orderdate}) \quad \text{[total = }\Sigma\text{ line items, derived]}$$

## ⚖️ Core Decision Matrix
| Axis | Types | Logical effect |
| :--- | :--- | :--- |
| structure | simple / composite | composite splits into parts |
| multiplicity | single / multi-valued | multi → new entity |
| origin | stored / derived | derived carried with sources |
| role | key / non-key | key → PK |

> [!NOTE] **Crossover Invariant:** classification is **client-driven** — the same field (phone number) may be simple or composite, single- or multi-valued, depending on requirements. Names share an entity prefix (`cust_…`), underscores not spaces.

## 📊 Exam Execution Trace

### Manual Execution Trace
Classifying attributes:

| Step / State | Attribute | Axes |
| :--- | :--- | :--- |
| **0 (Init)** | — | — |
| 1 | `age` | simple, single, derived |
| 2 | `address` | composite, single |
| 3 | `degrees` | simple, multi-valued |

## ⚠️ Pitfalls
- 💡 **Carry a derived attribute alongside its sources** ➔ during design always include every client-required attribute; store-vs-compute is decided later with sample data, not at conceptual stage.

## 🧠 Active Recall
> [!FAQ]- Classify attributes along the three axes with an example of each.
> - **Core Insight Requirement:** Three independent axes.
> > [!SUCCESS]- Answer
> > - **Direct Criterion:** Simple/composite (`age`/`address`); single/multi-valued (`tfn`/`degrees`); derived (`age` from DOB).
> > - **Technical Justification:** **Key cuts across** ➔ a `Key` attribute identifies; non-key describes.

> [!FAQ]- How is a multivalued attribute represented in Crow's Foot, and why?
> - **Core Insight Requirement:** No symbol.
> > [!SUCCESS]- Answer
> > - **Direct Criterion:** As a separate (weak) entity — `car_color` → `CAR_COLOR`.
> > - **Technical Justification:** **Relations are single-valued** ➔ each value gets its own row linked to the parent.
