# 🍉 Blade & Blossom — Fruit Slicer

<p align="center">
  <img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white" alt="HTML5" />
  <img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white" alt="CSS3" />
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" alt="JavaScript" />
  <img src="https://img.shields.io/badge/Canvas-2C3E50?style=for-the-badge&logo=html5&logoColor=white" alt="Canvas" />
  <img src="https://img.shields.io/badge/WebAudio-4A90D9?style=for-the-badge&logo=web-audio-api&logoColor=white" alt="Web Audio API" />
  <br />
  <img src="https://img.shields.io/badge/Single_File-✓-brightgreen" alt="Single File" />
  <img src="https://img.shields.io/badge/No_Dependencies-✓-brightgreen" alt="No Dependencies" />
  <img src="https://img.shields.io/badge/Offline_Ready-✓-brightgreen" alt="Offline Ready" />
  <img src="https://img.shields.io/badge/Mobile_Friendly-✓-brightgreen" alt="Mobile Friendly" />
</p>

<p align="center">
  <strong>A fast-paced, arcade-style fruit-slicing game — pure HTML/CSS/JS, no install required.</strong>
</p>

<p align="center">
  <a href="#-demo">Demo</a> •
  <a href="#-features">Features</a> •
  <a href="#-how-to-play">How to Play</a> •
  <a href="#-game-modes">Game Modes</a> •
  <a href="#-achievements">Achievements</a> •
  <a href="#-technical-details">Technical Details</a>
</p>

---

## 🎮 Demo

> **Play instantly:** Download `fruit-slice.html` and open it in any browser — no server required!

<p align="center">
  <img src="https://via.placeholder.com/800x500/1a1a2e/ffffff?text=Blade+%26+Blossom+Gameplay+Preview" alt="Blade & Blossom Gameplay Preview" width="100%" />
  <br />
  <em>Slice fruit, build combos, and climb the leaderboard!</em>
</p>

---

## ✨ Features

| Feature | Description |
|---------|-------------|
| **🗡️ Fluid Slicing** | Satisfying swipe mechanics with particle effects and sliced fruit animations |
| **🎮 3 Game Modes** | Classic (3 lives), Time Attack (60s), and Endless (escalating difficulty) |
| **🔥 Combo System** | Build multipliers with quick slices — "Nice!" → "Combo x3!" → "GREAT!" → "PERFECT!" → "UNSTOPPABLE!" |
| **🏆 4 Achievements** | Unlockable milestones that persist between sessions |
| **🎵 Procedural Audio** | All sounds and music generated via Web Audio API — no external files |
| **📊 Persistent Stats** | High scores, total fruit sliced, best combo, and achievements saved locally |
| **⚙️ Custom Settings** | Toggle sound effects, background music, and screen shake |
| **📱 Fully Responsive** | Plays beautifully on desktop, tablet, and mobile |
| **📦 One File** | Everything in a single HTML file — no build step, no dependencies |

---

## 🚀 How to Run

### Option 1: Local

```bash
# Download the file
curl -O https://example.com/fruit-slice.html

# Open in your browser
open fruit-slice.html   # macOS
start fruit-slice.html  # Windows
xdg-open fruit-slice.html # Linux
```

### Option 2: Double-Click

Just download `fruit-slice.html` and double-click it. That's it!

### Option 3: Web Hosting

Drop it on any static host (GitHub Pages, Netlify, S3, etc.) — nothing to build or configure.

---

## 🎯 How to Play

| Input | Action |
|-------|--------|
| **🖱️ Mouse Click + Drag** | Swipe the blade to slice fruit |
| **✋ Touch + Drag** (mobile) | Same as above |
| **⌨️ Space Bar** | Pause / Resume |
| **⏸️ Pause Button** (top right) | Pause the game |

---

## 🎮 Game Modes

### 🍎 Classic Mode
- **3 lives** — miss a fruit and lose one
- **Game over** — run out of lives or cut a bomb
- **Strategy:** Precision over speed

### ⏱️ Time Attack Mode
- **60-second timer** — slice as many fruits as possible
- **No life penalty** — missed fruits don't cost lives
- **Instant death** — a bomb still ends the run
- **Strategy:** Speed and accuracy under pressure

### 🌌 Endless Mode
- **3 lives** — miss a fruit and lose one
- **No timer** — survive as long as possible
- **Escalating difficulty** — spawn rate and speed increase over time
- **Strategy:** Endurance and adaptability

---

## 🏆 Achievements

| Achievement | Requirement |
|-------------|-------------|
| 🥷 **Fruit Ninja** | Slice 100 fruits total (across all games) |
| 🔥 **Combo Master** | Reach a 10x combo in a single run |
| 💎 **High Roller** | Score 1,000+ points in one run |
| ⏳ **Iron Wrist** | Survive 5 minutes in one run |

> 💾 All progress, high scores, and unlocked achievements are automatically saved in your browser's local storage.

---

## 🎨 Visual & Audio Design

### Visual Effects
- **Fruit Emoji Art** — colorful, recognizable fruit sprites
- **Particle Systems** — juice splatter and sparkle effects
- **Sliced Animation** — fruit halves split with a satisfying cut
- **Glow Effects** — dynamic lighting for slicing impact
- **Screen Shake** — optional haptic feedback for bombs and combos

