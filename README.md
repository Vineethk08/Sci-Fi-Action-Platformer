# Sci-Fi Action Platformer

A side-scrolling action platformer prototype built in **Defold 1.12.2** using the Void Docking Facility asset pack.

## 🎮 Gameplay

The goal of this prototype is to test a fully animated player character that can move, jump, aim at the cursor, and shoot blast projectiles in any direction.

- **Move**: A / D or Arrow Keys
- **Jump**: Spacebar (no double jump)
- **Aim**: Move the mouse cursor — aim snaps to nearest 45 degrees
- **Shoot**: Left mouse click

## ✨ Features

- Fully animated player with run, stand, and jump states
- Left and right facing animations (not flipped — separate sprite sets)
- 45-degree cursor aiming with backward aim clamping
- Blast projectile spawns from the gun tip, travels in aim direction, rotates to face direction
- Blast despawns on wall collision or going offscreen
- Tile-based level with floating platform and two floor heights
- Player fully enclosed — cannot walk or fall out of level
- Black background level aesthetic

## 🗂️ Project Structure

```
Sci-Fi_Action_Platformer/
├── input/
│   └── game.input_binding
├── main/
│   ├── images/
│   │   ├── player/         # All player sprites
│   │   ├── projectiles/    # Blaster sprites
│   │   └── tilesource/     # Level tileset
│   ├── level/
│   │   └── level.tilemap
│   ├── player/
│   │   ├── player.atlas    # 30 animation groups
│   │   ├── player.go
│   │   └── player.script
│   ├── projectiles/
│   │   ├── blast.atlas
│   │   ├── blast.go
│   │   └── blast.script
│   └── main.collection
└── game.project
```

## 🎨 Assets

Assets from the **Void Asset Pack: Docking Facility** (free section of itch.io).

## 🛠️ Built With

- [Defold](https://defold.com/) — Game Engine
- Lua — Scripting language

## 🚀 How to Run

1. Download and install [Defold](https://defold.com/download/)
2. Open Defold and select **Open Project**
3. Navigate to this folder and open `game.project`
4. Press **Cmd+B** (Mac) or **Ctrl+B** (Windows) to build and run

## 📝 Notes

- This is a prototype — no win/lose states
- Camera follow is not implemented in this version
- Developed as part of a Feather employee task
