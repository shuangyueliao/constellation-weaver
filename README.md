# Constellation Weaver

Rotate the night sky. Gather the linked stars. Weave all 25 constellations.

Constellation Weaver is an original single-file HTML5 puzzle game. You are the
stargazer: the stars are fixed on a celestial sphere, and you drag to spin the
sky around its axis (with a two-position tilt) to bring each linked pair of
stars together. When every dashed strand is tight — and no rule is broken —
press **WEAVE** to lock the constellation.

## How to play

- **Drag** (mouse or touch) to rotate the sky around its polar axis.
- **TILT I / II** flips the viewing axis between the two tilt positions.
- Bring every dashed pair of stars within adjacency distance — tight strands
  light up with flowing light.
- Keep **crest-marked** stars inside the moonlight (the left half of the sky).
- Keep **dark stars** (red halo) away from your strands — they pollute them.
- Never let strands cross each other.
- Press **WEAVE** to validate. Keyboard: ←/→ rotate, T tilt, Enter/Space weave.

## Features

- 25 handcrafted levels with a smooth difficulty curve: pure rotation puzzles,
  then moonlight constraints, dark-star interference, and finally five
  "drifting sky" time trials where the heavens slowly turn on their own.
- Star ratings (moves + time) and progress saved in localStorage.
- Fully procedural graphics (nebula, starlight, moon, trails) and WebAudio
  synthesized sound. No external assets, no tracking, no external links.

## Tech

Vanilla JavaScript + Canvas + WebAudio in one `index.html` (~48 KB).
The celestial-sphere projection, constraint solver and level validation are
pure functions, covered by an offline unit-test suite. Portal SDKs load only
on their own domains (CrazyGames / GameDistribution); standalone the game
loads nothing external.

All names, mechanics, artwork, level data, sounds and code are original work.
