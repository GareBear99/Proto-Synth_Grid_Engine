# SYNTH GRID ENGINE

<p align="center">
  <img src="geometry-synth-banner.svg" alt="Synth Grid Engine animated geometry banner" width="100%" />
</p>

<p align="center">
  <strong>Deterministic 2D simulation.</strong><br/>
  <strong>Projected to feel visually 3D.</strong><br/>
  <strong>Blueprint geometry becomes computation.</strong>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/status-experimental-7c3aed?style=for-the-badge" alt="Status: Experimental" />
  <img src="https://img.shields.io/badge/runtime-browser-2563eb?style=for-the-badge" alt="Runtime: Browser" />
  <img src="https://img.shields.io/badge/server-none-db2777?style=for-the-badge" alt="Server: None" />
  <img src="https://img.shields.io/badge/sim-deterministic-16a34a?style=for-the-badge" alt="Sim: Deterministic" />
</p>

<p align="center">
  <a href="#overview">Overview</a> •
  <a href="#features">Features</a> •
  <a href="#screenshots">Screenshots</a> •
  <a href="#controls">Controls</a> •
  <a href="#run-local">Run Local</a> •
  <a href="#support">Support</a> •
  <a href="#community">Community</a>
</p>

---

## Overview

Synth Grid Engine is a **math-first world runtime** where shell geometry, module layout, and deterministic execution all share the same blueprint-driven foundation.

Instead of treating geometry as decoration, this project treats geometry as **structure**, **storage**, and **execution space**.

The world itself becomes a programmable environment.

### Core model

- **Shell Blueprints** define world geometry
- **Module Blueprints** inject systems into the shell
- **Execution Layer** runs deterministic simulation logic
- **Rendering Layer** projects the simulation to feel visually 3D

**Geometry = storage**  
**Movement = computation**  
**Entities = executors**

---

## Why this is different

Most engines begin with rendering, then layer behavior on top.

Synth Grid Engine starts from the opposite direction:

- simulation first
- geometry first
- determinism first
- rendering as projection, not authority

That makes it useful for:

- reproducible world states
- low-weight simulation on old hardware
- modular runtime experiments
- blueprint-driven systems design
- future shell/module ecosystems

---

## Features

- Deterministic 2D simulation core
- Visually 3D projection style
- Blueprint-defined shell structures
- Modular attachment system for runtime components
- Seed-based world reproducibility
- Low overhead browser execution
- Debug-friendly architecture
- No server required

---

## Screenshots

### Iteration 8 — Example World

![Iteration 8 Example World](images/Image1.jpeg)

Included example blueprint: `blueprint_octagon.json`

Builds an octagon shell structure where modules can attach.

### Iteration 9 — Game Engine Prototype

![Synth Grid Engine Prototype](images/Image2.jpeg)

Prototype showing the deterministic shell simulation projected into a visually 3D-feeling environment.

Demonstrates:

- blueprint shell generation
- cube-grid projection mapping
- deterministic seed worlds
- modular system attachment
- spatial execution visualization

### Iteration 10 — Synth Grid Engine

![Synth Grid Engine](images/Image3.jpeg)

A blueprint-driven simulation shell where geometry becomes computation.

---

## Architecture

### 1. Shell Blueprint
Defines the shape of the world.

### 2. Module Blueprints
Attach behavior and systems into that world.

### 3. Execution Layer
Runs the deterministic simulation loop.

### 4. Projection Layer
Transforms 2D simulation state into a visually 3D presentation.

---

## Math-First Simulation

The engine is **math-first, not graphics-first**.

All simulation logic runs in deterministic 2D vector space. Rendering then projects that simulation into a visually 3D environment using techniques such as:

- perspective scaling
- layered sprites
- cube-grid projection
- depth shading

This gives the project several advantages:

- extremely low CPU usage
- deterministic reproducibility
- simple debugging and validation
- broad hardware compatibility

Even older machines can run the simulation cleanly because the project avoids the weight of a traditional 3D engine.

---

## Controls

