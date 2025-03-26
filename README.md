# Space Invaders

Welcome to the documentation for my Space Invaders. This project is a custom-engineered remake of the classic **Space Invaders**, implemented using a real-time game engine (Azul.Engine) and built entirely in C#.

> ✨ **157 total classes** |
> 🔄 **Data-driven architecture** |
> 💡 **10+ software design patterns used**

---

## 🌌 Project Summary

This project is a modern, performance-optimized clone of the classic arcade game *Space Invaders*. Built with architectural precision and game design in mind, the system handles:

- Multiple alien types (Squid, Crab, Octopus)
- Player-controlled ship with missile firing
- 3 types of bombs with dynamic movement
- Shields with erosion mechanics
- Animated UFOs with scoring logic
- Real-time collision handling and object pooling
- Scene and state management (Start, Play, Game Over)
- Level progression system with increasing difficulty

---

## 🔧 Technologies Used
- **Language:** C#
- **Game Engine:** Custom framework based on Azul.Engine
- **Design Patterns:** Factory, Observer, Proxy, Command, Composite, Strategy, Visitor, State, Iterator, Object Pooling

---

## 🖋️ Architectural Highlights
- **Data-Driven Architecture:** Enables scalable, modular development
- **Custom Timer & Command System:** Allows scheduled real-time actions (animations, alien movement, etc.)
- **Composite Pattern for GameObject Trees:** Used for alien grids, shields, and collision trees
- **State Pattern:** Controls transitions between menus, gameplay, and end states

---

## 🎮 Gameplay Features
- 3 alien types with unique point values (10, 20, 30)
- 3 bomb types with unique fall behavior (Zigzag, Rolling, Dagger)
- 4 destructible shields
- Missile and bomb collision interactions
- UFO appears at random intervals with sound and scoring
- Lives and scoring system
- Game loop with escalating difficulty and round progression

---

## 📃 Documentation Files
- `PROJECT_OVERVIEW.md` - Detailed overview of the game architecture
- `DESIGN_PATTERNS.md` - Deep dive into design pattern usage

---

## 🚫 Disclaimer
Due to copyright restrictions, **the source code cannot be shared publicly**. This repository focuses on documenting the architecture and design for educational and portfolio purposes.

---

## 👨‍💼 Author
**Aryan Patel**

