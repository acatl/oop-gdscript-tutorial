# Module 5: Clean Up and Refactor 🧹

## Overview

You’ve added villagers, enemies, signals, and a hero with health problems. Your game’s becoming a real adventure! But wait—your code is starting to look like a backpack full of half-eaten snacks. It's time to **refactor** and apply **Clean Code principles** to keep things tidy and maintainable.

---

## Learning Objectives

- Understand what **refactoring** means
- Identify bad code smells like repetition and long functions
- Apply small, practical Clean Code improvements
- Make your code easier to read, reuse, and extend

---

## RPG Analogy: The Messy Backpack 🎒

> You can survive with a messy inventory, sure. But good luck finding that one health potion when you need it.
> **Refactoring** is like organizing your backpack—same items, but everything’s easier to use.

---

## What Is Refactoring? ♻️

Refactoring means **changing how your code is written** without changing what it does. It’s like giving your code a makeover without touching its brain.

Examples:

- Renaming vague variables (`a`, `thing`) to meaningful ones (`enemy_health`)
- Extracting big functions into smaller ones
- Moving duplicate logic into reusable methods or classes

---

## Step-by-Step Guide

### 1. Fix Naming 🏷️

Bad:

```gdscript
var a = 100
func do_it():
    b = a - 10
```

Better:

```gdscript
var max_health = 100
func take_damage():
    var new_health = max_health - 10
```

> 🦼 **Clean Code Tip**
> Code should read like a story. You shouldn’t need to play detective to understand what variables mean.

---

### 2. Use Helper Functions 🪛

If you find yourself repeating code across methods, make a helper function.

Before:

```gdscript
func heal():
    current_hp += 10
    $ProgressBar.value = current_hp
    $Label.text = player_name
```

After:

```gdscript
func heal():
    current_hp += 10
    update_ui()

func update_ui():
    $ProgressBar.value = current_hp
    $Label.text = player_name
```

> 🦼 **Clean Code Tip**
> Small functions are your best friends. They reduce bugs, increase reuse, and are easier to test.

---

### 3. Respect the Single Responsibility Principle (SRP) 📦

Each class should do **one thing well**.

Bad example: `Player.gd` handles movement, combat, UI, sound, and sandwich recipes.

Better:

- `Player.gd` → movement + stats
- `UIController.gd` → handles updating the HUD
- `AudioManager.gd` → plays sounds

> Split your logic across multiple small, focused scripts. Like a well-coordinated RPG party, each one has a role.

---

## Refactor Example 🧪

Before:

```gdscript
func _process(delta):
    if current_hp <= 0:
        queue_free()
    $Label.text = player_name
    $ProgressBar.value = current_hp
```

After:

```gdscript
func _process(delta):
    if current_hp <= 0:
        die()
    update_ui()

func update_ui():
    $Label.text = player_name
    $ProgressBar.value = current_hp
```

---

## Challenges ✅

- [ ] Find a method in your game longer than 5 lines and break it up
- [ ] Rename 3 variables to better describe what they do
- [ ] Move repeated logic into a shared function

---

## Stretch Goal 💡

Refactor your `Player` and `Enemy` classes to inherit from a shared `CombatCharacter` if you added combat logic to both.

Bonus: Create a `HealthComponent.gd` script and attach it to both if you want to explore composition instead of inheritance.

---

## Summary 🎓

Refactoring is how you turn spaghetti into clean, bite-sized noodles of awesome. You’ve now learned to name clearly, keep functions small, and respect boundaries between classes. Your game runs the same—but your future self will thank you.

Next up: let’s give our characters more depth by adding leveling, quests, and decision-making! 🌟
