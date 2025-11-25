# Space Invaders - JavaScript Edition

![Space Invaders Gameplay](image2.png)  
*A classic arcade shooter recreated from scratch using vanilla JavaScript! Defend Earth from waves of alien invaders.*

**Space Invaders** is a fully functional clone of the iconic 1978 arcade game, built entirely with **HTML5**, **CSS3**, and **vanilla JavaScript** (no frameworks or libraries like Phaser or Three.js). It features smooth animations, collision detection, sound effects, and escalating difficulty—perfect for learning game development fundamentals.

Play it live by opening `index.html` in your browser!

## 🚀 Quick Start

1. **Clone the Repo**:
   ```bash
   git clone https://github.com/sksohel27/Space-Invader.git
   cd Space-Invader
   ```

2. **Run the Game**:
   - No installation required! Simply open `index.html` in any modern browser (Chrome, Firefox, Edge).
   - For the best experience, use fullscreen mode (F11).

## 🎮 How to Play

- **Move**: Left/Right arrow keys (or A/D keys).
- **Shoot**: Spacebar.
- **Objective**: Destroy all alien invaders before they reach the bottom or shoot you down.
- **Lives**: You have 3 lives—lose them all, and it's game over!
- **Scoring**: Higher waves = more points. Aliens speed up as you progress.

Sound effects include laser shots (`shoot.wav`) and explosions (`enemy-death.wav`).

## 🛠️ Technology Stack

This project is built with pure web technologies for a lightweight, dependency-free experience:

| Category       | Technologies                  | Purpose |
|----------------|-------------------------------|---------|
| **Markup**     | HTML5                        | Game structure, canvas integration, and audio elements |
| **Styling**    | CSS3                         | Positioning, animations (e.g., enemy movement), and responsive layout |
| **Logic**      | JavaScript (ES6+)            | Core game engine: Object-oriented controllers, event handling, collision detection, and game loop (via `requestAnimationFrame`) |
| **Assets**     | PNG images, WAV audio        | Sprites for player (`spaceship.png`), enemies (`invader.png`), bullets, and background |

- **Key JS Patterns**: Modular classes (`Player.js`, `Enemy.js`, `Bullet.js`, `EnemyController.js`, `BulletController.js`) for separation of concerns.
- **Game Loop**: Efficient 60 FPS rendering with `requestAnimationFrame`.
- **No External Dependencies**: 100% vanilla—runs anywhere without npm or build tools.

## 📁 Project Structure

```
Space-Invader/
├── .gitignore              # Ignores unnecessary files
├── Bullet.js               # Bullet logic and rendering
├── BulletController.js     # Manages bullet arrays and collisions
├── Enemy.js                # Individual enemy behavior
├── EnemyController.js      # Spawns and controls enemy waves
├── MovingDirection.js      # Enum for enemy movement directions
├── Player.js               # Player ship controls and shooting
├── index.html              # Entry point: Canvas setup and game initialization
├── index.js                # Main game loop and orchestration
├── README.md               # Project docs
├── enemy-death.wav         # Explosion sound
├── shoot.wav               # Laser sound
├── image2.png              # Gameplay screenshot
├── image3.jpg              # Alternative screenshot
├── invader.png             # Enemy sprite
├── photo-1445905595283-21f8c... # Background nebula image
├── spacecraft.png          # Player ship sprite
└── spaceship.png           # Alternate player sprite
```

## 🧠 Development Insights

- **Collision Detection**: Axis-aligned bounding box (AABB) checks for bullets, enemies, and player.
- **Enemy Waves**: Enemies move in a grid, descending and reversing direction on edge hits.
- **Performance**: Canvas 2D context for fast drawing; objects are reused/recycled to minimize GC.
- **Extensibility**: Easy to add power-ups, bosses, or multiplayer by extending controllers.

This project was built as a learning exercise in vanilla JS game dev—total code ~500 lines!

## 🔧 Contributing

Contributions welcome! Fork the repo, add features (e.g., high-score persistence with localStorage), and submit a PR.

- Follow ES6+ standards.
- Test in multiple browsers.
- Update screenshots if UI changes.

## ⚠️ Known Issues

- Audio may not autoplay on mobile (browser policy)—tap to enable.
- No mobile touch controls yet (desktop-focused).

---

*Last updated: November 2024*
