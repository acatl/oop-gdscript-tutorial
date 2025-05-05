# Module 13: Next Steps & Expansions 🚀

**Hash ID**: `mod13-0ae97cb1`

## Overview

Congratulations, hero! You’ve completed the core Tiny Town RPG tutorial—and now the _real_ adventure begins.

This module provides optional feature ideas, framed as Agile-style **user stories**, so you can continue practicing object-oriented design while leveling up your coding skills.

---

## 🧠 Why User Stories?

User stories describe what a player (or developer) wants to do and why. They help break big ideas into manageable goals.

> ✨ Example Format:
> **As a player**, I want to \[do something] so that \[I get this benefit].

---

## 🌱 Foundational Expansions

### 🎯 Add More Enemy Types

**As a player**, I want to fight different enemies so that each battle feels unique.

- Add `Goblin`, `Skeleton`, or `Mage` scenes that inherit from `Enemy.gd`
- Give each unique stats or abilities

### 💬 Dialogue Choices

**As a player**, I want to choose how I respond to villagers so that I feel more in control.

- Add a `DialogueManager.gd` that handles conversation trees
- Use buttons to present options and consequences

### 🔓 Unlockable Areas

**As a player**, I want to collect keys to open new areas so that I feel rewarded for exploring.

- Add locked doors that check for items in the inventory
- Connect to the item system you built in Module 9

### 📜 More Complex Quests

**As a player**, I want quests that have multiple steps so that they feel more like a story.

- Add a `QuestStage.gd` component
- Use signals to trigger stage progress

---

## 💎 Polishing Ideas

### 🎨 Add Character Portraits

**As a player**, I want to see who I’m talking to so that the game feels more alive.

### 🎵 Add Music and SFX

**As a player**, I want the game to sound fun and dramatic so that I’m more immersed.

### 🕹 Gamepad Support

**As a player**, I want to play with a controller so that I can chill on the couch.

### 🧙 Class System

**As a player**, I want to choose a class (like mage or knight) so that I can customize how I play.

- Add subclasses of `Player.gd` with special abilities
- Use the Strategy Pattern to manage skills

---

## 🧱 Bigger Systems to Try

- **Turn-Based Combat System**
- **Shop System with Currency**
- **Crafting System**
- **Achievements or Trophy Room**
- **Minimap or World Map**
- **Skill Trees**

---

## 🗂 Bonus: Organize Your Ideas

Use a lightweight Agile board or kanban system:

- `To Do`: Feature ideas
- `Doing`: What you’re building now
- `Done`: Victory!

Try tools like Trello, Notion, or a simple notebook.

---

## Final Words 💬

You’ve built a fully functioning game using real software architecture practices. Keep pushing forward. Learn by making. And always keep your hero’s backpack clean.

> 🏁 _Now go forth and code the next legend!_