### Audio (Web Audio API)
- **Slice Sound** — crisp cutting noise
- **Combo Chimes** — escalating tones for combos
- **Bomb Explosion** — dramatic boom effect
- **Background Music** — ambient loop generated on the fly
- **No Audio Files** — everything is synthesized procedurally

---

## ⚙️ Settings

From the main menu → **Settings**, you can toggle:

- 🔊 Sound Effects
- 🎵 Background Music
- 💥 Screen Shake
- 🔄 Reset all saved high scores and achievements

---

## 🛠️ Technical Details

### Architecture

```
fruit-slice.html (single file)
├── HTML5 Canvas (rendering)
├── CSS3 (styles, animations, responsive layout)
├── JavaScript (game logic, physics, audio)
│   ├── Game loop (requestAnimationFrame)
│   ├── Physics engine (gravity, collision detection)
│   ├── Particle system (juice, sparkles)
│   ├── Combo system (timing-based multiplier)
│   ├── Audio engine (Web Audio API synthesis)
│   └── Save system (localStorage)
└── No external dependencies or assets
```

### Performance Optimization
- **Canvas rendering** — efficient drawing with `requestAnimationFrame`
- **Object pooling** — reuses particle and fruit objects
- **Responsive scaling** — adapts to any screen size
- **Touch optimization** — smooth interaction on mobile devices

---

## 🔧 Customization

Everything lives in `fruit-slice.html`. Easy places to tweak:

```javascript
// Add or remove fruit, change size or emoji
const FRUIT_TYPES = [
  { emoji: '🍎', size: 50 },
  { emoji: '🍊', size: 45 },
  // ...
];

// Adjust bomb spawn rate (0 = never, 1 = always)
function bombChance() {
  return Math.random() < 0.15; // 15% chance
}

// Adjust difficulty ramp
function updateDifficulty() {
  // Spawn rate increases by 0.1 per 10 seconds
  // Speed increases by 5% per 10 seconds
}

// Combo timing window (milliseconds)
const COMBO_WINDOW = 1500; // 1.5 seconds between slices
```

```css
/* Color palette (CSS :root variables) */
:root {
  --primary: #e74c3c;
  --secondary: #2c3e50;
  --background: #1a1a2e;
  --accent: #f1c40f;
}
```

---

## 📊 Save Data

All progress is stored in `localStorage`:

```javascript
{
  highScores: {
    classic: 0,
    timeAttack: 0,
    endless: 0
  },
  totalFruitsSliced: 0,
  bestCombo: 0,
  achievements: {
    fruitNinja: false,
    comboMaster: false,
    highRoller: false,
    ironWrist: false
  },
  settings: {
    sound: true,
    music: true,
    screenShake: true
  }
}
```

---

## 🚀 Future Roadmap

### Phase 1: Quality of Life
- [ ] Keyboard shortcuts for all actions
- [ ] Tutorial overlay for new players
- [ ] More fruit types (🍉 🥝 🍇 🍑)
- [ ] Colorblind-friendly modes

### Phase 2: Social Features
- [ ] Local multiplayer (same device)
- [ ] Shareable high score screenshots
- [ ] Online leaderboards (optional backend)

### Phase 3: Content Expansion
- [ ] Special power-ups (double points, slow motion)
- [ ] Daily challenges with unique rewards
- [ ] Seasonal themes and event modes
- [ ] Customizable blade trails

---

## 🤝 Contributing

This is a single-file project, but contributions are welcome!

### How to Contribute

1. **Fork** the repository
2. **Create** a feature branch: `git checkout -b feature/amazing-feature`
3. **Make** your changes to `fruit-slice.html`
4. **Test** thoroughly (desktop + mobile)
5. **Commit** with a clear message
6. **Push** to your branch
7. **Open** a Pull Request

### Guidelines

- Keep it **single-file** — no splitting into multiple files
- **No dependencies** — no third-party libraries
- **Mobile-first** — test on both desktop and mobile
- **Performance** — maintain 60fps on mid-range devices
- **Accessibility** — keyboard support and ARIA labels

---

## 📄 License

MIT License — see [LICENSE](LICENSE) for details.

---

## 🙏 Acknowledgments

- Inspired by classic fruit-slicing games like *Fruit Ninja* 🍉
- Built with ❤️ using pure web technologies
- Perfect for quick gaming sessions, offline play, and nostalgia

---

<p align="center">
  <strong>Slice. Combo. Dominate. 🗡️</strong>
  <br />
  <sub>One file. No limits. Pure arcade action.</sub>
</p>

<p align="center">
  <a href="#">
    <img src="https://img.shields.io/badge/Play_Now-🎮-brightgreen" alt="Play Now" />
  </a>
  <a href="#">
    <img src="https://img.shields.io/badge/Download-📥-blue" alt="Download" />
  </a>
  <a href="#">
    <img src="https://img.shields.io/badge/Star_⭐-on_GitHub-yellow" alt="Star on GitHub" />
  </a>
</p>
