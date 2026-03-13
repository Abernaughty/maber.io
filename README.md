# maber.io

Landing page for [maber.io](https://maber.io) — a real-time WebGL fluid simulation built entirely in GLSL shaders and vanilla JavaScript.

## What it is

A fully custom fluid dynamics simulation running in the browser using WebGL. No physics libraries — the simulation is implemented directly in GLSL fragment shaders including advection, pressure solving, vorticity confinement, and curl.

## Tech Stack

- **WebGL + GLSL** — fluid simulation
- **Vanilla JavaScript** — no frameworks
- **Azure Static Web Apps** — hosting

## Project Structure

```
maber.io/
├── index.html
├── style.css
├── js/
│   ├── fluidSimulation.js   # Core WebGL simulation
│   └── main.js              # Entry point, interaction handling
├── shaders/                 # GLSL fragment and vertex shaders
│   ├── advection.frag
│   ├── curl.frag
│   ├── divergence.frag
│   ├── pressure.frag
│   ├── gradient.frag
│   ├── vorticity.frag
│   ├── splat.frag
│   ├── display.frag
│   └── base.vert
└── images/                  # Site assets
```

## Running locally

Open `index.html` directly in a browser — no build step required.

## Related Projects

- [Portfolio](https://github.com/Abernaughty/Portfolio) — dev.maber.io portfolio site
- [PCPC](https://github.com/Abernaughty/PCPC) — Pokémon Card Price Checker
