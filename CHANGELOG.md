# 📜 Changelog — Tom's Long Night

*All notable changes follow [Semantic Versioning](https://semver.org).*

## [Unreleased]

### Planned
- Screen shake intensity tuning
- Particle lifetime adjustments
- Minor HUD polish

---

## [1.0.0] — 2026-02-11 — Initial Release

### ✨ Features
- Core gameplay loop: stomp pumpkins, survive nights
- 4 enemy types: bats, pumpkins, ghosts, bombs
- Smart item drops (hearts/potions/stars) based on player HP
- Combo system with score multipliers
- Day progression with escalating difficulty
- Apollo-style optimized code (4082 tokens)

### 🎨 Visuals
- Clean night aesthetic: moon, stars, purple sidewalk
- Animated pumpkins (sprites 13/14)
- 3-skull game over screen
- Minimalist HUD with clock (sprite 22)

### 🔊 Audio
- 14 SFX slots mapped (ready for sound design)
- Konami code debug mode (↑↑↓↓←→←→BA)

### 🐞 Fixes
- Fixed stomp damage bug (player no longer takes damage when stomping)
- Aligned item drop height with pumpkin/Tom (y=96)
- Removed confusing pumpkin shadow
- Balanced day 1 drop rates for accessibility

### 🚀 Technical
- All loops use reverse iteration (`for i=#tbl,1,-1`) — no crashes
- Object pooling for particles/drops/enemies
- Save high scores via `dset()`/`dget()`
- Debug mode with CPU/mem/fps monitoring
