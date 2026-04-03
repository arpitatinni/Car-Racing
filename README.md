# Car Racing Game

A 2D car racing game built with **Python** and **OpenGL (PyOpenGL)**, featuring real-time rendering, multiple difficulty levels, collision detection, and interactive gameplay mechanics — all drawn from scratch using OpenGL primitives.

---

## Preview

> Player controls a red car on a track, dodging oncoming enemy cars while trying to maximize score. A special golden car occasionally appears that can reduce your collision count.

---

## Features

- **Difficulty Selection Menu** — Choose between Easy, Medium, and Hard before starting
- **Player Car Movement** — Smooth WASD keyboard controls with boundary detection
- **Enemy Car Spawning** — Randomized enemy cars appear at the top of the track and move downward, zigzagging across the lane
- **Special Golden Car** — A rare golden car spawns periodically; successfully avoiding it reduces your collision count by 1
- **Collision Detection** — Tracks how many times the player collides with enemy cars; too many collisions ends the game
- **Score System** — Score increases each time an enemy car is successfully passed without collision
- **Pause / Resume** — Toggle pause mid-game using the on-screen button
- **Restart & Exit** — In-game control buttons (Restart, Pause/Play, Exit) drawn entirely with OpenGL primitives
- **Custom Rendering** — Cars, wheels, windshields, grass, and road are all rendered using `GL_POINTS` and mathematical geometry (no sprites or images)

---

## Controls

| Key | Action |
|-----|--------|
| `W` | Move car up |
| `S` | Move car down |
| `A` | Move car left |
| `D` | Move car right |
| `ESC` | Quit the game |
| Mouse Click | Select difficulty / Use control buttons |

---

## Difficulty Levels

| Level  | Car Speed | Spawn Rate | Enemy Speed | Max Collisions |
|--------|-----------|------------|-------------|----------------|
| Easy   | 3         | Every 45 frames | 1      | 7              |
| Medium | 5         | Every 30 frames | 2      | 5              |
| Hard   | 7         | Every 20 frames | 3      | 3              |

---

## Tech Stack

| Technology | Purpose |
|------------|---------|
| Python 3   | Core programming language |
| PyOpenGL   | Real-time 2D rendering via OpenGL |
| GLUT       | Window creation, input handling, game loop |
| `random`   | Randomized enemy spawning and positions |
| `math`     | Circular wheel rendering using trigonometry |

---

## Project Structure

```
Car-Racing/
│
└── 423 Project.py       # Main game file (all logic and rendering)
```

---

## Installation & Setup

### Prerequisites

Make sure you have Python 3 installed, then install the required library:

```bash
pip install PyOpenGL PyOpenGL_accelerate
```

> On some systems you may also need `freeglut`. Install it via:
> - **Linux:** `sudo apt-get install freeglut3-dev`
> - **Windows:** Download from [transmissionzero.co.uk](http://www.transmissionzero.co.uk/software/freeglut-devel/)
> - **macOS:** `brew install freeglut`

### Run the Game

```bash
python "423 Project.py"
```

## Author

**Arpita Ghosh**

---
