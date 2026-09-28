# ⚔️ Lumina Adventure
![Alt text](assets/kingdom.png)
**A terminal-based RPG powered by Node.js and Express.**

Lumina Adventure is an experimental role-playing game where HTTP requests become player commands. Instead of controlling the game through a traditional graphical interface, players explore the world, fight enemies, interact with characters, and progress through the adventure directly from the terminal.

The project was originally built as a learning exercise to explore **server-side JavaScript, application logic, routing, state management, and interactive systems**.

---

## 🎮 The Concept

You have been summoned to protect the **Kingdom of Lumina**.

Fight monsters, help villagers, explore the world, and grow strong enough to challenge the tyrant threatening the kingdom.

The unusual part?

**Your terminal is the game controller.**

```bash
curl localhost:4000/w
```

Every HTTP request represents an action inside the game.

```text
Terminal Command
      ↓
Express Route
      ↓
Game Logic
      ↓
Player / World State
      ↓
Game Response
```

---

## 🧠 What This Project Demonstrates

Lumina Adventure explores several software-development concepts through a simple RPG:

- Node.js server-side development
- Express routing
- HTTP-based interactions
- Application and player state
- Coordinate-based world navigation
- Combat systems
- NPC interactions
- Events and quests
- Inventory and rewards
- Conditional game logic

Although this is an early learning project, it helped develop the systems-thinking and programming fundamentals that I later applied to larger automation and application-development work.

---

## 🛠️ Technology

- **JavaScript**
- **Node.js**
- **Express**
- **REST-style HTTP routing**
- **cURL** for player interaction

---

## 🚀 Getting Started

### Requirements

Make sure you have installed:

- Node.js
- npm
- Git
- A terminal or command prompt

### 1. Clone the repository

```bash
git clone https://github.com/romellbermundo/lumina-adventure.git
cd lumina-adventure
```

### 2. Install dependencies

```bash
npm install
```

### 3. Start the server

```bash
npm start
```

The game server runs locally on:

```text
localhost:4000
```

### 4. Start the adventure

Open another terminal and enter:

```bash
curl localhost:4000/
```

Welcome to Lumina.

---

## 🗺️ How to Play

Actions are performed by sending requests to the game server.

### Movement

```bash
curl localhost:4000/w
```

Move north.

```bash
curl localhost:4000/s
```

Move south.

```bash
curl localhost:4000/a
```

Move west.

```bash
curl localhost:4000/d
```

Move east.

### Observe

Inspect your current location:

```bash
curl localhost:4000/o
```

Exploration is important. Observe new locations to discover enemies, characters, events, and other interactions.

### Location

Check your current position:

```bash
curl localhost:4000/location
```

### Combat

Attack an enemy:

```bash
curl localhost:4000/attack
```

Additional commands and interactions can be discovered as you explore the game.

---

## 🧩 Game Systems

Lumina Adventure includes several interconnected systems:

**World Exploration**  
Navigate through a coordinate-based game world.

**Combat**  
Encounter and fight enemies as you explore.

**NPC Interaction**  
Meet characters and interact with them through game commands.

**Events & Quests**  
Trigger events and progress through different encounters.

**Player Progression**  
Manage player status, healing, rewards, and other gameplay mechanics.

The goal of the project was to experiment with how these systems could interact through a simple server-side architecture.

---

## 🏗️ Architecture

The current version uses a deliberately simple architecture centered around an Express server.

```text
PLAYER
  │
  │ HTTP / cURL
  ▼
EXPRESS ROUTES
  │
  ▼
GAME LOGIC
  │
  ├── Movement
  ├── Combat
  ├── NPCs
  ├── Events
  ├── Items
  └── Player State
  │
  ▼
GAME RESPONSE
```

A future version could separate these systems into individual modules and introduce persistent game state, automated testing, and a dedicated user interface.

---

## 💡 Lessons From the Project

Lumina Adventure started as a programming exercise, but it introduced several concepts that became important in my later development work:

- breaking a larger problem into smaller systems
- translating user actions into application logic
- managing interactions between different pieces of state
- designing repeatable program behavior
- thinking beyond individual functions toward complete workflows

Those same principles now influence how I approach **GIS development, systems automation, and geospatial workflows**.

---

## 🔮 Possible Future Improvements

If the project is revisited, potential improvements include:

- modularizing the game engine
- separating routes from game logic
- persistent player state
- automated tests
- improved error handling
- a browser-based interface
- API documentation
- Docker containerization
- cloud deployment

The original implementation is intentionally preserved as an example of an earlier stage in my software-development journey.

---

## 👨‍💻 About the Developer

I'm **Romell Bermundo**, a GIS Developer focused on **systems automation, geospatial development, and practical software solutions**.

My professional work focuses on turning complex and repetitive processes into reliable systems using technologies such as Python, ArcPy, FME, SQL, and enterprise GIS.

Lumina Adventure represents an earlier part of that journey: learning how to turn rules, state, and user actions into a working software system.
