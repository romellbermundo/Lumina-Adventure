# ⚔️ Lumina Adventure
![Alt text](assets/kingdom.png)


**A terminal-based role-playing adventure powered by Node.js and Express.**

Fight monsters, explore the Kingdom of Lumina, help its villagers, grow stronger, and challenge the tyrant king.

Instead of using a traditional graphical interface, **your terminal is the controller**. Player commands are sent to the game server through HTTP requests.

---

## 📑 Table of Contents

- [About the Game](#-about-the-game)
- [The Story](#-the-story)
- [How It Works](#️-how-it-works)
- [Features](#-features)
- [Technology](#️-technology)
- [Installation](#-installation)
- [How to Play](#️-how-to-play)
- [Commands](#️-commands)
- [Gameplay Tips](#-gameplay-tips)

---

## 🎮 About the Game

**Lumina Adventure** is a terminal-based RPG where the player explores a coordinate-based world by sending commands to a Node.js and Express server.

Instead of clicking buttons or controlling a character with a keyboard, actions are performed through HTTP requests.

For example:

```bash
curl localhost:4000/w
```

sends your character north.

The server processes the command, updates the game state, and responds with what happens next.

Explore the world, encounter enemies, interact with characters, collect items, and discover the Kingdom of Lumina through the terminal.

---

## 📖 The Story

> **Oracle:** You have been summoned to protect the Kingdom of Lumina, but you must first prove yourself worthy of the power of the Hero.
>
> Go forth, Hero. And may the Great Spirit be with you.

You open your eyes and find yourself transported to the **Tutorial Area**.

Your journey begins here.

Learn how to move through the world, survive your first battles, and discover why you have been summoned to Lumina.

Your ultimate goal:

**Protect the villagers and save the kingdom from the tyrant king.**

---

## ⚙️ How It Works

Lumina Adventure turns HTTP requests into RPG commands.

```text
PLAYER
  │
  │  curl localhost:4000/w
  ▼
EXPRESS SERVER
  │
  ▼
COMMAND PROCESSING
  │
  ├── Movement
  ├── Combat
  ├── Observation
  ├── Interaction
  └── Items
  │
  ▼
GAME STATE
  │
  ├── Player
  ├── Location
  ├── Enemies
  ├── NPCs
  └── Events
  │
  ▼
TERMINAL RESPONSE
```

The Express server acts as both the **game engine** and the interface between the player and the world.

Each route represents an action the player can perform.

---

## ✨ Features

### 🗺️ World Exploration

Move through a coordinate-based world and discover different locations throughout Lumina.

### ⚔️ Combat

Encounter enemies and attack them using terminal commands.

### 👥 Characters

Meet NPCs throughout the kingdom and interact with them as you explore.

### 🎒 Items & Rewards

Discover items and rewards during your adventure.

### 📜 Events & Quests

Explore the world to uncover encounters and objectives.

### ❤️ Player Status

Check
