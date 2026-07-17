---
unit: FIT2099
type: MOC
tags: [Monash/CS_DS, 2026/S1]
---
# 📘 FIT2099: Object-Oriented Design and Implementation

> [!INFO] Map of Content
> Index for **FIT2099 Object-Oriented Design and Implementation** (Java). Domain B: every design note carries a Mermaid `classDiagram`; designs are judged on **Coupling / Cohesion / Extensibility**. Start with [[OOP Building Blocks (Class, Object, Field, Method)]].

## 📊 Assessment Map

- **Assessment:** engine-based Java group project across milestones + individual work *(⚠ splits unverified — fill from unit outline)*.
- **Assessed skills:** design rationale in Coupling/Cohesion/Extensibility terms, UML/Mermaid diagrams, SOLID application, smell → refactor.

## 🧰 Toolkit Cheatsheets (pinned — pre-lab / pre-exam single re-reads)
- 📌 [[FIT2099 Unit Cheatsheet]] — whole-unit exam crib — principles, smells→refactors, contracts, UML rules
- [[Java Toolkit (Cheatsheet)]] — code a class from a blank editor: class anatomy, modifiers, types/`==`-vs-`equals`, collections, inheritance/polymorphism/interfaces/enums, exceptions/DbC/CQS, DI/defensive copying, Factory Method, and the smell→refactoring quick-map.
- [[UML Toolkit (Cheatsheet)]] — draw from a blank page: class-diagram compartments/visibility/**relationship-arrow legend**/multiplicity/stereotypes, sequence-diagram lifelines/messages/activation/fragments, and the domain/activity/use-case/CRC modelling tools (Mermaid syntax throughout).

## 📅 Knowledge Index

### Week 1 — Java & OO Fundamentals
- [[Java Static Typing]] -> Parent Framework: [[Java Program Structure]]
- [[Java Program Structure]] -> Parent Framework: [[OOP Building Blocks (Class, Object, Field, Method)]]
- [[OOP Building Blocks (Class, Object, Field, Method)]] -> Parent Framework: [[Java Program Structure]]
- [[Java Data Types, Casting and References]] -> Parent Framework: [[OOP Building Blocks (Class, Object, Field, Method)]]
- [[Java Constructors]] -> Parent Framework: [[OOP Building Blocks (Class, Object, Field, Method)]]
- [[Java Control Flow (Conditionals and Loops)]] -> Parent Framework: [[Java Program Structure]]
- [[Java Arrays]] -> Parent Framework: [[Java Program Structure]]
- [[Client-Supplier Relationship (Java)]] -> Parent Framework: [[OOP Building Blocks (Class, Object, Field, Method)]]

### Week 2 — Modifiers, UML Relationships, Design Principles & Inheritance
- [[Java Packages and Imports]] -> Parent Framework: [[Java Program Structure]]
- [[Encapsulation and Access Modifiers (Java)]] -> Parent Framework: [[OOP Building Blocks (Class, Object, Field, Method)]]
- [[Static and Final (Java)]] -> Parent Framework: [[OOP Building Blocks (Class, Object, Field, Method)]]
- [[UML Associations and Dependencies (Java)]] -> Parent Framework: [[Client-Supplier Relationship (Java)]]
- [[Three Core Design Principles (Java)]] -> Parent Framework: [[Client-Supplier Relationship (Java)]]
- [[Inheritance (Java)]] -> Parent Framework: [[OOP Building Blocks (Class, Object, Field, Method)]]

### Week 3 — Collections, Polymorphism & Abstraction
- [[Java Collections (List, Set, Map)]] -> Parent Framework: [[Java Arrays]]
- [[Polymorphism (Java)]] -> Parent Framework: [[Inheritance (Java)]]
- [[Abstract Classes (Java)]] -> Parent Framework: [[Inheritance (Java)]]
- *(deepened this week: [[Static and Final (Java)]] — static↔instance access matrix, why-use/why-carefully; [[Encapsulation and Access Modifiers (Java)]] — encapsulation boundaries & ReD; [[Java Packages and Imports]] — `module-info.java`)*

### Week 4 — Interfaces & Enumerations
- [[Interfaces (Java)]] -> Parent Framework: [[Abstract Classes (Java)]]
- [[Enumerations (Java)]] -> Parent Framework: [[Three Core Design Principles (Java)]]
- *(deepened this week: [[Java Data Types, Casting and References]] — `==` (identity) vs `.equals()` (value) & the String Pool)*

