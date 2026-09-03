# DEPIXELER — Incremental Destruction Roguelite

[![GitHub Pages](https://img.shields.io/badge/Play%20Now-GitHub%20Pages-00e5ff?style=for-the-badge&logo=github)](https://allanroz.github.io/Depixeler/)
[![License: MIT](https://img.shields.io/badge/License-MIT-4a7fff?style=for-the-badge)](LICENSE)
[![Vanilla JS](https://img.shields.io/badge/Vanilla-JS%20%2F%20Canvas%202D-ffd700?style=for-the-badge&logo=javascript)](index.html)

> **Launch energy orbs into enormous pixel formations. Excavate ancient megastructures, trigger explosive chain reactions, and destroy the Golden Core.**

Play directly in your browser: **[https://allanroz.github.io/Depixeler/](https://allanroz.github.io/Depixeler/)**

---

## 🎮 Overview

**Depixeler** is an incremental destruction roguelite arcade game built entirely in Vanilla HTML5 Canvas and JavaScript. Fire volleys of specialized energy orbs into procedurally generated formations consisting of tens of thousands of individual pixels. Mine matter into Bits, craft custom synergies from random post-wave drafts, unlock permanent capabilities in a vast skill tree, and deploy automated turrets and excavation drones.

---

## ✨ Key Features

### 💥 Enormous Destructible Pixel Megastructures
- High-performance grid engine handling thousands of active pixels powered by chunk-cached flat typed arrays (`Uint8Array`, `Uint16Array`, `Uint32Array`).
- **7 Reactive Pixel Types**:
  - 🟦 **Normal (Blue)** — Standard structural matter.
  - 🟪 **Hard (Purple)** — Reinforced multi-hit resilient blocks.
  - 🔷 **Armored (Teal)** — Heavy defense lattice with damage reduction.
  - 🟧 **Explosive (Orange)** — Volatile nodes triggering violent blast shockwaves.
  - 🟨 **Electric (Yellow)** — Conductive conduits that fork lightning arcs to neighboring blocks.
  - 🟩 **Poison (Green)** — Acidic bio-pixels that corrode surrounding material over time.
  - ⭐ **Golden Core (Gold)** — The ancient heart of the structure shielded by dense matter.

### 🔮 Specialized Orb Archetypes
- **Kinetic Orb**: High-velocity ballistic projectile with elastic ricochet mechanics.
- **Lightning Orb**: Emits branching electrical arcs to zap clusters of pixels in proximity.
- **Poison Orb**: Infuses hit targets with corrosive acid that ticks damage over time.
- **Laser Orb**: High-frequency beam penetrator that punches straight through lines of matter.

### ⚡ Roguelite Synergy Drafting & Progression
- **Post-Wave Card Drafts**: Choose 1 of 3 procedural upgrade cards between stages to customize your build during each run.
- **Permanent Upgrade Tree (19+ nodes)**:
  - **Ball Systems**: Speed, Damage, Radius, Volley Size, Bounce Efficiency.
  - **Destruction**: Blast Radius, Lightning Jump Count, Critical Chance, Detonation Probability.
  - **Economy**: Bits Per Pixel, Combo Multipliers, Bit Magnetism.
  - **Automation**: Deployable Auto-Turrets, Turret Overclocking, Orbital Excavation Drones, Passive Erosion.
  - **Projectiles**: Unlock and cycle between Orb types.
- **Combo Multiplier Engine**: String together rapid destruction chains to multiply bit collection up to 10× and beyond.

### 🛡️ Cyber Energy Arena & Tactile Boundaries
- Visible neon boundary rails with real-time impact energy flares and shockwave ripples when balls bounce.
- Laser-etched coordinate ticks, sector corner brackets, and hazard void drop threshold.
- Visual and acoustic **Core Radar**: A proximity tracker that increases in pulse frequency as your orbs dig closer to the hidden Golden Core.

### 🎵 Procedural Web Audio Synthesizer
- 100% synthesized sound effects powered by the Web Audio API with zero external audio assets.
- Dynamic pitch-scaled collision chimes, laser sweeps, explosive thuds, and combo chords.

---

## 🕹️ Controls

| Action | Mouse / Touch | Keyboard |
| :--- | :--- | :--- |
| **Aim & Launch** | Click/tap & drag on field to aim, release to launch | <kbd>Space</kbd> (Launch) |
| **Recall Balls** | Click **⚡ RECALL** button | <kbd>R</kbd> |
| **Pan Camera** | Click & drag with Middle/Right Mouse or 2-finger drag | <kbd>W</kbd> <kbd>A</kbd> <kbd>S</kbd> <kbd>D</kbd> or <kbd>↑</kbd> <kbd>←</kbd> <kbd>↓</kbd> <kbd>→</kbd> |
| **Zoom View** | Mouse Wheel / Pinch Gesture | — |
| **Toggle Game Speed** | Click **1X / 2X** speed button | — |
| **Pause / Menu** | Click Pause button | <kbd>Esc</kbd> |
| **Mute Audio** | Sound icon in Settings / HUD | <kbd>M</kbd> |

---

## 🚀 Deployment (GitHub Pages)

This project has **zero build steps** and **zero external dependencies**. All styling, game logic, canvas rendering, and sound synthesizers are contained within `index.html`.

To host your own copy on GitHub Pages:

1. Push or fork the repository to GitHub.
2. Go to **Settings** → **Pages** (`https://github.com/<your-username>/Depixeler/settings/pages`).
3. Under **Build and deployment**:
   - **Source**: `Deploy from a branch`
   - **Branch**: `main` | `/ (root)`
4. Click **Save**. Within 1–2 minutes, your game is live!

---

## 🛠️ Architecture & Tech Stack

- **Graphics**: HTML5 2D Canvas with chunk-dirty-rect offscreen rasterization.
- **Memory**: Flat typed arrays (`Uint8Array`, `Uint32Array`, `Float32Array`) for cache-friendly pixel grid and projectile loops.
- **Audio**: Web Audio API Procedural Synthesizer (sine, triangle, saw, white-noise nodes + dynamic gain/frequency envelopes).
- **Save State**: LocalStorage persistence for lifetime runs, currencies, unlocks, and statistics.
- **Design System**: Retro-futuristic dark neon palette inspired by classic vector and arcade aesthetics.

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).