# SYNTH GRID ENGINE

<p align="center">
  <img src="assets/geometry-synth-banner.svg" alt="Synth Grid Engine animated geometry banner" width="100%" />
</p>

<p align="center">
  <b>Deterministic 2D simulation.</b>
  <br/>
  <b>Projected to feel visually 3D.</b>
  <br/>
  <b>Blueprint geometry becomes computation.</b>
</p>

<p align="center">
  <img alt="status" src="https://img.shields.io/badge/status-experimental-8a2be2">
  <img alt="runtime" src="https://img.shields.io/badge/runtime-browser-00c2ff">
  <img alt="server" src="https://img.shields.io/badge/server-none-ff4fd8">
  <img alt="simulation" src="https://img.shields.io/badge/sim-deterministic-8bff6a">
</p>

---

## What this is

Synth Grid Engine is a **math-first world runtime** where shell geometry, module layout, and deterministic execution all share the same blueprint-driven foundation.

Instead of treating the world like a background for gameplay, this system treats the world itself as an active computational structure:

- **geometry = storage**
- **movement = computation**
- **entities = executors**
- **blueprints = source of truth**

The simulation runs in **2D vector space** for clarity, repeatability, and low overhead, then projects outward into a scene that feels visually 3D.

---

## Why it matters

This engine is built around a different philosophy than a typical game prototype.

Most engines start with rendering and then bolt logic onto the visuals.
Synth Grid Engine does the opposite:

- simulation first
- geometry first
- deterministic execution first
- visuals as projection of truth

That makes it useful for:

- blueprint-driven world generation
- modular shell systems
- spatial execution visualization
- low-cost simulation on older hardware
- debugging and validation without hidden engine state
- future operating-system-like worlds and simulation shells

---

## Core architecture

### 1. Shell Blueprint
Defines the structural world shape.

Examples:
- octagons
- rings
- hulls
- shells
- custom procedural topology

### 2. Module Blueprints
Attach systems into the shell.

Examples:
- ship modules
- scanner modules
- HUD modules
- future execution or sensing systems

### 3. Execution Layer
Runs the deterministic simulation loop.

This is where movement, state transitions, interactions, and spatial logic resolve.

---

## Main design principles

### Deterministic by default
The same seed and blueprint input should produce the same world state.

### 2D core, 3D feeling
Everything important happens in a clean simulation plane.
Rendering then uses projection, scale, depth ordering, and geometry tricks to give it a spatial 3D feel.

### Modular runtime
The engine is meant to load shell and module blueprints at runtime rather than hardcoding one world forever.

### Lightweight execution
This is meant to run smoothly even on older systems without requiring a full heavyweight 3D pipeline.

### Blueprint-first development
The blueprint is not an accessory. It is the actual authority.

---

## Current iterations

## Iteration 8 — Example World

![Iteration 8 Example World](images/Image1.jpeg)

Included example blueprint:

`blueprint_octagon.json`

Purpose:
- builds an octagon shell structure
- establishes attachment points for modules
- serves as the clearest baseline world example

---

## Iteration 9 — Game Engine Prototype

<details>
<summary><b>Open Iteration 9 details</b></summary>

![Synth Grid Engine Prototype](images/Image2.jpeg)

This phase proves the simulation can function as a real runtime, not just a static concept.

Demonstrated systems:
- blueprint shell generation
- cube-grid projection mapping
- deterministic seed worlds
- modular system attachment
- spatial execution visualization

The interface supports runtime loading of:
- Shell Blueprints
- Ship Modules
- Scanner Modules
- HUD Modules

This prototype also acts as a stepping stone for the broader **ThingsHappening** systems.

</details>

---

## Iteration 10 — Synth Grid Engine

![Iteration 10 Demo](images/Image3.jpeg)

This is the clearest expression so far of the real idea:

> a blueprint-driven simulation shell where geometry becomes computation

It pushes the project beyond a simple prototype and toward a reusable world-runtime architecture.

Inspirations:
- TRON-style grid worlds
- Geometry Wars energy and spatial clarity
- modular operating-system-like environments

---

## Feature highlights

- deterministic 2D simulation core
- visually 3D projection feel
- runtime blueprint loading
- modular attachment architecture
- low-overhead execution model
- debuggable state flow
- portable browser-based runtime
- no server required

---

## Controls

| Key | Action |
|---|---|
| `WASD` | Move master control |
| `Mouse` | Aim vector |
| `C` | Toggle reticle |
| `` ` `` | Toggle debug overlay |
| `R` | Reset |

---

## Running the engine

1. Download the repository.
2. Open `index.html` in a browser.
3. Load shell and module blueprints through the runtime UI.

No server is required.

---

## Recommended blueprint load order

1. **Shell blueprint**
2. **Ship module**
3. **Scanner module**
4. **HUD module** *(optional)*

---

## Example module blueprint

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

## Technical framing

This project is best understood as a **simulation shell runtime** rather than only a game scene.

The long-term power comes from the fact that the same architecture can support:

- simulated worlds
- executable shell spaces
- modular scanning systems
- HUD-driven control surfaces
- future operating-system-like spatial interfaces

That is the deeper point of the engine:

**the environment is not decoration.**
**the environment is the machine.**

---

## Why this approach is strong

Compared to heavy traditional scene-first architectures, this structure gives you:

- easier reproducibility
- easier validation
- easier debugging
- lower hardware requirements
- cleaner future expansion into modular systems

Even older machines can run this kind of runtime comfortably because the expensive part is not a full 3D engine.

---

## Next evolution direction

The natural next steps are:

- richer shell blueprint types
- more advanced module behaviors
- stronger execution visualization
- improved HUD instrumentation
- stronger scanner identity and effects
- stricter runtime validation and debug tooling
- cleaner world-to-computation mapping

---

## Summary

Synth Grid Engine is a blueprint-driven, deterministic simulation runtime where 2D truth is projected into 3D-feeling space.

It is lightweight, modular, reproducible, and built around the idea that **geometry itself can be the executable structure**.
