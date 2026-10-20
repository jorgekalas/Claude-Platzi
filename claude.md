# Project: 3D Perseverance Rover Simulation (60-minute class)

## Context
This folder is used to teach a live Claude Code class. The instructor builds, together with the students, a 3D simulation of NASA's **Perseverance** rover driving on Mars, in **under 60 minutes**. Students are beginners. Simplicity, speed and visible progress matter more than realism.

## Tech rules
- **One file only:** `index.html` with inline `<script type="module">`. No build tools, no npm, no frameworks.
- **Three.js** loaded from a CDN with an import map, pinned version:
  - `https://cdn.jsdelivr.net/npm/three@0.160.0/build/three.module.js`
  - addons: `https://cdn.jsdelivr.net/npm/three@0.160.0/examples/jsm/`
- Build the rover from **basic primitives** (boxes, cylinders, spheres). No external 3D models, textures or images. Generate any texture procedurally.
- It must open by double-clicking `index.html` or with a simple local server (`npx serve` or `python -m http.server`).
- Keep the code short, readable and well organized in clear sections with short comments. Students will read it.

## Class plan (each step should end with something visible in the browser)
| Time | Step | Result |
|------|------|--------|
| 0–10 min | Scene, camera, lights, `OrbitControls`, Martian sky | Empty 3D world |
| 10–20 min | Mars terrain: red-orange ground with procedural hills, scattered rocks | A Martian landscape |
| 20–35 min | Rover model: body, 6 wheels, mast with camera head, robotic arm, RTG at the back, antenna | Recognizable Perseverance |
| 35–45 min | Driving: WASD / arrow keys, wheels spin, rover follows the terrain height | Drivable rover |
| 45–55 min | Extras: camera follows the rover, dust particles behind the wheels, simple HUD (speed, position, "sol") | Polished simulation |
| 55–60 min | Wrap-up and optional ideas | Discussion |

Optional extras if time allows: Ingenuity helicopter flying nearby, mast rotating to look around, day/night cycle, collision with rocks.

## How Claude should work in this class
- Do **one step at a time** and keep each change small, so the class can follow along.
- After each step, say in 2–3 short sentences what was added and what to look for in the browser.
- Prefer the simplest approach that works. Don't add physics engines or complex architecture.
- If something breaks, fix it quickly and explain the cause in one sentence. It's a teaching moment.
- The class may be in Spanish: if the instructor writes in Spanish, answer in Spanish. Code comments can be in Spanish too.

## Perseverance reference (for a recognizable look)
- White/light gray body, about 3 m long, 2.7 m wide, 2.2 m tall.
- 6 aluminum wheels on a rocker-bogie suspension (show it as simple angled bars).
- Tall mast at the front with a box "head" (Mastcam-Z / SuperCam).
- 5-joint robotic arm at the front with a turret at the end.
- RTG power source: a dark finned cylinder angled at the back.
- High-gain antenna: a flat hexagonal disc on the deck.
