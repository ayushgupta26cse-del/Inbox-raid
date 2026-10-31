# ⚡ NOVA ARCADE — Cyber Anime Multi-Game Hub & Digital Chore-Breaker

[![Version](https://img.shields.io/badge/version-2.5.0-cyan.svg)](file:///C:/Users/ayugu/.gemini/antigravity/scratch/inbox-raid/index.html)
[![Stack](https://img.shields.io/badge/tech-HTML5%20%7C%20CSS3%20%7C%20ES6%20JavaScript-magenta.svg)](file:///C:/Users/ayugu/.gemini/antigravity/scratch/inbox-raid/index.html)
[![Zero-Dependencies](https://img.shields.io/badge/dependencies-0%20(Pure%20Vanilla)-brightgreen.svg)](file:///C:/Users/ayugu/.gemini/antigravity/scratch/inbox-raid/index.html)
[![Sandbox](https://img.shields.io/badge/security-100%25%20Client--Side%20Simulated-gold.svg)](file:///C:/Users/ayugu/.gemini/antigravity/scratch/inbox-raid/index.html)

> *"Level Up Your Play. Play Games, Clear the Void."*

---

## 🌸 Overview & Vision

**NOVA ARCADE** is a responsive, highly polished anime-inspired sci-fi gaming hub engineered for Gen Z. Digital chores—especially triaging hundreds of unread emails, organizing messy repositories, and managing cognitive backlog—are notoriously prone to severe procrastination due to decision fatigue.

NOVA ARCADE gamifies chore execution by placing players in the cockpit of a futuristic cosmic command deck. Its flagship experience, **Inbox Raid**, transforms email sorting into a fast-paced 60-second arcade blitz where simulated communications are categorized rapidly into **Keep**, **Archive**, or **Purge**. Players chain rapid combos, recover lost hours, and eliminate digital dread.

Alongside Inbox Raid, the platform features a complete arcade suite of relaxing and reflex mini-games, an interactive 3D solid isometric navigation cube, an original floating mascot companion (**KIKO**), a custom theme and card loadout hangar, and flight telemetry tracking.

---

## 📁 Project Directory Structure

```text
C:\Users\ayugu\.gemini\antigravity\scratch\inbox-raid\
├── index.html          # Core single-page application and multi-view deck markup
├── styles.css          # Futuristic anime-cyber stylesheet, 3D cube engine, themes & HUD
├── serve.ps1           # Zero-dependency local PowerShell web server (port 8080)
├── README.md           # Exhaustive project documentation and technical manual
├── js/
│   └── game.js         # Core application router, Web Audio synthesizer, mini-game engines,
│                       # particle system, KIKO assistant, and localStorage telemetry
└── data/
    └── emails.js       # 30 believable, witty, and fictional sample transmission datasets
```

---

## 🎮 Core Games & Experiences

### 1. 📬 Inbox Raid (The Flagship Chore-Breaker)
- **Triage Mechanics**: Sort through a stack of 20 randomized transmissions within a 60-second radial countdown.
- **Three Core Decisions**:
  - **Keep (<kbd>K</kbd> / Swipe Right)**: Retain important tasks or replies in active memory (+100 base score).
  - **Archive (<kbd>A</kbd> / Swipe Down)**: File receipts, newsletters, and reference logs into the cold vault (+100 base score).
  - **Purge (<kbd>D</kbd> / Swipe Left)**: Vaporize cold pitches, promos, and spam clutter (+100 base score).
- **Quantum Streak Multiplier**: Consecutive decisions made within 3.8 seconds build a streak multiplier up to **3.0x MAX**. Rapid decisions under 1.4 seconds grant an additional **+25 Swift Reflex bonus**.
- **Instant Decision Rollback (<kbd>Z</kbd>)**: Reversible undo stack restores points, timers, and stack state seamlessly.
- **Mission Results Telemetry**: Breakdown of final score, pilot rank (Recruit to S-Rank Void Commander), transmissions cleared, peak streak, time saved estimate, decision pace, vector distribution charts, and a collapsible inspection drawer.

### 2. 🌸 Star Garden (Zen Botanical Experience)
- **Concept**: A tranquil cosmic garden for mindful unwinding.
- **Gameplay**: Click or tap anywhere across a drifting starfield canvas to catch comets and cultivate animated neon celestial blossoms with glowing layered petals and sparkling starlight cores.
- **Features**: Real-time canvas particle rendering, blossom counter, and one-click reset control (`🔄`).

### 3. 🚀 Nebula Dodger (30-Second Adrenaline Reflex Runner)
- **Concept**: High-speed reflex flight simulator through asteroid swarms.
- **Gameplay**: Pilot a nimble cyber ship using smooth mouse tracking or touchscreen gestures. Dodge incoming dense cosmic asteroids while collecting emerald energy cores to rack up points during a 30-second blitz.
- **Features**: Dual-axis collision detection, thruster fire particle trails, dynamic spawn balancing, and score tracking.

### 4. ⚡ Data Core Meltdown Escape (Reactor Suspense Puzzle)
- **Concept**: Emergency reactor room containment crisis.
- **Gameplay**: 4 critical reactor containment rods (**Alpha**, **Beta**, **Gamma**, **Delta**) suffer sudden heat spikes. Players must diagnose and click the vibrating rods in sequence before the 25-second thermal countdown hits zero.
- **Features**: Visual overheat jitter animations, status indicators, and multi-tone sound confirmations.

### 5. 🏬 Management & Idle Tycoon Discovery
- **Curation Hub**: Curated showcase for management simulation tycoons, including:
  - **My Dream Mall** (Retail Paradise Builder)
  - **Ideal Bank Tycoon** (High-Finance Banking Simulator)
  - **Idle Cinema Empire** (3D Movie Mogul)
  - **Cyber Bistro Manager** (Neon Ramen & Tea Automation)
- **Safe Iframe Compliance**: Built with legitimate sandbox verification notices and in-site preview modals, ensuring external simulations respect user privacy without broken embeds.

---

## 🎲 3D Solid Isometric Cube Engine

The central feature of the Home deck is an advanced 3D solid isometric navigation cube:

```
                  +-------------------+
                 /   📋 BRIEFING     /|
                /       (Top)       / |
               +-------------------+  |
               |                   |  |
               |                   | ⚡ RAID
               |     🏠 HOME       |  | (Right)
               |     (Front)       |  |
               |                   | /
               |                   |/
               +-------------------+
```

- **Solid 3D Cube Geometry**: Built with strict isometric orientation (`rotateX(25deg)`), opaque cyber shielding (`background: rgba(8, 14, 38, 0.98)`), and `backface-visibility: hidden`. Rear faces are occluded, presenting a single solid 3D block with exactly **three visible faces at any time** (Front, Right, Top).
- **Zero-G Levitation & Harmonic Nutation**: Encapsulated in `.cube-levitation-wrap` to execute organic zero-gravity bobbing (`translateY(-9px)` to `translateY(9px)`) with subtle gyroscopic roll angles.
- **Kinetic 3D Dragging with Inertia**: Click and drag with mouse or touch to freely spin the cube in 3D across pitch and yaw. Releasing coasts with damping friction and snaps to the nearest face (`cubic-bezier(0.34, 1.35, 0.64, 1)`).
- **Interactive Mouse Parallax & Hover Deceleration**: Cursor movement tilts the orbital rings and cube in opposing parallax directions; hovering over the stage smoothly decelerates the spin (`.slow-spin`) for effortless reading.
- **3D Face Detachment ("Holo-Pop")**: Hovering or focusing any face projects it outward in 3D space (`translateZ(72px)`), animating white/magenta corner cyber brackets and triggering a holographic scanline sweep (`.face-shimmer`).
- **Internal Pulsing Plasma Core**: An inner glowing plasma reactor with counter-rotating dashed lattice rings radiates cyan and magenta luminescence through beveled edges.
- **Discoverable Controls**: Step-by-step `◀` and `▶` rotation arrows and an active orientation indicator (`Facing: 🏠 Home`, `Facing: ⚡ Inbox Raid`, etc.) ensure full discoverability without unfolding the cube.

---

## 🎨 UI/UX Design System & Customization

### 1. App-Style Icon Controls & Global Tooltips
- **No Text Clutter**: Prominent text controls were replaced with sleek, recognizable app-style icon buttons:
  - Pause dock: Resume (`▶` + `<kbd>Esc</kbd>`), Restart (`🔄` + `<kbd>R</kbd>`), and Home (`🏠`).
  - Action icons: Universal `✕` (Close) and `🔄` (Reset) controls.
  - Play crests: Recognizable glowing circular play buttons (`btn-play-crest`, `btn-play-game-icon`).
- **CSS Tooltip System (`[data-tooltip]`)**: All icon-only buttons display a floating, sci-fi bordered tooltip with action names on hover and keyboard focus (`:focus-visible`), complete with `aria-label` accessibility.

### 2. Original Anime Character Artwork (Zero Copyright Infringement)
All game artwork and badges are custom-crafted vector SVGs:
- **🌸 Star Garden**: *Aoi (Celestial Blossom Maiden)* — Gentle sakura spirit with floral hairpins and starlight aura.
- **🚀 Nebula Dodger**: *Ren (Flight Ace Pilot)* — High-velocity pilot with cyber visor HUD reflection and thrusters.
- **⚡ Core Escape**: *Kai (Reactor Hacker)* — Cyberpunk technician with illuminated diagnostic goggles.
- **📬 Inbox Raid**: *Luna (Chrono Courier)* — Quantum data messenger with holographic wings.
- *Strictly original artwork — zero Marvel, LEGO, or third-party copyrighted characters.*

### 3. Compact Records & Telemetry (No White Boxes)
- High Score, Longest Streak, Total Transmissions, and Time Saved are styled as compact cyber app tiles (`.record-tile`) with dark frosted gradients, neon perimeter borders, and custom anime SVG crests.
- Telemetry logs are stored persistently in browser `localStorage`.

### 4. Hangar Loadout & Theme Engine
Switch between 4 cosmic color themes and 3 holographic card styles on the fly:

| Theme ID | Name | Primary Core | Accent Pulse | Atmosphere |
| :--- | :--- | :--- | :--- | :--- |
| `quantum` | **Quantum Nexus** | Electric Cyan (`#00f2fe`) | Anime Pink (`#ff3388`) | Deep Indigo Void |
| `solar` | **Solar Flare** | Radiant Gold (`#ffaa00`) | Sunspot Ember (`#ff4400`) | High-Contrast Stellar Plasma |
| `cyberpunk`| **Cyberpunk Matrix**| Acid Green (`#00ffaa`) | Hot Pink (`#ff0077`) | Subterranean Terminal |
| `stealth` | **Stealth Void** | Ice Cyan (`#38bdf8`) | Slate Steel (`#64748b`) | Tactical Low-Signature Display |

#### Hologram Card Surface Styles
- **Holo-Glass**: Frosted glass with blurred nebular refraction and sleek cyan borders.
- **Tactical Armor**: Solid midnight shielding (`#091026`) with sharp vector outlines for high contrast.
- **Neon Hyperdrive**: Electrified magenta perimeter glow with high-intensity chromatic aura.

### 5. Playful "Bubble-Focus" Optics
- Cards and controls subtly enlarge and highlight when hovered or focused, like a magnifying bubble (`transform: scale(1.045) translateY(-3px)`).
- Can be toggled On/Off in **Settings** or automatically suppressed when reduced motion is preferred.

### 6. KIKO — Original AI Mascot Companion
- A friendly, floating anime companion located in the screen corner.
- Offers interactive guidance, rules explanations, and digital triage advice via an expandable local chat panel.
- Operates 100% locally in client memory with zero external API calls or network latency.

---

## 🕹️ Controls & Keyboard Shortcuts

| Action | Mouse / Touch Gesture | Keyboard Shortcut |
| :--- | :--- | :---: |
| **Keep Transmission** | Click Keep Button / Swipe Right | <kbd>K</kbd> or <kbd>→</kbd> |
| **Archive Transmission** | Click Archive Button / Swipe Down | <kbd>A</kbd> or <kbd>↓</kbd> |
| **Purge Transmission** | Click Purge Button / Swipe Left | <kbd>D</kbd> or <kbd>←</kbd> |
| **Undo Last Decision** | Click Revert Button | <kbd>Z</kbd> or <kbd>Ctrl+Z</kbd> |
| **Pause / Resume Raid** | Click Pause Button in HUD | <kbd>P</kbd> or <kbd>Esc</kbd> |
| **Restart Raid** | Click Restart Button in Pause Modal | <kbd>R</kbd> |
| **Rotate 3D Cube** | Click Cube Face, Drag Stage, or Click ◀ / ▶ | <kbd>Enter</kbd> / <kbd>Space</kbd> on focused face |
| **Summon KIKO Assistant** | Click Floating Mascot in Bottom-Right | Focus & <kbd>Enter</kbd> |
| **Inspect Safety Popover** | Right-click marked simulation elements | Tab focus |

---

## 🛡️ Simulation Safety & Privacy Guarantee

> **IMPORTANT**: NOVA ARCADE is an entirely self-contained educational prototype and chore game.
> - **Zero Real Email Access**: Does not connect to Gmail, Outlook, IMAP, POP3, or any email server.
> - **Zero External Data Transmission**: All 30 fictional emails in `data/emails.js` are mock records loaded locally.
> - **Zero Data Collection**: No cookies, tracking beacons, or analytics scripts are embedded.
> - **Local State Persistence**: High scores, theme settings, and streaks are stored strictly within the user's browser `localStorage` and `sessionStorage`.

---

## 🚀 How to Run the Website

### Option 1: Direct Browser Launch
Open `index.html` directly in Google Chrome, Microsoft Edge, Mozilla Firefox, or Safari:
```powershell
Start-Process "C:\Users\ayugu\.gemini\antigravity\scratch\inbox-raid\index.html"
```

### Option 2: Local HTTP Server (PowerShell)
Run the built-in lightweight local web server script:
```powershell
powershell -ExecutionPolicy Bypass -File C:\Users\ayugu\.gemini\antigravity\scratch\inbox-raid\serve.ps1
```
Open your browser and navigate to:
```text
http://localhost:8080/
```

### Option 3: Static Hosting Deployment
The project is 100% static (HTML, CSS, JS). Deploy instantly to any static host by pushing the directory to:
- **GitHub Pages**: Upload repository and enable Pages on `main` branch.
- **Vercel**: Run `vercel` from the root directory.
- **Netlify**: Drag and drop the `inbox-raid` folder into Netlify Drop.

---

## ♿ Accessibility & Device Compatibility

- **Screen Reader Support**: Equipped with live region announcers (`#screenReaderAnnouncer` with `aria-live="polite"`), descriptive `aria-label` attributes on icon-only controls, and semantic HTML5 headings.
- **Visible Keyboard Focus**: Crisp, high-contrast cyan focus rings (`:focus-visible`) on all interactive buttons, cards, and inputs.
- **Reduced Motion Support**: Fully respects OS preference `prefers-reduced-motion: reduce` and provides an explicit manual toggle in **Settings** to disable starfield drift, nebular floating, and cube auto-spinning.
- **Responsive Layout**: Fluid CSS Grid and Flexbox layouts optimized across desktop ultra-wides, laptops, tablets, and mobile smartphones with native touch-swipe gestures.

---

## 📄 License & Attribution

Designed and engineered as a high-fidelity interactive prototype for **PromptWars**.  
All character illustrations, crests, synthesized Web Audio tones, and code are original creations. All simulated company names and email transmissions are fictional.
