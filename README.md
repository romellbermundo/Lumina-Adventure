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

Check your character's condition and progress while playing.

### 🧭 Observation

Inspect your current location to discover enemies, characters, and other important information.

---

## 🛠️ Technology

Lumina Adventure is built using:

- **JavaScript**
- **Node.js**
- **Express.js**
- **HTTP requests**
- **REST-style routes**
- **Git**
- **GitHub**

The project explores how a web server can be used for something very different from a traditional website: **running an interactive game.**

---

## 🚀 Installation

### Requirements

Make sure you have installed:

- Node.js
- npm
- Git

A terminal capable of running `curl` is also required.

### 1. Clone the repository

```bash
git clone https://github.com/romellbermundo/lumina-adventure.git
```

### 2. Enter the project directory

```bash
cd lumina-adventure
```

### 3. Install dependencies

```bash
npm install
```

### 4. Start the game server

```bash
npm start
```

The game server runs locally on:

```text
http://localhost:4000
```

### 5. Open another terminal

Start the adventure with:

```bash
curl localhost:4000/
```

Welcome to Lumina.

---

## 🕹️ How to Play

Every action in Lumina Adventure is performed by sending a request to the game server.

For example, if the game tells you:

```text
/w
```

enter:

```bash
curl localhost:4000/w
```

The server will process your action and tell you what happens.

### Movement

Move north:

```bash
curl localhost:4000/w
```

Move south:

```bash
curl localhost:4000/s
```

Move west:

```bash
curl localhost:4000/a
```

Move east:

```bash
curl localhost:4000/d
```

---

## ⌨️ Commands

### 🧭 Movement

| Action | Command |
|---|---|
| North | `/w` |
| South | `/s` |
| West | `/a` |
| East | `/d` |

Example:

```bash
curl localhost:4000/w
```

### 👀 Observe

Inspect your current location:

```text
/o
```

or:

```text
/observe
```

Example:

```bash
curl localhost:4000/o
```

**Tip:** Observe whenever you enter a new location.

### 📍 Location

Check your current position:

```text
/location
```

Example:

```bash
curl localhost:4000/location
```

### ⚔️ Attack

Attack an enemy:

```text
/k
```

or:

```text
/attack
```

Example:

```bash
curl localhost:4000/attack
```

There are more commands and interactions waiting inside the game.

**Part of the adventure is discovering them.**

---

## 💡 Gameplay Tips

### Use Your Command History

You don't need to type:

```bash
curl localhost:4000/
```

from scratch every time.

Press the **Up Arrow** in your terminal to bring back your previous command, then change the route.

For example:

```text
curl localhost:4000/w
                     ↑
              change only this
```

This makes exploring much faster.

### Observe Often

When entering a new location, use:

```bash
curl localhost:4000/o
```

The world may contain enemies, NPCs, events, or other things worth investigating.

### Explore

Not everything is explained immediately.

Experiment with commands, explore different locations, and discover how the world works.

> **For it is by fire that gold is made.**

---

## 🧙 A Little Secret

Since you actually read the README, here's a cheat code.

If you get lost, try:

```bash
curl localhost:4000/teleport
```

It will return you to your original location.

Use it wisely.

---

# ⚔️ Enter Lumina

The Oracle has summoned you.

The kingdom is waiting.

Start the server:

```bash
npm start
```

Open another terminal:

```bash
curl localhost:4000/
```

**Your adventure begins.**
Check
