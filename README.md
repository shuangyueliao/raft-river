# Raft River

A free single-file HTML5 river rafting dodge game. Ride an endless top-down
river that speeds up as you go. Steer your raft past rocks (lose a life),
whirlpools (suck you in for one wild second) and drifting logs, and grab
drift bottles (+5, they carry letters), fish schools (+2) and gold coins.
The river splits into forks around sandy islands — the narrow channel is
high risk but loaded with coins. Every 500 m restores a life (max 3).

**Play:** https://shuangyueliao.github.io/raft-river/

## Features

- Endless procedurally generated river with meanders and island forks;
  obstacle generation guarantees a passable channel (raft width x 1.5)
  on every cross-section, verified by automated tests
- Rock collisions cost a life with screen shake; whirlpools pull you in,
  spin you for exactly 1 second, then release with 2.5 s immunity;
  logs drift across the current
- Score = distance (1 point per 10 m) + collectibles; milestone life
  restore every 500 m; best score and best distance saved in localStorage
- Living water: animated ripple lines and flow streaks, foam on rocks,
  wake trail, parallax forest banks, rowing animation whose stroke rate
  follows your speed
- Fully synthesized audio (WebAudio): water white noise that swells with
  speed, splashes, whirlpool sweeps, coin chimes, milestone arpeggio
- Mouse drag / touch drag / arrow keys; responsive portrait-first canvas;
  auto-pause when the tab is hidden; mute button with persistence
- Zero external assets, zero analytics, zero external links in gameplay

## Controls

- Drag with mouse or finger to steer; or `←` / `→` (also `A` / `D`)
- `Enter` / `Space` to start or retry

## Tech

Vanilla JavaScript + Canvas + WebAudio in one `index.html` (~49 KB).
Portal SDKs (CrazyGames / GameDistribution) load only on their own domains;
gameplayStart / gameplayStop are wired for the CrazyGames SDK.

## Run locally

```bash
python3 -m http.server 8891
# open http://localhost:8891/
```

## License

MIT