### Week 5 — SOLID Principles
- [[SOLID Principles (Java)]] -> Parent Framework: [[Three Core Design Principles (Java)]]  *(hub: overview table, ReD, LCOM, downcasting/`instanceof`)*
- [[Single Responsibility Principle (Java)]] -> Parent Framework: [[SOLID Principles (Java)]]
- [[Open-Closed Principle (Java)]] -> Parent Framework: [[SOLID Principles (Java)]]
- [[Liskov Substitution Principle (Java)]] -> Parent Framework: [[SOLID Principles (Java)]]
- [[Interface Segregation Principle (Java)]] -> Parent Framework: [[SOLID Principles (Java)]]
- [[Dependency Inversion Principle (Java)]] -> Parent Framework: [[SOLID Principles (Java)]]

### Week 6 — Applying Abstraction: Injection, Copying & Rationale
- [[Dependency Injection (Java)]] -> Parent Framework: [[Dependency Inversion Principle (Java)]]
- [[Defensive Copying (Java)]] -> Parent Framework: [[Encapsulation and Access Modifiers (Java)]]
- [[Design Rationale (FIT2099)]] -> Parent Framework: [[SOLID Principles (Java)]]  *(⭐ Assignment 1 writing artefact)*
- *(deepened this week: [[Dependency Inversion Principle (Java)]] — hinge point + DI link; [[Encapsulation and Access Modifiers (Java)]] — abstraction-layer sizing & connascence)*

### Week 7 — Dynamic Modelling
- [[UML Sequence Diagrams (Java)]] -> Parent Framework: [[UML Associations and Dependencies (Java)]]  *(⭐ Assignment interaction diagrams)*

### Week 8 — Design by Contract, Exceptions & Factory
- [[Design by Contract (Java)]] -> Parent Framework: [[Client-Supplier Relationship (Java)]]
- [[Command-Query Separation (Java)]] -> Parent Framework: [[Design by Contract (Java)]]
- [[Exceptions, Assertions and Validation (Java)]] -> Parent Framework: [[Design by Contract (Java)]]
- [[Factory Method Pattern (Java)]] -> Parent Framework: [[Abstract Classes (Java)]]  *(first GoF pattern)*
- *(deepened this week: [[Liskov Substitution Principle (Java)]] — the DbC subcontracting formulation, weaker-pre/stronger-post)*

### Week 9 — Code & Design Smells + Refactoring
- [[Design Smells (Java)]] -> Parent Framework: [[SOLID Principles (Java)]]  *(smell catalogue + smell→refactoring map)*
- [[Refactoring (Java)]] -> Parent Framework: [[Design Smells (Java)]]

### Week 10 — Refactoring to Address Code Smells
- *(deepened this week: [[Refactoring (Java)]] — the refactor-to-enable-change motivation (Fowler `statement()` scenario) + the identify→fix→apply→test→commit→repeat loop; no new note — Week 10 is a worked deepening of the Week 9 material.)*

### Week 11 — Design in the Lifecycle, Technical Debt & the Design Process
- [[Software Design in the Lifecycle (FIT2099)]] -> Parent Framework: [[FIT2099_MOC]]  *(when/why to design; SDLC + Lean)*
- [[Technical Debt (FIT2099)]] -> Parent Framework: [[Refactoring (Java)]]
- [[Design Process and Techniques (FIT2099)]] -> Parent Framework: [[Software Design in the Lifecycle (FIT2099)]]  *(how to design)*
- [[CRC Cards (FIT2099)]] -> Parent Framework: [[Design Process and Techniques (FIT2099)]]

### 📐 UML Notation References (consolidated)
- [[UML Class Diagrams (Java)]] — the **static** notation legend: box compartments, `+`/`-`/`#`/`~` visibility, stereotypes, and the full relationship-arrow table (generalisation / realization / association / dependency / aggregation / composition) + multiplicity. *(Class-diagram syntax was taught piecemeal across the Week 2 associations/inheritance decks and the abstract-class/interface UML slides; this note gathers it in one place.)*
- [[UML Sequence Diagrams (Java)]] — the **dynamic** notation legend (see Week 7).

## 🧭 Suggested Reading Order

