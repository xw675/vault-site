---
unit: FIT2099
parent: "[[Java Program Structure]]"
tags: [SWE/Java, SWE/OOP, Monash/CS_DS]
aliases: [Class, Object, Field, Attribute, Method, Instance]
---
# [[OOP Building Blocks (Class, Object, Field, Method)]]

**Context:** [[FIT2099_MOC]] · the four atoms of object orientation · the blueprint→instance idea · built with [[Java Constructors|constructors]], used via the [[Client-Supplier Relationship (Java)|client relationship]]
**Parent Framework:** [[Java Program Structure]]

> [!abstract] Quick Revision
> - **🎯 Objective:** model a domain thing as a class, then create objects from it ➔ class = blueprint, object = instance.
> - **📦 Core Components:** class (template) ➔ object (instance) | field/attribute (data) | method/behaviour (action).
> - **⚡ Critical Bottleneck:** a **class** is the design; an **object** is a concrete thing built from it via `new` — one class, many objects each with their own field values.

## 📝 Dashboard Blueprint
### 1. Class vs Object
- **Class** ➔ a **blueprint/template** describing how objects of that type look; the coffee-machine *design*.
- **Object** ➔ an **instance** created from the class (`new CoffeeMachine()`); an actual coffee machine off the factory line.
- **Relationship** ➔ one class → many objects, each holding its own data.

### 2. Fields (Attributes)
- **Field/attribute** ➔ a variable belonging to a class/object — a piece of **data** (`brand`, `water`).
- **Object references as fields** ➔ a field may itself be an instance of another class (`MilkContainer milkContainer`).

### 3. Methods (Behaviours)
- **Method/behaviour** ➔ an **action** an object can perform — update or return its data (`serveCoffee()`).

## ⚙️ Core Implementation
### 🔹 CoffeeMachine
> [!code]- classDiagram + Java
> ```mermaid
> classDiagram
>   class CoffeeMachine {
>     -boolean isBrewing
>     -float water
>     -String brand
>     -MilkContainer milkContainer
>     +serveCoffee() void
>   }
>   CoffeeMachine --> MilkContainer : has-a
> ```
> ```java
> public class CoffeeMachine {   // class = blueprint
>     private String brand;      // field / attribute
>     public void serveCoffee() {}   // method / behaviour
> }
> // Main.java
> CoffeeMachine nespresso = new CoffeeMachine();  // object = instance
> ```
> 💡 **Exam Pitfall:** **`-` = private, `+` = public in a classDiagram** ➔ fields are usually `private` (hidden), methods `public` (the interface) — the basis of information hiding.

> [!NOTE] **Crossover Invariant:** the class file name **must** match the class name ([[Java Program Structure]]); each object gets its own copy of the fields, so two `CoffeeMachine`s can hold different `brand` values while sharing the one `serveCoffee()` behaviour.

## 🧠 Active Recall
> [!FAQ]- Distinguish class, object, field, and method with the coffee-machine example.
> > [!SUCCESS]- Answer
> > - **Direct Criterion:** Class = the `CoffeeMachine` blueprint; object = a specific `new CoffeeMachine()` instance; field/attribute = its data (`brand`, `water`); method/behaviour = an action (`serveCoffee()`).
> > - **Technical Justification:** **Blueprint vs instance** ➔ the class defines structure once; each object instantiates it with its own field values.

> [!FAQ]- Why can a class's field be another class type (e.g. `MilkContainer`)?
> > [!SUCCESS]- Answer
> > - **Direct Criterion:** Fields hold data of any type, including references to other objects, so a `CoffeeMachine` can *have-a* `MilkContainer` as an attribute.
> > - **Technical Justification:** **Composition** ➔ objects are built from other objects; this "has-a" link is the seed of the [[Client-Supplier Relationship (Java)|client–supplier relationship]].
