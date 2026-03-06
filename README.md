# maber.io

Personal portfolio site for [maber.io](https://maber.io), featuring a real-time WebGL fluid
simulation as a background effect.

> 🚧 **In progress** — fluid-sim background integration is planned. Currently deployed with static background.

## Tech Stack

- **[SvelteKit](https://kit.svelte.dev/)** — site framework
- **Tailwind CSS** — styling
- **WebGL + GLSL** — fluid simulation background (`/fluid-sim`)
- **Azure Static Web Apps** — hosting

## Quick Start

```bash
npm install
npm run dev        # http://localhost:5173
npm run build      # production build
npm run preview    # preview production build locally
```

## Project Structure

```
maber.io/
├── src/
│   ├── routes/              # SvelteKit pages (+page.svelte, +layout.svelte)
│   ├── lib/
│   │   ├── components/      # Reusable Svelte components (ProjectCard, etc.)
│   │   └── stores/          # Svelte stores
│   └── app.css              # Global styles
├── static/
│   └── images/              # Static assets
├── fluid-sim/               # WebGL fluid simulation (planned background effect)
│   ├── index.html           # Standalone demo
│   ├── js/                  # Simulation logic
│   └── shaders/             # GLSL fragment shaders
└── svelte.config.js
```

## The Fluid Simulation

`/fluid-sim` contains a real-time fluid dynamics simulation built entirely in WebGL and GLSL
shaders — no physics libraries. Open `fluid-sim/index.html` directly in a browser to run it
as a standalone demo.

**Planned:** integrate the fluid-sim as the animated background of the landing page hero section.

## Deployment

The site is deployed to Azure Static Web Apps via the `staticwebapp.config.json` configuration.

```bash
npm run build
# Deploy the generated build/ output to Azure Static Web Apps
```

## Scripts

```bash
npm run dev            # Dev server with hot reload
npm run build          # Production build
npm run lint           # ESLint
npm run format         # Prettier
npm run test           # Vitest unit tests
npm run test:coverage  # Test coverage report
```
