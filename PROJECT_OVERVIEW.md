# Project Overview - Space Invaders 

## 🌍 Introduction
This project is a real-time game system inspired by the original *Space Invaders* arcade game. The project was built in **C#** using a performance-focused, custom game engine called **Azul.Engine**. The primary objective was to showcase modular game architecture, advanced object-oriented design, and effective use of real-time constraints.

---

## 🎮 Game Description
In this game, the player controls a spaceship that can move horizontally across the bottom of the screen and fire missiles upward to destroy waves of alien invaders.

### Core Gameplay Features:
- Horizontal ship movement with spacebar firing
- Three alien types: Squid (10 pts), Crab (20 pts), Octopus (30 pts)
- Aliens arranged in a **5x11 grid** (total 55 aliens per round)
- Increasing speed as aliens are eliminated
- Randomly spawning **UFO** with sound and score bonus
- Dynamic **bomb dropping** behavior with three movement types (Zigzag, Rolling, Dagger)
- **Four destructible shields** protecting the player
- Lives tracking, scoring, and multiple rounds

---

## 🔄 Architecture & Design
This project is a showcase of clean architecture principles in a real-time system. Key focuses:

### ✅ Data-Driven Engine
- Entities and behaviors are controlled via managers and events
- Object creation and animation logic are modular and extendable

### ⚙️ Game Flow Management
- Three separate game scenes: `SelectScene`, `PlayScene`, `GameOverScene`
- Managed via State pattern and centralized `SceneContext`

### 🪡 Real-Time Command Queue
- Global `TimerManager` processes time-based commands using a sorted priority queue
- Avoids clutter in the main game loop and enables precise scheduling

---

## 📈 System Stats
- **157 custom C# classes**
- **Multiple GameObject trees** using Composite pattern
- Fully encapsulated collision detection system using Visitor pattern
- Score system integrated with game objects and collision observers
- Sprite optimization via Proxy pattern (shared RealSprites across lightweight proxies)
- Timed actions (alien march, animation, missile launch) handled with Command pattern

---

## 🚀 Engine Components
- **GameObjectManager** - Handles all update/draw logic for game entities
- **SpriteBatchManager** - Renders sprites using shared RealSprites
- **CollisionPairManager** - Tracks all collision pairs and applies responses
- **TimerManager** - Runs scheduled events using time-stamped command objects
- **SceneContext** - Central controller managing game states
- **UFORoot, AlienGrid, ShieldFactory** - Custom factories and composites for creating game object groups

---

## 🏋️ Design Philosophy
- Use of **design patterns** to keep logic decoupled and extendable
- Clean **separation of concerns** for rendering, input, game rules, and object lifecycle
- Performance and memory optimization via **object pooling** and **proxy rendering**
- Scalability through reusable architecture for multiple levels and game rounds

---

## 📖 Documentation Breakdown
This GitHub repository includes:
- `README.md` - Project summary and highlights
- `PROJECT_OVERVIEW.md` - This file
- `DESIGN_PATTERNS.md` - Explanation of each pattern used and its purpose
- `FEATURES.md` - Detailed list of gameplay and technical features
- `VIDEO_DEMO.md` - Demo video link and walkthrough

---

## 📅 Timeline & Submission
- Course: SE 456 - Architecture of Real-Time Systems
- Term: Winter 2025
- Instructor: Edward Keenan
- Submission Date: March 24, 2025
- YouTube Demo: [https://youtu.be/zfRrIUzsXG8](https://youtu.be/zfRrIUzsXG8)

---

## 🚫 Copyright
This repository **does not** contain source code due to university policies. It focuses solely on architectural documentation, design explanation, and gameplay behavior showcase for educational and portfolio purposes.
