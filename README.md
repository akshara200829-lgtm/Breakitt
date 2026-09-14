# Breakitt

Breakitt is browser based game to smash plates,bowls,vases and cups by swiping.


https://github.com/user-attachments/assets/3d7ccd8f-9b2f-4564-8c7c-20aa17e76698

live demo : [akshara200829-lgtm.github.io/Breakitt/](https://akshara200829-lgtm.github.io/Breakitt/).


To run locally:

git clone https://github.com/akshara200829-lgtm/Breakitt.git 

cd Breakitt

npx serve .


Features:

- Swipe through an item ; Drag through an item on shelf to break it
- Every item type has its own sound, point value, and rarity (rarer stuff = more points)
- Chain smashes fast enough and you build a combo multiplier (up to ×10)
- Broken items respawn after a short delay so the shelves never stay empty

How it works:
Breakitt uses Matter.js for the physics simulation — when you swipe through an object, it's replaced with a set of procedurally generated shard polygons that inherit the swipe's velocity and direction, so every break looks different.Sounds is created using Web Audio API

How to Play:
 
1. Load the page — shelves fill up with random items
2. Swipe your mouse or finger through an item to smash it
3. Keep hitting things within 3 seconds of each other to stack your combo
4. Watch your score climb, let broken items respawn, and keep playing

Tech Stack:
 
- **Matter.js** — physics engine (gravity, collisions, rigid bodies)
- **poly-decomp** — breaks shard shapes into convex pieces so collisions work right
- **Web Audio API** — every break sound is generated on the fly, no audio files
- **Vanilla HTML/CSS/JS** — no framework, no build tools
  
