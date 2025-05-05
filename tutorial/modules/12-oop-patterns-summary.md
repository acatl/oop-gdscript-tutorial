# Module 12: OOP Patterns Recap & Resources 🧠

**Hash ID**: `mod12-bfa8b9d2`

## Overview

In this module, we’ll review the **object-oriented design patterns** introduced across the Tiny Town RPG tutorial. These patterns aren’t just fancy words—they’re powerful tools that make your code easier to expand, debug, and reuse. You'll also find links to reliable resources to go deeper.

---

## Patterns You’ve Already Used

### 🧠 State Pattern

**Used In**: Module 8 – Basic AI System
**Why It Matters**: Helps model complex behavior by giving each state (like patrol, idle, chase) its own logic. Keeps code organized and makes it easy to add or change behavior.

🔗 [Wikipedia: State Pattern](https://en.wikipedia.org/wiki/State_pattern)

---

### 🎯 Strategy Pattern

**Used In**: Module 8 (optional stretch goal)
**Why It Matters**: Let different enemies use different movement or combat strategies without rewriting the whole AI. You pick the behavior at runtime.

🔗 [Wikipedia: Strategy Pattern](https://en.wikipedia.org/wiki/Strategy_pattern)

---

### 🧩 Component Pattern

**Used In**: Module 9 – Inventory and Items (optional stretch goal)
**Why It Matters**: Lets you compose object behavior from small reusable parts (like `HealEffect` or `UnlockDoorEffect`) instead of relying on deep inheritance trees.

🔗 [Wikipedia: Component-based software engineering](https://en.wikipedia.org/wiki/Component-based_software_engineering)

---

### 📣 Observer Pattern (Signals)

**Used In**: Module 4, 6, 7, and more
**Why It Matters**: Signals allow parts of your game to communicate without being tightly coupled. Great for clean, modular designs. It’s the secret sauce behind UI updates, quest events, and more.

🔗 [Wikipedia: Observer Pattern](https://en.wikipedia.org/wiki/Observer_pattern)

---

### 🏭 Factory Pattern

**Used In**: Module 10 – Saving and Loading
**Why It Matters**: Centralizes object creation. Useful when restoring objects (like items) from saved data or building content dynamically.

🔗 [Wikipedia: Factory Pattern](https://en.wikipedia.org/wiki/Factory_method_pattern)

---

### 🌐 Singleton Pattern

**Used In**: Modules 6 and 10 (LevelManager, SaveManager)
**Why It Matters**: Makes a class globally accessible—great for saving, loading, or tracking game state. Should be used sparingly and responsibly!

🔗 [Wikipedia: Singleton Pattern](https://en.wikipedia.org/wiki/Singleton_pattern)

---

## What's Next?

Here are some additional OOP design patterns that are useful for more advanced game architecture. You won't need them just yet—but keep them on your radar as your projects grow:

### 🔀 Command Pattern

**Use Case**: Encapsulate actions like "attack", "cast spell", or "undo move" as objects. Great for turn-based games or redo systems.
🔗 [Wikipedia: Command Pattern](https://en.wikipedia.org/wiki/Command_pattern)

### 🏛️ MVC (Model-View-Controller)

**Use Case**: Separate game logic (Model), UI (View), and control input (Controller). Great for UI-heavy games.
🔗 [Wikipedia: Model–View–Controller](https://en.wikipedia.org/wiki/Model–view–controller)

### 🧪 Prototype Pattern

**Use Case**: Quickly clone objects like enemies or bullets with the same properties. Can be paired with object pooling.
🔗 [Wikipedia: Prototype Pattern](https://en.wikipedia.org/wiki/Prototype_pattern)

### ♻️ Decorator Pattern

**Use Case**: Add new behavior to objects without changing their structure. Great for items that modify player or spell behavior.
🔗 [Wikipedia: Decorator Pattern](https://en.wikipedia.org/wiki/Decorator_pattern)

### 🔁 Chain of Responsibility

**Use Case**: Pass a request through a chain of handlers. Useful for building dialogue systems, AI decision pipelines, or event resolution.
🔗 [Wikipedia: Chain-of-responsibility Pattern](https://en.wikipedia.org/wiki/Chain-of-responsibility_pattern)

---

These patterns are your **game dev toolkit**. They help you:

- Keep code clean and modular
- Avoid repetition
- Add new features without breaking old ones
- Think like a software architect 💼

Keep these in mind as you expand your Tiny Town RPG or build something entirely new!
