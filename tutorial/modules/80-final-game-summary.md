# 🕹️ Final Game: “Tiny Town RPG”

## 🎯 Core Concept

A top-down, single-screen RPG where a player explores a small village, talks to quirky NPCs, fights off basic enemies, and levels up. The game acts as a **sandbox for learning OOP**, not a massive open-world adventure.

---

## 🧩 Core Features (at completion)

### 🧍‍♂️ Player Character

- Created from a `Player.gd` class (inherits from `Character.gd`)
- Has:

  - A name
  - HP (health bar UI)
  - Basic actions: `take_damage()`, `heal()`, and `level_up()`

### 🏘️ Villagers (NPCs)

- Instanced from a `Villager.tscn` scene using export variables
- Each has:

  - A name
  - A unique dialogue line
  - (Optionally) basic idle animations or triggered speech

### 👹 Enemies

- Inherited from a shared `Character.gd` base class
- Types like `Goblin` and `Orc`, each with different stats or behaviors
- Can:

  - Take damage and die
  - Be instanced manually or spawned dynamically

### ⚔️ Combat

- A shared `CombatManager` (or combat logic function) handles simple battles
- The player and enemy take turns dealing damage using shared method calls
- No turn-based system—just simple script-driven interactions

### 💬 Signals

- Signals used for:

  - Notifying when an enemy is defeated
  - Alerting UI to update XP or progress
  - Triggering dialogue popups

### 📦 Composition

- Optional reusable components like:

  - `HealthComponent`
  - `DialogueComponent`
  - `InventoryComponent` (basic)

- Demonstrates "composition over inheritance" in select areas

### 🧼 Clean Code Integration

- Code is refactored throughout with Clean Code principles:

  - Meaningful naming
  - SRP (Single Responsibility)
  - Reusability and clarity
  - No overengineering

### 🎯 Challenges & Stretch Goals

- Add a `QuestGiver` NPC with a simple quest (“Defeat 3 goblins”)
- Add an `XP` and `leveling` system with feedback
- Add `defend()` or `special()` actions to certain classes

---

## 📊 What This Game _Isn’t_ (on purpose)

- Not an inventory or crafting sim
- No save/load system
- Not a full RPG system with branching quests
- No large overworld or dungeon system
- No pathfinding or complex AI (basic movement only if any)

---

### 🧠 What Students Learn

By the end, students will understand:

- How OOP works in a game engine (using Godot 4.x)
- How to write, reuse, and refactor classes
- How to use inheritance and composition together
- How to use signals to connect game logic
- How to keep code clean and clear from the start
