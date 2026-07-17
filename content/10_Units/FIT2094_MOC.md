---
unit: FIT2094
type: MOC
tags: [Monash/CS_DS, 2026/S1]
---
# 📘 FIT2094: Databases

> [!INFO] Map of Content
> Index for **FIT2094 Databases**. Each link below is a standalone atomic note. Start with [[Database Design Life Cycle]] and follow the links. Conceptual modelling uses **Crow's Foot** notation throughout.

## 📊 Assessment Map

- **Written Assignment (70%)** ➔ THE unit: design (ER → logical → normalised) + executable Oracle SQL; fed by Weeks 2–10 and [[Oracle SQL Toolkit (Cheatsheet)]].
- **Test (30%)** ➔ theory: relational model, relational algebra, normalisation reasoning. No exam.

## 🧰 Toolkit Cheatsheets (pinned — pre-lab / pre-exam single re-reads)
- 📌 [[FIT2094 Unit Cheatsheet]] — whole-unit exam crib — design pipeline, normalisation, SQL decision rules, transactions, NoSQL
- [[Oracle SQL Toolkit (Cheatsheet)]] -> integrates Topics 8–9: anatomy, predicates, functions, joins, subqueries + integration katas

## 📅 Knowledge Index

### Week 2 — Conceptual Modelling (ER, Crow's Foot)
- [[Database Design Life Cycle]] -> Parent Framework: [[Conceptual Model]]
- [[Conceptual Model]] -> Parent Framework: [[Database Design Life Cycle]]
- [[Entity Relationship Diagram (ERD)]] -> Parent Framework: [[Conceptual Model]]
- [[Entity (Conceptual Modelling)]] -> Parent Framework: [[Entity Relationship Diagram (ERD)]]
- [[Attribute (Conceptual Modelling)]] -> Parent Framework: [[Entity (Conceptual Modelling)]]
- [[Relationship (Conceptual Modelling)]] -> Parent Framework: [[Entity Relationship Diagram (ERD)]]
- [[Cardinality (Crow's Foot Notation)]] -> Parent Framework: [[Relationship (Conceptual Modelling)]]
- [[Identifying vs Non-Identifying Relationship]] -> Parent Framework: [[Relationship (Conceptual Modelling)]]
- [[Associative Entity]] -> Parent Framework: [[Relationship (Conceptual Modelling)]]
- [[Conceptual vs Logical Model]] -> Parent Framework: [[Conceptual Model]]

### Week 3 — The Relational Model and Relational Algebra
- [[Relational Model]] -> Parent Framework: [[Conceptual vs Logical Model]]
- [[Domain (Relational Model)]] -> Parent Framework: [[Relational Model]]
- [[Relation (Database)]] -> Parent Framework: [[Relational Model]]
- [[Relation Properties]] -> Parent Framework: [[Relation (Database)]]
- [[Functional Dependency]] -> Parent Framework: [[Relation (Database)]]
- [[Super Key and Candidate Key]] -> Parent Framework: [[Relation (Database)]]
- [[Primary Key]] -> Parent Framework: [[Super Key and Candidate Key]]
- [[Foreign Key and Referential Integrity]] -> Parent Framework: [[Primary Key]]
- [[Data Integrity]] -> Parent Framework: [[Relational Model]]
- [[NULL Value]] -> Parent Framework: [[Relational Model]]
- [[Relational Algebra]] -> Parent Framework: [[Relational Model]]
- [[Select and Project (σ, π)]] -> Parent Framework: [[Relational Algebra]]
- [[Set Operations in Relational Algebra]] -> Parent Framework: [[Relational Algebra]]
- [[Relational Algebra Joins]] -> Parent Framework: [[Relational Algebra]]

### Week 4 — Normalisation
- [[Database Anomalies]] -> Parent Framework: [[Normalisation]]
- [[Functional Dependency]] -> Parent Framework: [[Relation (Database)]] *(extended in Week 4: full/partial/transitive/total)*
- [[Normalisation]] -> Parent Framework: [[Relational Model]]
- [[Unnormalised Form (UNF)]] -> Parent Framework: [[Normalisation]]
- [[First Normal Form (1NF)]] -> Parent Framework: [[Normalisation]]
- [[Second Normal Form (2NF)]] -> Parent Framework: [[Normalisation]]
- [[Third Normal Form (3NF)]] -> Parent Framework: [[Normalisation]]
- [[Synthesis (Normalisation)]] -> Parent Framework: [[Normalisation]]

### Week 5 — Logical Modelling (ER → Relational)
- [[Logical Modelling (ER Mapping)]] -> Parent Framework: [[Conceptual vs Logical Model]]
- [[Mapping Entities and Attributes (Logical)]] -> Parent Framework: [[Logical Modelling (ER Mapping)]]
- [[Mapping Binary Relationships (Logical)]] -> Parent Framework: [[Logical Modelling (ER Mapping)]]
- [[Mapping Unary and Ternary Relationships (Logical)]] -> Parent Framework: [[Logical Modelling (ER Mapping)]]
- [[Logical Modelling Constraints]] -> Parent Framework: [[Logical Modelling (ER Mapping)]]
- [[Surrogate Key]] -> Parent Framework: [[Primary Key]]

### Week 6 — Physical Design & DDL (Oracle)
- [[Personal Data and Privacy in Database Design]] -> Parent Framework: [[Database Design Life Cycle]]
- [[SQL Sublanguages (DDL, DML, DCL)]] -> Parent Framework: [[Relational Model]]
- [[Oracle Data Types]] -> Parent Framework: [[SQL Sublanguages (DDL, DML, DCL)]]
- [[DDL Table Creation]] -> Parent Framework: [[SQL Sublanguages (DDL, DML, DCL)]]
- [[Altering and Dropping Tables]] -> Parent Framework: [[DDL Table Creation]]
- [[Column Value Constraints (Check vs Lookup)]] -> Parent Framework: [[Data Integrity]]
- [[Foreign Key and Referential Integrity]] -> Parent Framework: [[Primary Key]] *(extended in Week 6: on-delete RESTRICT/CASCADE/SET NULL)*

### Week 7 — DML & Transactions
- [[DML INSERT (Oracle)]] -> Parent Framework: [[SQL Sublanguages (DDL, DML, DCL)]]
- [[DML UPDATE and DELETE (Oracle)]] -> Parent Framework: [[SQL Sublanguages (DDL, DML, DCL)]]
- [[Database Transaction]] -> Parent Framework: [[SQL Sublanguages (DDL, DML, DCL)]]
- [[ACID Properties]] -> Parent Framework: [[Database Transaction]]
- [[Concurrency Control and Locking]] -> Parent Framework: [[Database Transaction]]
- [[Deadlock]] -> Parent Framework: [[Concurrency Control and Locking]]
- [[Database Recovery]] -> Parent Framework: [[Database Transaction]]

### Week 8 — SQL Querying (SELECT)
- [[SQL SELECT and WHERE]] -> Parent Framework: [[SQL Sublanguages (DDL, DML, DCL)]]
- [[SQL Sorting, Distinct & Alias]] -> Parent Framework: [[SQL SELECT and WHERE]]
- [[SQL Formatting Functions (NVL, TO_CHAR, TO_DATE)]] -> Parent Framework: [[SQL SELECT and WHERE]]
- [[SQL Joins (ANSI)]] -> Parent Framework: [[SQL SELECT and WHERE]]
- [[SQL Subquery (Nested SELECT)]] -> Parent Framework: [[SQL SELECT and WHERE]]

### Week 9 — SQL Intermediate (Aggregation & Subqueries)
- [[SQL Aggregate Functions and GROUP BY]] -> Parent Framework: [[SQL SELECT and WHERE]]
- [[SQL Subquery (Nested SELECT)]] -> Parent Framework: [[SQL SELECT and WHERE]] *(extended in Week 9: scalar / column / multi-column output types, ANY/ALL)*

### Week 10 — Advanced SQL
- [[SQL Conditional Expressions (CASE, DECODE)]] -> Parent Framework: [[SQL SELECT and WHERE]]
- [[SQL Subquery Approaches (Nested, Correlated, Inline)]] -> Parent Framework: [[SQL Subquery (Nested SELECT)]]
- [[Populating Tables from Queries (INSERT-SELECT, CTAS)]] -> Parent Framework: [[DDL Table Creation]]
- [[SQL Views]] -> Parent Framework: [[SQL SELECT and WHERE]]
- [[SQL Self Join and Outer Join]] -> Parent Framework: [[SQL Joins (ANSI)]]
- [[SQL Set Operators]] -> Parent Framework: [[SQL SELECT and WHERE]]
- [[SQL Formatting Functions (NVL, TO_CHAR, TO_DATE)]] -> Parent Framework: [[SQL SELECT and WHERE]] *(extended in Week 10: EXTRACT, LPAD/RPAD, LTRIM/TRIM)*
- [[Query Processing and the Optimiser]] -> Parent Framework: [[SQL SELECT and WHERE]]

### Week 11 — Big Data & NoSQL (Relational vs Non-Relational)
- [[Big Data and the Vs]] -> Parent Framework: [[Relational Model]]
- [[NoSQL Databases]] -> Parent Framework: [[Big Data and the Vs]]
- [[NoSQL Data Models]] -> Parent Framework: [[NoSQL Databases]]
- [[MongoDB Document Model]] -> Parent Framework: [[NoSQL Data Models]]
- [[MongoDB CRUD Operations]] -> Parent Framework: [[MongoDB Document Model]]

## 🧭 Suggested Reading Order

1. [[Database Design Life Cycle]] — the four stages (Requirements → Conceptual → Logical → Physical), what each produces and how technology-dependence increases down the stages.
2. [[Conceptual Model]] — a high-level, technology-independent, stakeholder-readable view; ER methodology; the "model exactly the brief" rule.
3. [[Entity Relationship Diagram (ERD)]] (Chen rectangles/ovals/diamonds vs **Crow's Foot** three-partition entities + cardinality lines — the unit's standard) → [[Entity (Conceptual Modelling)]] (real-world object; **strong vs weak**) → [[Attribute (Conceptual Modelling)]] (key/non-key; simple/composite; single/multi-valued; derived) → [[Relationship (Conceptual Modelling)]] (degree: unary/binary/ternary; verb labels; multiple relationships between two entities).
4. [[Cardinality (Crow's Foot Notation)]] (min/max symbols: one/many/zero) → [[Identifying vs Non-Identifying Relationship]] (solid vs dashed line; key inheritance) → [[Associative Entity]] (resolving M:N into two 1:M with a bridging entity + composite key) → [[Conceptual vs Logical Model]] (entity → relation; Primary/Foreign keys; M:N must be resolved in the logical model).
5. [[Relational Model]] (Codd 1970; relation as a mathematical set; vs hierarchical/network; closure) → [[Domain (Relational Model)]] (valid atomic values; $\text{dom}(\cdot)$) → [[Relation (Database)]] (heading/schema $R(A_1..A_n)$ + body; tuple; degree = #attrs, cardinality = #tuples) → [[Relation Properties]] (set-derived: no duplicates, unordered, atomic = 1NF; relation ≠ table) → [[Functional Dependency]] ($A\to B$; determinant; basis of keys).
6. [[Super Key and Candidate Key]] (unique vs minimal/irreducible; alternate keys) → [[Primary Key]] (desirable characteristics; natural vs surrogate; composite) → [[Foreign Key and Referential Integrity]] (FK = PK elsewhere; match full PK or NULL) → [[Data Integrity]] (entity / referential / column-domain) → [[NULL Value]] (not a value; SQL only; four reasons).
7. [[Relational Algebra]] (procedural, relationally complete, closure; SQL → algebra in the DBMS) → [[Select and Project (σ, π)]] ($\sigma$ rows, $\pi$ columns with dedup) → [[Set Operations in Relational Algebra]] (union/intersect/difference; union-compatible) → [[Relational Algebra Joins]] (theta/equi/natural; product + select + project).
8. [[Database Anomalies]] (insert/update/delete from redundancy) → [[Functional Dependency]] (full/partial/transitive/total; dependency diagram) → [[Normalisation]] (bottom-up; goals; UNF→1NF→2NF→3NF) → [[Unnormalised Form (UNF)]] (form → relation; repeating group in brackets; no PK).
9. [[First Normal Form (1NF)]] (PK + remove repeating groups; list partial deps) → [[Second Normal Form (2NF)]] (remove partial deps; general/candidate-key definition; list transitive deps) → [[Third Normal Form (3NF)]] (remove transitive deps; list all full deps; PART → 4 PKs/3 FKs) → [[Synthesis (Normalisation)]] (merge same-subject 3NF relations across multiple forms).
10. [[Logical Modelling (ER Mapping)]] (entity→relation, key→PK, relationship→FK; terminology table; database-type-dependent) → [[Mapping Entities and Attributes (Logical)]] (composite → component attrs; multivalued → new relation + lookup; weak entity → inherited composite PK) → [[Mapping Binary Relationships (Logical)]] (1:M = FK on many side; M:N = bridging relation; 1:1 = FK to minimise NULLs / consolidate if total).
11. [[Mapping Unary and Ternary Relationships (Logical)]] (1:M unary = recursive renamed FK; M:N unary & ternary = associative relation with composite PK) → [[Logical Modelling Constraints]] (recursive/1:1-total identifying relationships forbidden; beware loops) → [[Surrogate Key]] (added only at logical stage; manual; UNIQUE constraint on the natural key).
12. [[Personal Data and Privacy in Database Design]] (data minimisation; client decides; privacy/anti-discrimination) → [[SQL Sublanguages (DDL, DML, DCL)]] (structure/data/access; DDL auto-commits) → [[Oracle Data Types]] (CHAR/VARCHAR2/NUMBER/DATE) → [[DDL Table Creation]] (CREATE + ALTER-add named constraints; ordering; circular deps; composite PK/FK) → [[Altering and Dropping Tables]] (ALTER modify; DROP PURGE / CASCADE CONSTRAINTS) → [[Column Value Constraints (Check vs Lookup)]] (NULL vs NOT NULL; CHECK vs lookup) → [[Foreign Key and Referential Integrity]] (on-delete RESTRICT/CASCADE/SET NULL by participation).
13. [[DML INSERT (Oracle)]] (named/positional; TO_DATE; SEQUENCE NEXTVAL/CURRVAL) → [[DML UPDATE and DELETE (Oracle)]] (SET/WHERE; subquery not hardcode; UPPER/LOWER; omit-WHERE hits all) → [[Database Transaction]] (all-or-nothing; COMMIT/ROLLBACK) → [[ACID Properties]] (atomicity/consistency/isolation/durability) → [[Concurrency Control and Locking]] (lost update; S/X locks; granularity; 2PL) → [[Deadlock]] (deadly embrace; prevention/avoidance/detection) → [[Database Recovery]] (log; checkpoint; write-through vs deferred REDO/UNDO; forward recovery).
14. [[SQL SELECT and WHERE]] (SELECT/FROM/*; schema prefix; comparison/BETWEEN/IN/LIKE/IS NULL; AND-OR-NOT precedence; three-valued logic) → [[SQL Sorting, Distinct & Alias]] (arithmetic + AS; ORDER BY ASC/DESC, NULLS FIRST/LAST, multi-col; DISTINCT) → [[SQL Formatting Functions (NVL, TO_CHAR, TO_DATE)]] (NVL type-match; TO_DATE compare; TO_CHAR date/number; sysdate/dual) → [[SQL Joins (ANSI)]] (JOIN ON / USING / NATURAL; implicit forbidden; natural-join Cartesian trap) → [[SQL Subquery (Nested SELECT)]] (= vs IN; join-in-subquery; no hardcode).
15. [[SQL Aggregate Functions and GROUP BY]] (MIN/MAX/AVG/SUM/COUNT; COUNT(*) vs COUNT(col); GROUP BY; HAVING vs WHERE; clause order; the four grouping mistakes) → [[SQL Subquery (Nested SELECT)]] (output shapes: scalar → comparison, single column → IN/ANY/ALL, multi-column → row-constructor IN; compare-to-aggregate and min-per-group).
16. [[SQL Conditional Expressions (CASE, DECODE)]] (searched/simple CASE; DECODE equality-only) → [[SQL Subquery Approaches (Nested, Correlated, Inline)]] (independent-once vs per-row vs FROM-alias vs scalar-in-SELECT) → [[Populating Tables from Queries (INSERT-SELECT, CTAS)]] (INSERT…SELECT; CTAS drops constraints) → [[SQL Views]] (virtual table; banned in A2) → [[SQL Self Join and Outer Join]] (self-join aliases; INNER vs LEFT/RIGHT/FULL) → [[SQL Set Operators]] (UNION/UNION ALL/INTERSECT/MINUS; union-compatible) → [[SQL Formatting Functions (NVL, TO_CHAR, TO_DATE)]] (EXTRACT; LPAD/RPAD; LTRIM/TRIM) → [[Query Processing and the Optimiser]] (parse→analyse→CBO→execute; nested vs correlated cost).
17. [[Big Data and the Vs]] (Volume/Velocity/Variety + more; scale up vs out; structured/semi/unstructured) → [[NoSQL Databases]] (not-only-SQL; Bigtable/Dynamo; non-relational/distributed/schema-less; sharding vs replication) → [[NoSQL Data Models]] (key-value / document / column-family / graph; aggregation vs traversal) → [[MongoDB Document Model]] (db/collection/document/field; BSON/ObjectId; embed vs reference; Oracle JSON_OBJECT/JSON_ARRAYAGG) → [[MongoDB CRUD Operations]] (insert/find/update/delete; $-operators; $ positional & $elemMatch; SQL↔Mongo map).

## 🎯 Learning Outcomes

After Week 2 you should be able to: situate conceptual modelling within the database design life cycle; explain the purpose and characteristics of a conceptual model and apply the rule that it captures exactly what the brief describes; read and draw Crow's Foot ER diagrams — entities (strong/weak), attributes (key/non-key, simple/composite, single/multi-valued, derived), and relationships (unary/binary/ternary, with verb labels and multiple relationships shown separately); express both minimum and maximum cardinality on each end of a relationship; distinguish identifying (solid) from non-identifying (dashed) relationships; resolve a many-to-many relationship with an associative/bridging entity carrying a composite key; and map a conceptual model to a relational logical model with primary and foreign keys.

After Week 3 you should be able to: explain the relational model (Codd) and why a relation is a mathematical set distinct from a table; describe a relation's heading/body and compute its degree and cardinality; state the relation properties (no duplicates, unordered, atomic = 1NF) and the role of domains; read functional dependencies $A\to B$; derive super keys, candidate keys (minimality), the primary key (natural vs surrogate, desirable characteristics), and alternate keys; implement relationships with foreign keys and enforce the three data-integrity rules (entity, referential, column/domain), including the role of NULLs; and write relational-algebra queries — SELECT ($\sigma$), PROJECT ($\pi$), union/intersect/difference (union-compatible), and theta/equi/natural joins — relating them to SQL.

After Week 4 you should be able to: explain insert/update/delete anomalies and their cause (redundancy from poor structure); classify functional dependencies as full, partial, transitive, or total and draw a dependency diagram; carry out the normalisation process UNF → 1NF → 2NF → 3NF on a form — representing the form as a UNF (repeating groups in brackets, no PK), identifying primary/candidate keys, and at each step removing repeating groups (1NF), partial dependencies (2NF, general definition), and transitive dependencies (3NF) while listing the appropriate dependencies and leaving PK/FK pairs; count the resulting PKs and FKs; and synthesise the 3NF relations from multiple forms into one integrated schema.

After Week 5 you should be able to: map a conceptual ER model to a relational logical model — entities to relations, identifiers to primary keys, and relationships to foreign keys — using the correct terminology at each design level; handle composite attributes (component attributes), multivalued attributes and weak entities (new relations); apply the relationship-mapping rules for 1:M (FK on the many side), M:N (bridging relation with composite-PK FKs), 1:1 (FK placed to minimise NULLs, or consolidate a total 1:1), 1:M unary (recursive renamed FK), M:N unary and ternary (associative relations); recognise configurations that cannot exist (recursive and 1:1-total identifying relationships, relationship loops); and add a surrogate key at the logical stage while protecting the natural key with a unique constraint.

After Week 6 you should be able to: apply data-minimisation and privacy/anti-discrimination principles when deciding which personal attributes to store (the client, not the designer, decides); classify SQL as DDL, DML, or DCL and explain why DDL auto-commits while DML is transactional (`COMMIT`/`ROLLBACK`); choose Oracle data types (`CHAR`, `VARCHAR2`, `NUMBER(p,s)`, `DATE`); write `CREATE TABLE` with inline `NOT NULL` and add every other constraint as a named table constraint via `ALTER TABLE`, in a valid creation order — resolving circular FK references by the split-then-`ALTER` method and declaring composite PK/FK pairs; evolve a schema with `ALTER TABLE` (add column/constraint, `MODIFY`, drop/enable/disable) and remove tables with `DROP TABLE ... PURGE` / `CASCADE CONSTRAINTS`; enforce column-value rules via `CHECK` constraints vs lookup tables and decide nullability; and select on-delete referential actions (RESTRICT/CASCADE/SET NULL) from the participation shown in the data model.

After Week 7 you should be able to: write DML to populate and maintain a schema — `INSERT` (named-column vs positional, NULLs for optional columns, `TO_DATE` for typed dates, `SEQUENCE` `NEXTVAL`/`CURRVAL` for numeric PKs), `UPDATE` and `DELETE` driven by a `WHERE` clause that derives filter values from a **subquery** rather than a hardcoded lookup (and never omits `WHERE` unintentionally), using `UPPER`/`LOWER` for case-insensitive matching; explain a transaction as an all-or-nothing unit controlled by `COMMIT`/`ROLLBACK` and the four `ACID` properties; describe the concurrency problem (lost update), serial vs interleaved scheduling, shared/exclusive locks and their granularity, two-phase locking, and deadlocks (deadly embrace) with prevention/avoidance/detection-and-recovery; and outline database recovery — the transaction log, checkpointing, write-through (UNDO+REDO) vs deferred-write (REDO-only) policies, and forward recovery from backups after a hard crash.

After Week 8 you should be able to: write ANSI SQL `SELECT` queries against the HiFlying Drone schema using only unit-approved syntax — choose columns (or `*`) with the correct account/schema prefix; filter rows with `WHERE` predicates (comparison operators, `BETWEEN`, `IN`/`NOT IN`, `LIKE` with `%`/`_`, `IS NULL`/`IS NOT NULL`) combined by `AND`/`OR`/`NOT` with correct precedence and three-valued (TRUE/FALSE/UNKNOWN) logic; compute and alias columns (`AS`, quoted aliases), order results (`ASC`/`DESC`, multi-column, `NULLS FIRST`/`LAST`, sort by alias) and remove duplicates with `DISTINCT`; format output with `NVL` (matching data types), `TO_DATE` (comparing dates) and `TO_CHAR` (date and number/currency pictures, `sysdate`/`dual`); join tables with ANSI `JOIN … ON`, `JOIN … USING`, and `NATURAL JOIN` (never implicit joins, and avoiding the no-common-column Cartesian trap); and retrieve values indirectly with subqueries in the `WHERE` clause (`=` for single-row, `IN` for multi-row, joins inside the subquery), never hardcoding a looked-up value.

After Week 9 you should be able to: summarise data with aggregate functions (`MIN`, `MAX`, `AVG`, `SUM`, `COUNT`), distinguishing `COUNT(*)` (all rows, incl. NULLs) from `COUNT(col)` (non-null values); group rows with `GROUP BY` and filter the resulting groups with `HAVING`, respecting the rule that every `SELECT`/`ORDER BY` column is either grouped or aggregated, the logical clause order (FROM → WHERE → GROUP BY → aggregate → HAVING → SELECT → ORDER BY), the WHERE-vs-HAVING distinction, and the common grouping errors (ungrouped columns, missing `GROUP BY`, grouping a `TO_CHAR` expression, and no aliases in `GROUP BY` on the marked Oracle version); and choose the correct subquery operator by output shape — a scalar with comparison operators (e.g. above-average), a single column with `IN`/`NOT IN`/`ANY`/`ALL`, and multiple columns with a row-constructor `(a, b) IN (...)` (e.g. the minimum price per drone type).

After Week 10 you should be able to: use advanced SQL against the HiFlying Drone schema — return conditional labels with `CASE` (searched and simple) and `DECODE` (equality only); choose a subquery approach (nested/independent, correlated/per-row, inline view in `FROM`, or scalar subquery in the `SELECT` list) and explain why a correlated subquery costs more; populate tables from a query with `INSERT … SELECT` and `CREATE TABLE AS SELECT` (knowing CTAS omits constraints); define, query, and drop a `VIEW` (while using subqueries instead of views for Assignment 2); write self-joins (aliasing a table joined to itself on a recursive FK) and outer joins (`LEFT`/`RIGHT`/`FULL`) to retain unmatched rows; combine result sets with the union-compatible set operators `UNION`, `UNION ALL`, `INTERSECT`, and `MINUS`; apply further Oracle functions (`EXTRACT` for date parts, `LPAD`/`RPAD`, `LTRIM`/`TRIM` for text alignment); and read an access plan conceptually (SQL parser → analysis → cost-based optimiser → execution) to compare query strategies, without being assessed on query efficiency.

After Week 11 you should be able to (Learning Outcome 5 — contrast non-relational with relational): explain why Big Data (the 3 Vs — Volume, Velocity, Variety, plus Variability/Veracity/Value/Visualisation) overwhelms a transactional RDBMS on both ingest and real-time retrieval, and the two scaling strategies (vertical scale-up vs horizontal scale-out on commodity servers); describe NoSQL as "not only SQL" (origins in Google Bigtable and Amazon Dynamo) with its defining characteristics (non-relational, mostly open source, distributed, schema-less) and how data is distributed by sharding vs replication; distinguish the four NoSQL data models (key-value, document, column-family, graph) by data shape and access pattern (aggregation-oriented vs traversal-oriented); model data in MongoDB (database/collection/document/field, BSON and the ObjectId `_id`, embedded/denormalised vs referenced/normalised documents, and generating JSON from Oracle with `JSON_OBJECT`/`JSON_ARRAYAGG`); and perform MongoDB CRUD (`insertOne`/`insertMany`, `find` with filters, projections and `$`-operators, `updateOne`/`updateMany` with `$set`/`$inc`, array updates with the `$` positional operator and `$elemMatch`, and `deleteOne`/`deleteMany`/`drop`), relating each to its SQL equivalent.
