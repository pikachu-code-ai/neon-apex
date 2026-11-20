# neon-apex# 🏎️ NEON APEX — Cyberpunk Pseudo-3D Highway Racer

**NEON APEX** is a fast-paced, OutRun-inspired pseudo-3D cyberpunk highway racer built entirely in a single, zero-dependency HTML5 file. Weave through synthwave skylines at 350+ KM/H, battle rival AI racers, master 3-tier Apex Drifts on escalating mountain and highway circuits, and unleash Hyper Overdrive EMP blasts.

---

## ✨ Key Features

- **Customisable Race Setup:** Independently toggle **Track Levels (1–5+)**, **AI Bot Racers (Solo, 3, 5, or 8 Bots)**, and **Highway Obstacles (Clear Road vs. Easy Traffic)**.
- **Progressive Track Geometry:** Every level introduces sharper hairpins, rapid S-chicanes, steeper blind hills, stronger cornering G-forces, and narrower asphalt.
- **Competitive AI Pack Racing:** Race against up to 8 named cyber-bots (`VEX-09`, `KAIRO`, `NYX`, `ZERO`, `SOLARIS`, `ECHO`, `PULSE`, `RONIN`) with adaptive rubber-banding, slipstream grazing, friendly side-bumps, and a real-time **Vertical Pack Radar**.
- **Forgiving Arcade Physics:** Features auto-cruise acceleration, 8 regenerating Aegis Shields (+1 shield every 10 seconds), wide near-miss graze hitboxes, and Endless Mode progression beyond the finish line.
- **Procedural Web Audio Synthesizer:** Real-time synthesized laser blasts, drift charge harmonics, graze chimes, power-up arpeggios, and crash bursts—no external audio files required.

---

## 🏁 Track Levels

| Level | Circuit Name | Distance Goal | Track Characteristics |
| :--- | :--- | :---: | :--- |
| **Level 1** | **Neon Sweepers** | `4,000 m` | Wide asphalt with smooth, forgiving sweeping turns |
| **Level 2** | **Twin Chicanes** | `5,000 m` | Rapid S-bends and rolling elevation crests |
| **Level 3** | **Blind Hairpins** | `6,000 m` | Sharp hairpin turns paired with steep drops |
| **Level 4** | **Omega Corkscrew** | `7,000 m` | Heavy G-force switchbacks and tighter lanes |
| **Level 5** | **Apex Master** | `8,000 m` | Narrow technical circuit with double-apex hairpins and fast rival bots |
| **Level 6+** | **Endless Hyper Apex** | `∞` | Automatically scales road curvature, hills, and speed every 2,500m in Endless Mode |

---

## ⚡ Gameplay Mechanics & Power-Ups

### Core Mechanics
- **Near-Miss Graze Combos (Up to 16X):** Skim close to traffic or rival bots to trigger electric graze arcs, build your score multiplier, and charge Overdrive energy.
- **Apex Drift (`Shift`):** Hold Drift while steering through corners to charge 3 boost tiers (**Tier 1 Cyan** ➔ **Tier 2 Magenta** ➔ **Tier 3 Gold**). Releasing grants an immediate speed surge.
- **Hyper Overdrive (`Space` / `E` / `Enter`):** Once charged to 100%, unleash an EMP wave that converts nearby traffic into magnetic score crystals while granting invulnerability, 2X score, and twin plasma cannons for 7 seconds.
- **Neon Chevron Boost Pads:** Drive over glowing green road chevrons for an instant `+60 KM/H` surge.
- **Sector Bosses (Obstacles ON):** At the halfway point of a run, face the 3-phase **OMEGA ENFORCER** dreadnought with telegraphed 3D lane lasers.

### 6 Tactical Power-Up Capsules
- **⚡ PLASMA CANNONS (`10s`):** Fires twin forward plasma bolts that vaporize traffic into magnetic crystals and damage bosses.
- **🛡️ AEGIS RAM SHIELD (`+1 Shield & 9s`):** Restores 1 hull shield and activates a barrier that smashes rival cars and traffic off the road.
- **🧲 MAGNET SIPHON (`10s`):** Pulls score crystals and power-up capsules toward your car across all lanes.
- **👻 PHASE CLOAK (`8s`):** Allows you to phase safely through traffic while still earning near-miss graze points.
- **⏳ CHRONO FLOW (`8s`):** Slows down highway traffic and boss attack timers by 50%.
- **🚀 TWIN TURBO (`9s`):** Unlocks a `420 KM/H` top speed and doubles Apex Drift charge speed.

---

## 🎮 Controls

### Desktop
| Key | Action |
| :--- | :--- |
| **`A` / `D`** or **`◀` / `▶`** | Steer Left / Right |
| **`W`** or **`▲`** | Surge Boost (above auto-cruise speed) |
| **`S`** or **`▼`** | Brake |
| **`Shift`** | Hold while steering to **Apex Drift** |
| **`Space` / `E` / `Enter`** | Activate **Hyper Overdrive** (at 100%) |
| **`P`** or **`Esc`** | Pause / Resume Game |
| **`M`** | Toggle Synthesizer SFX Mute |

### Mobile & Touch Devices
- **Steering:** Use the on-screen **`◀` / `▶`** touch pads or **touch-and-drag** directly anywhere on the highway canvas.
- **Drifting:** Hold the **`🌀 DRIFT`** button while steering.
- **Overdrive:** Tap the **`OVERDRIVE`** button when charged to 100%.

---

## 🛠️ Technical Architecture

- **Single-File Portable Bundle:** All HTML, responsive CSS, game logic, rendering, and audio synthesis live inside `neon_apex.html`.
- **Pseudo-3D Projection Engine:** Projects segmented road geometry with dynamic horizontal curvature, vertical hills, rumble strips, and roadside pylons onto an HTML5 2D Canvas.
- **Zero-GC Object Pooling & Sprite Atlas:** Pre-renders neon glow strokes onto offscreen canvases at startup and recycles particles, plasma bolts, crystals, and score popups through fixed-capacity object pools for smooth 60 FPS performance.

---

## 🚀 How to Run

1. Download `neon_apex.html`.
2. Open the file directly in any modern desktop or mobile web browser (Chrome, Edge, Safari, Firefox)—no build tools or local server required.