1. [[Java Static Typing]] — Java is statically typed (a variable's type is fixed at declaration), so the compiler catches type errors at **compile time** that Python only catches at runtime.
2. [[Java Program Structure]] — the anatomy of a Java program: `public class` matching the file name, the `main` entry point (`public static void main(String[] args)`), `System.out.println`, and semicolons.
3. [[OOP Building Blocks (Class, Object, Field, Method)]] — the four building blocks: class (blueprint) vs object (instance), fields (attributes/data) and methods (behaviours).
4. [[Java Data Types, Casting and References]] — primitives vs `String`/reference types, value-vs-reference (heap) semantics, widening/narrowing casts, and class-vs-local scope.
5. [[Java Constructors]] — the special same-named method that runs on `new`, the default zero-arg constructor, overloaded constructors, `this`, and declaration/instantiation/initialisation.
6. [[Java Control Flow (Conditionals and Loops)]] — `if`/`else`, the ternary operator, `switch` (with `break`), and the `while` / `do-while` / `for` / `for-each` loops.
7. [[Java Arrays]] — creating (literal or `new T[n]`), accessing/updating by 0-based index, and `.length`.
8. [[Client-Supplier Relationship (Java)]] — one class as a client of others (holding them as fields and calling their methods), knowing only *how to call* not *how they work* — the first taste of coupling.
9. [[Java Packages and Imports]] — grouping classes into namespaces (`package` first, then `import`), fully-qualified names, and why wildcard imports are discouraged.
10. [[Encapsulation and Access Modifiers (Java)]] — hiding state behind `private` fields with selective accessors; the `public`/`protected`/default/`private` visibility table.
11. [[Static and Final (Java)]] — the non-access modifiers: `static` (class-level, one shared copy) and `final` (assign-once, constants, reference non-transitivity).
12. [[UML Associations and Dependencies (Java)]] — has-a (association, stored field, solid `-->`) vs uses-a (dependency, method parameter, dashed `..>`), multiplicity, and the aggregation/composition read-only caveat.
13. [[Three Core Design Principles (Java)]] — DRY, classes responsible for their own properties (SRP-seed / feature-envy smell), and avoiding excessive literals.
14. [[Inheritance (Java)]] — `extends` (is-a generalisation), `super` for constructors/members, `protected`, method overriding + `@Override`, the access-widening rule, and `final` to block inheritance.
15. [[Java Collections (List, Set, Map)]] — resizable `ArrayList`/`HashSet`/`HashMap`, generics + wrapper types, program-to-the-interface, and the List/Set/Map decision table.
16. [[Polymorphism (Java)]] — upcasting a subclass into a base-type variable, runtime (dynamic) dispatch of overridden methods, polymorphic containers, and the base-variable-hides-subclass-methods trade-off.
17. [[Abstract Classes (Java)]] — the never-instantiated base type, abstract methods (no body), concrete-vs-abstract, and the UML italics/`«abstract»` convention.
18. [[Interfaces (Java)]] — pure capability contracts, `implements` (one `extends`, many interfaces), default methods, the interface/abstract/concrete table, and `«interface»` realization arrows.
19. [[Enumerations (Java)]] — type-safe named constants that fix the magic-number/string smell, `switch` on an enum, and the `«enumeration»` UML stereotype.
20. [[SOLID Principles (Java)]] — the five design guidelines as a set (overview table, ReD, the LCOM cohesion metric, and the downcasting/`instanceof` smell), then one smell→refactor note per principle: [[Single Responsibility Principle (Java)|SRP]], [[Open-Closed Principle (Java)|OCP]], [[Liskov Substitution Principle (Java)|LSP]], [[Interface Segregation Principle (Java)|ISP]], [[Dependency Inversion Principle (Java)|DIP]].
21. [[Dependency Injection (Java)]] — supplying a class's collaborators from outside (constructor/setter/interface injection), the client/service/interface/injector roles, DI vs DIP, and mock-based testing.
22. [[Defensive Copying (Java)]] — preventing a privacy leak by copying mutable objects on the way in and out of a class (aliasing, mutable vs immutable).
23. [[Design Rationale (FIT2099)]] — ⭐ the Assignment 1 justification artefact: design goals, reason + alternative + trade-off per decision, and the marked don'ts (restating SOLID, describing not justifying, over-future-proofing/YAGNI).
24. [[UML Sequence Diagrams (Java)]] — ⭐ the dynamic/interaction diagram: objects & lifelines (concrete classes only), synchronous/return messages, activation bars, object create/delete, and the `loop`/`alt`/`opt` control-flow fragments.
25. [[Design by Contract (Java)]] — client/supplier obligations: preconditions, postconditions, invariants; blame-on-breach (precondition→exception, postcondition→assertion); fail-fast; subcontracting as the DbC form of LSP. Plus [[Command-Query Separation (Java)]], [[Exceptions, Assertions and Validation (Java)]], and the first GoF pattern, [[Factory Method Pattern (Java)]].
26. [[Design Smells (Java)]] — Fowler's subjective catalogue of surface symptoms (Bloaters, Change Preventers, Couplers, Procedural, Dispensables, Overengineering) and the smell→refactoring-step map; the Divergent-Change⇄Shotgun-Surgery opposition; "branching on type information" → Replace Conditional with Polymorphism. Then [[Refactoring (Java)]] — the behaviour-preserving treatment: Fowler's definition, the identify-smell→apply→test→commit→repeat loop, the "two hats" (refactor first, then add feature), refactoring to make future change easier, and tests as the safety net.
27. [[Software Design in the Lifecycle (FIT2099)]] — where design sits in the SDLC (Waterfall: requirements→analysis→design→implementation→verification→maintenance; what / what-mean / how), the messy overlap in practice, Lean just-in-time/just-enough design (decide as late as possible), when to do conscious design (inception/architectural, complex-or-risky, refactoring), and the goal of shared understanding in stakeholders' heads. Then [[Technical Debt (FIT2099)]] — quick-messy vs clean-slow, the burn-down gap, the Reckless/Prudent × Deliberate/Inadvertent quadrant, and repayment by refactoring to a *better* design. Then [[Design Process and Techniques (FIT2099)]] — design as a creative act, understanding the domain first, brainstorming/model storming, top-down vs bottom-up, and scenario-based design/use cases — refined with [[CRC Cards (FIT2099)]] (Class–Responsibility–Collaboration, scenario role-play, SRP-driven splitting, collaborations→associations).

## 🎯 Learning Outcomes

1. Iteratively apply OO **design principles** to design small-to-medium systems using UML class diagrams and interaction diagrams.
2. Describe the **quality** of OO designs — meeting requirements and the effective application of OO concepts/principles.
3. Apply OO programming constructs — **abstraction, information hiding, inheritance, polymorphism** — to implement designs in **Java**.
4. Apply effective strategies to **refactor and debug** OO implementations using language tools.
5. Apply software-engineering practice with peers using IDEs, UML tools, and version control.

*(Week 1 covers LO3 foundations — the Java language and the class/object model — before the design principles and UML of later weeks.)*
*(Week 2 opens LO1/LO2 — UML relationships and OO design principles — plus the LO3 inheritance/encapsulation constructs. Domain-B scope note: model with **Association, Dependency, and Inheritance**; aggregation/composition are read-only.)*
*(Week 3 completes the core LO3 OO toolkit — **polymorphism** and **abstraction** — and adds the applied Java Collections API; the static/final, encapsulation and packages notes were deepened rather than duplicated.)*
*(Week 4 adds **interfaces** (capability contracts / multiple type inheritance) and **enumerations** (type-safe constants), rounding out the abstraction toolkit; the data-types note gained `==` vs `.equals()`.)*
*(Week 5 is the design-rationale core (LO1/LO2): the **SOLID** principles — the vocabulary for justifying design decisions in the assignment. A hub note holds the overview; each principle has its own smell→refactor pattern note.)*
*(Week 6 applies abstraction in practice (LO3/LO4): **dependency injection** (implementing DIP), **defensive copying** (protecting encapsulation), and the **Design Rationale** writing artefact that the Assignment is graded on. The Constants recap is already covered by the Enumerations/Static-and-Final notes.)*
*(Week 7 adds **dynamic modelling** (LO1): UML **sequence diagrams** to document runtime interactions — the behavioural companion to the static class diagram, and an Assignment deliverable alongside the rationale.)*
*(Week 8 covers **Design by Contract** (LO2/LO3): pre/postconditions & invariants, exception-vs-assertion blame, fail-fast, and subcontracting (the DbC form of LSP) — plus Command-Query Separation, exception/validation mechanics, and the first GoF creational pattern (Factory Method).)*
*(Week 9 is the **refactor/debug** outcome (LO4): recognising **code & design smells** as maintainability symptoms and mapping each to a **refactoring step**, then the discipline of **refactoring** itself (behaviour-preserving, test-driven, two hats). Ties back to SOLID/OCP (type-branching → polymorphism) and composition. No new toolkit code — conceptual + design-example material.)*
*(Week 10 continues LO4: a worked **refactoring** deepening (Fowler's theatrical `statement()` — refactor to make the HTML/plaintext + new-play-type changes easy). Folded into the existing Refactoring note rather than duplicated.)*
*(Week 11 is the **process/meta** outcome (LO1/LO5): where design fits in the **lifecycle** and *when/why* to design (Lean, just-enough), **technical debt** and its prudent/reckless quadrant, and *how* designers actually work — creative approaches (top-down/bottom-up/scenario-based) and **CRC cards**. Process-level material; no new code toolkit.)*
