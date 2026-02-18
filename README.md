# 🎱 Roll-a-Ball

A 3D ball-rolling game built in Unity as a learning project. The player controls a ball using keyboard or gamepad input, rolling around a level to collect pick-ups while a camera smoothly follows the action.

---

## 🎮 Gameplay

- Roll the ball using keyboard (WASD or arrow keys) or a gamepad
- Collect pick-up objects scattered around the level
- A counter tracks how many pick-ups you have collected
- Boost objects are placed around the level (boost mechanic in development)

---

## 📁 Project Structure

```
Assets/
├── Scripts/
│   ├── PlayerController.cs   # Player movement, pick-up collection, score tracking
│   ├── CameraController.cs   # Smooth camera follow
│   ├── Rotator.cs            # Makes pick-up objects spin
│   └── boost.cs              # Boost mechanic (in development)
├── Scenes/                   # Game scenes
├── Materials/                # Visual materials
├── Prefabs/                  # Reusable game objects
└── TextMesh Pro/             # UI text rendering
```

---

## 🧩 Scripts Overview

### PlayerController.cs
Handles everything related to the player ball:
- Reads movement input using Unity's new Input System
- Applies physics-based force to the Rigidbody for smooth rolling
- Detects collisions with pick-up and boost objects using trigger detection
- Updates the on-screen pick-up counter using TextMesh Pro

### CameraController.cs
Keeps the camera locked behind the player:
- Calculates the offset between the camera and player at game start
- Maintains that offset every frame so the camera follows smoothly without snapping

### Rotator.cs
Makes collectible pick-up objects spin in place:
- Rotates objects on all three axes every frame
- Uses `Time.deltaTime` to keep rotation speed consistent regardless of frame rate

### boost.cs
Placeholder script for a boost mechanic currently in development.

---

## 🛠️ Built With

- [Unity](https://unity.com/) — Game engine
- C# — Scripting language
- Unity Input System — Controller and keyboard input
- TextMesh Pro — UI text rendering
- Universal Render Pipeline (URP) — Rendering

---

## 🚀 Getting Started

1. Clone this repository:
   ```bash
   git clone https://github.com/JehosaphatsTuff/Test-Area.git
   ```
2. Open the project in Unity (Unity 6 or later recommended)
3. Open the scene in `Assets/Scenes/`
4. Press **Play** to run the game

---

## 🗺️ Roadmap

- [ ] Complete boost mechanic
- [ ] Add win condition when all pick-ups are collected
- [ ] Add a timer
- [ ] Add sound effects
- [ ] Build and export for Windows

---

## 👤 Author

**JehosaphatsTuff**  
[GitHub Profile](https://github.com/JehosaphatsTuff)
