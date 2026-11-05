# Raft River — Store Submission Materials

## Short description (CrazyGames / GameDistribution / itch.io, 178 chars)

Ride an endless river on your raft. Dodge rocks, whirlpools and drifting
logs, snatch bottles, fish and gold, and thread the risky narrow forks.
How far can the current take you?

## Details

- Genre: Arcade / Casual / Dodger
- Controls: Mouse drag or touch drag to steer. Keyboard: ←/→ (or A/D).
  Enter/Space to start or retry.
- Features: Endless procedural river with meanders and island forks,
  whirlpools that trap you for one second, log drifters, distance + pickup
  scoring, life restore every 500 m, best score/distance saving, mute
  toggle, auto-pause on tab switch, procedural graphics & synthesized
  sounds, single-file HTML5 (no external assets), works offline once loaded.
- Tech: Vanilla JavaScript, Canvas, WebAudio. No frameworks, no tracking.
- Guarantee: obstacle generation always leaves a passable channel of at
  least raft width × 1.5 on every cross-section (verified by automated
  tests over 200 generated worlds).

## Tags

raft, river, dodge, arcade, casual, endless, runner, water, single-file

## CrazyGames submission checklist
- [x] Self-contained index.html (SDK loads only on crazygames domains)
- [x] gameplayStart / gameplayStop / loadingStart / loadingStop / happytime events wired
- [x] Responsive (canvas scales, portrait-friendly)
- [x] No external links inside gameplay, no analytics
- [ ] Cover: cover-16x9.png (1280×720)
- [ ] Screenshots: 1280×800 raw

## GameDistribution

- Upload raft-river-gd.zip (contains only index.html).
- SDK main.min.js auto-loads on gamedistribution / gd.games domains only.

## itch.io
- Upload zip (rename to raft-river.zip), mark "This file is playable in
  browser", entry file: index.html, viewport portrait (420×780 or similar),
  kind: html.
- Pricing: $0 (donations optional)
