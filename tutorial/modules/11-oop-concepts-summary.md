# Module 11: OOP Concepts Recap & Resources 🧩&#x20;

**Hash ID**: `mod11-c0d7fb1b`

## Overview

Object-Oriented Programming (OOP) is the backbone of Tiny Town RPG. In this module, we’ll look back at the core OOP **concepts** you've practiced throughout the tutorial—what they mean, why they matter, and how they improve your game.

We'll also give you some solid references to explore each concept further.

---

## Core Concepts You’ve Practiced

### 🧱 Classes & Objects

**Used In**: All modules
**Why It Matters**: A class defines the blueprint, and an object is the thing built from it. It’s how your `Player`, `Enemy`, and `Quest` come to life.

🔗 [Wikipedia: Class (computer programming)](https://en.wikipedia.org/wiki/Class_%28computer_programming%29)

---

### 🧠 Encapsulation

**Used In**: Modules 1, 5, 6
**Why It Matters**: Keeps related data and behavior inside the same unit. Protects complexity and avoids exposing too much of how something works.

🔗 [Wikipedia: Encapsulation (computer programming)](https://en.wikipedia.org/wiki/Encapsulation_%28computer_programming%29)

---

### 🔁 Inheritance

**Used In**: Module 3 – Battle Mechanics
**Why It Matters**: Allows new classes to reuse behavior from a base class (like `Character.gd`). Reduces duplication and makes it easy to extend functionality.

🔗 [Wikipedia: Inheritance (object-oriented programming)](https://en.wikipedia.org/wiki/Inheritance_%28object-oriented_programming%29)

---

### 🧬 Polymorphism

**Used In**: Module 3, 8 (implicitly through state switching and inherited behavior overrides in enemies)
**Why It Matters**: Different objects can respond to the same method name in their own way (e.g., `die()` work differently for enemies and players). Flexible, elegant code!

🔗 [Wikipedia: Polymorphism (computer science)](https://en.wikipedia.org/wiki/Polymorphism_%28computer_science%29)

---

### 🧩 Composition

**Used In**: Modules 6, 7, 9
**Why It Matters**: Build complex behavior by assembling small parts instead of deep inheritance chains. You saw this with components like `Quest`, `LevelComponent`, and `HealEffect`.

🔗 [Wikipedia: Composition over inheritance](https://en.wikipedia.org/wiki/Composition_over_inheritance)

---

### 📬 Messaging & Decoupling

**Used In**: Module 4 – Signals
**Why It Matters**: Loose coupling between objects makes your code more flexible and modular. Signals help different parts of your game react without knowing about each other.

🔗 [Wikipedia: Loose coupling](https://en.wikipedia.org/wiki/Loose_coupling)

---

## What's Next?

Here are some foundational OOP concepts worth exploring next:

### 🧼 SOLID Principles

These five foundational principles help you write more maintainable, scalable, and flexible code—especially in larger projects or collaborative teams. They’re widely used in software architecture and also apply directly to game development, especially when your project starts to grow.

Learn the five design principles that help make software more maintainable:

- **S**ingle Responsibility
- **O**pen/Closed
- **L**iskov Substitution
- **I**nterface Segregation
- **D**ependency Inversion

🔗 [Wikipedia: SOLID](https://en.wikipedia.org/wiki/SOLID)

### 🧪 Abstraction

A key idea that’s behind _everything_ in OOP. Focus on what an object does, not how it does it.

🔗 [Wikipedia: Abstraction (computer science)](https://en.wikipedia.org/wiki/Abstraction_%28computer_science%29)

---

## Takeaway

You’re not just writing GDScript—you’re thinking like an object-oriented programmer! 💡

These core concepts are the reason your Tiny Town RPG is clean, modular, and ready to grow. Now that you’ve got the foundation, you’re equipped to build bigger and smarter games.
