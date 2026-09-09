# Breakitt

Breakitt is an interactive 2D physics simulation built with Matter.js and the Web Audio API. The application simulates dynamic fracture mechanics and procedurally synthesizes collision audio in real-time, representing an exploratory implementation of client-side rigid-body destruction.

live demo : [akshara200829-lgtm.github.io/Breakitt/](https://akshara200829-lgtm.github.io/Breakitt/).

## Features

- Swipe through an item ; it shatters into random polygon shards that fly off and settle
- Every item type has its own sound, point value, and rarity (rarer stuff = more points)
- Chain smashes fast enough and you build a combo multiplier (up to ×10)
- Screen shake dust  on impact
- Broken items respawn after a short delay so the shelves never stay empty

## How to Play
 
1. Load the page — shelves fill up with random items
2. Swipe your mouse or finger through an item to smash it
3. Keep hitting things within 3 seconds of each other to stack your combo
4. Watch your score climb, let broken items respawn, and keep playing

## Tech Stack
 
- **Matter.js** — physics engine (gravity, collisions, rigid bodies)
- **poly-decomp** — breaks shard shapes into convex pieces so collisions work right
- **Web Audio API** — every break sound is generated on the fly, no audio files
- **Vanilla HTML/CSS/JS** — no framework, no build tools
  
### How to run locally
 
Launch `index.html` directly in any standards-compliant browser, or serve the directory via Python:
 
```bash
git clone https://github.com/akshara200829-lgtm/Breakitt.git
cd Breakitt
python3 -m http.server 8000
```
 
Then open `http://localhost:8000` in your browser.