| Key | Action |
|---|---|
| WASD | Move master control |
| Mouse | Aim vector |
| C | Toggle reticle |
| ` | Toggle debug overlay |
| R | Reset |

---

## Run Local

1. Clone or download the repository
2. Keep the folder structure intact
3. Open `index.html` in a browser

No server required.

---

## Loading Blueprints

Upload blueprints through the runtime UI.

Recommended order:

1. Shell blueprint
2. Ship module
3. Scanner module
4. HUD module (optional)

### Example module blueprint

```json
{
  "moduleType": "scanner",
  "id": "SCAN_01",
  "style": "default",
  "config": {},
  "script": ""
}
```

---

## Roadmap

- Expand shell blueprint vocabulary
- Improve module interoperability
- Extend scanner and HUD systems
- Formalize blueprint validation
- Add richer debug and visualization tooling
- Grow toward full Synth Grid runtime ecosystem

---

## Contributing

Contributions, experiments, architecture suggestions, and bug reports are welcome.

### Best ways to contribute

- Open an **Issue** for bugs or feature requests
- Start a **Discussion** for ideas, architecture, and direction
- Submit a **Pull Request** for improvements
- Star the repo to help surface the project
- Share the repo with people into engine architecture, simulation, or procedural systems

---

## Community

Use these repo surfaces to help the project grow:

- **Issues** → bug reports, tasks, feature requests
- **Discussions** → architecture talk, ideas, showcases, Q&A
- **Pull Requests** → direct improvements
- **Releases** → versioned drops when milestones are reached
- **Projects** → roadmap and task tracking, if enabled
- **Wiki** → long-form engine documentation, if enabled

### Suggested promotion setup for the repo

- Enable **Discussions** in repo settings
- Add **issue templates** for bug report / feature request / question
- Add a **pull request template**
- Pin a strong **Discussion welcome thread**
- Create a first **Release** once the README + visuals are stable
- Add repo **topics** like `simulation`, `engine`, `procedural`, `browser`, `deterministic`, `blueprint`, `javascript`

---

## Support

If you want to support the project directly, add your support links here.

### GitHub Sponsors

```md
[![Sponsor on GitHub](https://img.shields.io/badge/Sponsor-GitHub-ea4aaa?style=for-the-badge&logo=githubsponsors)](https://github.com/sponsors/YOUR_GITHUB_USERNAME)
```

### Buy Me a Coffee

```md
[![Buy Me a Coffee](https://img.shields.io/badge/Buy%20Me%20a%20Coffee-Support-ffdd00?style=for-the-badge&logo=buymeacoffee&logoColor=000000)](https://www.buymeacoffee.com/YOUR_HANDLE)
```

### Example support block for this README

Replace the placeholders above, then drop this into the top section if you want the buttons visible immediately:

```md
<p align="center">
  <a href="https://github.com/sponsors/YOUR_GITHUB_USERNAME">
    <img src="https://img.shields.io/badge/Sponsor-GitHub-ea4aaa?style=for-the-badge&logo=githubsponsors" alt="Sponsor on GitHub" />
  </a>
  <a href="https://www.buymeacoffee.com/YOUR_HANDLE">
    <img src="https://img.shields.io/badge/Buy%20Me%20a%20Coffee-Support-ffdd00?style=for-the-badge&logo=buymeacoffee&logoColor=000000" alt="Buy Me a Coffee" />
  </a>
</p>
```

---

## Repo Links

Once enabled, you can also add direct links like these near the top of the README:

```md
- [Issues](../../issues)
- [Discussions](../../discussions)
- [Pull Requests](../../pulls)
- [Releases](../../releases)
```

Or as a centered block:

```md
<p align="center">
  <a href="../../issues">Issues</a> •
  <a href="../../discussions">Discussions</a> •
  <a href="../../pulls">Pull Requests</a> •
  <a href="../../releases">Releases</a>
</p>
```

---

## License

Add your preferred license here.

If this is still experimental, even a simple placeholder is better than leaving it ambiguous.

---

## Notes

This project is part of a broader direction exploring deterministic simulation, modular runtime systems, and geometry-driven execution environments.
