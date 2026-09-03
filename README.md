# Blade & Blossom — Fruit Slicer 🍉

A fast-paced, arcade-style fruit-slicing game built as a single self-contained HTML file. No install, no build step, no external assets — just open it in a browser and play.

## How to run it

1. Download `fruit-slice.html`.
2. Double-click it (or open it via File → Open in your browser).
3. That's it — everything (graphics, sound, save data) runs entirely client-side in that one file.

It also works if you drop it on any static web host (GitHub Pages, Netlify, a plain S3 bucket, etc.) — there's nothing to build or configure.

## Controls

| Input | Action |
|---|---|
| Mouse click + drag | Swipe the blade to slice fruit |
| Touch + drag (mobile/tablet) | Same as above |
| Space bar | Pause / Resume |
| Pause button (top right) | Pause the game |

## Game modes

- **Classic** — 3 lives. Missed fruit costs a life. Ends when you run out of lives or cut a bomb.
- **Time Attack** — 60-second timer. Slice as much as you can. Missed fruit doesn't cost a life, but a bomb still ends the run instantly.
- **Endless** — 3 lives, no timer, difficulty keeps climbing the longer you survive.

## Scoring & combos

- Each sliced fruit is worth a base **10 points**.
- Slicing fruit in quick succession builds a **combo multiplier**, adding bonus points and triggering messages: `Nice!` → `Combo x3!` → `GREAT!` → `PERFECT!` → `UNSTOPPABLE!`
- Cutting a **bomb** ends the game immediately, regardless of mode.

## Achievements

| Achievement | Requirement |
|---|---|
| 🥷 Fruit Ninja | Slice 100 fruits total (across all games) |
| 🔥 Combo Master | Reach a 10x combo in a single run |
| 💎 High Roller | Score 1,000+ points in one run |
| ⏳ Iron Wrist | Survive 5 minutes in one run |

High scores, total fruit sliced, best combo, and unlocked achievements are all saved automatically and persist between sessions.

## Settings

From the main menu → **Settings**, you can toggle:
- Sound effects
- Background music
- Screen shake
- Reset all saved high scores and achievements

## Technical notes

- Pure HTML/CSS/JavaScript, rendered on an HTML5 `<canvas>` — no external libraries or frameworks.
- All sound effects and music are generated on the fly with the Web Audio API (oscillators + filtered noise) — there are no audio files to load.
- Fruit emoji are used as the base art, layered with particle effects, glow, and clipped "sliced half" animations for the cutting effect.
- Difficulty (spawn rate and fruit speed) scales smoothly with score and survival time.
- Fully responsive layout — playable on desktop, tablet, and mobile.

## Customizing

Everything lives in `fruit-slice.html`. A few easy places to tweak:
- `FRUIT_TYPES` — add/remove fruit, change their size or emoji.
- `bombChance()` — adjust how often bombs spawn.
- `updateDifficulty()` — adjust the difficulty ramp.
- `COMBO_WINDOW` — adjust how forgiving the combo timing is.
- CSS `:root` variables at the top of the `<style>` block — adjust the color palette.
