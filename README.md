# Breakitt

A silly website to break things and forget about your stress for a minute.

Swipe/drag through the plates, bowls, cups, pots and vases sitting on the shelf and watch them shatter. That's it. That's the whole app.

Made for trying out [Matter.js]— physics, shard generation, procedural crunch sounds, score/combo stuff, all of it just for fun.

## Run it

Open `index.html` in a browser. No build step, no dependencies to install.

Or clone it and use a local server if you want:

```bash
git clone https://github.com/your-username/breakitt.git
cd breakitt
python3 -m http.server
```

Then go to `localhost:8000`.

## Live demo

https://akshara200829-lgtm.github.io/Breakitt/

## How it works

- **Matter.js** handles all the physics — gravity, shard collisions, impulses on impact
- Swipe speed and drag distance decide if a hit counts as a "smash"
- Shards get generated procedurally (irregular polygon slices from the impact point), not pre-made assets
- Each object type (plate/bowl/cup/pot/vase) has its own weight, shard count, sound, and point value
- Crunch sounds are generated on the fly with the Web Audio API — no sound files
- Broken shelf items respawn after a short delay

## Assets

Product photos background-removed and cropped for the shelf sprites. Shelf background is a stock photo.

## Why

No real reason. Wanted to build something dumb and satisfying while learning Matter.js.
