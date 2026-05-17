# I/O SYNTH GRID ENGINE

<p align="center">
  <img src="geometry-synth-banner.svg" alt="Synth Grid Engine animated geometry banner" width="100%" />
</p>

<p align="center"><strong>Deterministic 2D simulation. Projected to feel visually 3D.</strong><br><strong>Blueprint geometry becomes computation.</strong></p>

<p align="center">
  <a href="https://github.com/GareBear99/Synth-Grid-Engine/issues"><img alt="Issues" src="https://img.shields.io/github/issues/GareBear99/Synth-Grid-Engine?style=for-the-badge"></a>
  <a href="https://github.com/GareBear99/Synth-Grid-Engine/discussions"><img alt="Discussions" src="https://img.shields.io/github/discussions/GareBear99/Synth-Grid-Engine?style=for-the-badge"></a>
  <a href="https://github.com/GareBear99/Synth-Grid-Engine/stargazers"><img alt="Stars" src="https://img.shields.io/github/stars/GareBear99/Synth-Grid-Engine?style=for-the-badge"></a>
  <a href="https://github.com/GareBear99/Synth-Grid-Engine/network/members"><img alt="Forks" src="https://img.shields.io/github/forks/GareBear99/Synth-Grid-Engine?style=for-the-badge"></a>
</p>

<p align="center">
  <a href="https://github.com/sponsors/GareBear99"><img alt="GitHub Sponsors" src="https://img.shields.io/badge/Sponsor-GitHub-ea4aaa?style=for-the-badge&logo=githubsponsors"></a>

</p>

## 🔐 Built on ARC-Core

> **[ARC-Core](https://github.com/GareBear99/ARC-Core)** is the authority / event / receipt kernel that this engine is built on. Every grid mutation, module attachment, blueprint load, and execution step is an ARC-Core-shaped event with a receipt. The engine's deterministic-simulation guarantee derives from ARC-Core's event-sourcing discipline.

| Engine layer | ARC-Core pattern |
|---|---|
| Blueprint loading (shell / module) | Signed receipt per load — blueprint hash bound to receipt |
| Grid mutations (cell, actor, layer) | Append-only event log |
| Module attachment (ship / scanner / HUD) | Authority-gated events |
| Deterministic simulation loop | Replay state by re-applying the event log |
| Save/load files | Event log + snapshot, receipt-verified on load |
| Voxel Directory + Neural-Synth sync | Shared event chain between both subsystems |
| Audit trail | `ARC_CORE_AUDIT_v44.txt` and iteration audits track receipt lineage |

Related ARC repos:

- [ARC-Core](https://github.com/GareBear99/ARC-Core) — authority / event / receipt kernel *(backbone of this engine)*
- [Seeded-Universe-Recreation-Engine](https://github.com/GareBear99/Seeded-Universe-Recreation-Engine) — sibling seed-first simulation project on the same backbone
- [arc-lucifer-cleanroom-runtime](https://github.com/GareBear99/arc-lucifer-cleanroom-runtime) — deterministic kernel direction
- [ARC-Neuron-LLMBuilder](https://github.com/GareBear99/ARC-Neuron-LLMBuilder) — governed AI build loop (same author, same doctrine)

## What this is

Synth Grid Engine is a math-first world runtime where shell geometry, module layout, and deterministic execution all share the same blueprint-driven foundation.

Instead of treating geometry as decoration, the engine treats it as structure, storage, routing, and execution space. The world itself becomes a programmable surface.

This project is built around a **deterministic 2D simulation core** with a **visually 3D projection layer**. That keeps the runtime lightweight, reproducible, and portable while still delivering a high-contrast synthwave spatial feel.

## Iteration 0 — Synth Shell #0
![Example](images/Image0.jpeg)
- Lucipher Synth #0
## Core idea

The engine loads blueprints that define how the world behaves.

### 1) Shell Blueprint
Defines the geometry of the world.

### 2) Module Blueprints
Attach systems into the shell.

### 3) Execution Layer
Runs the deterministic simulation loop.

**Geometry = storage**  
**Movement = computation**  
**Entities = executors**

## Why it is different

- **Math-first, not graphics-first**
- **Deterministic worlds from seed and blueprint state**
- **2D simulation core with visually 3D presentation**
- **Low CPU footprint on older hardware**
- **Modular runtime architecture instead of a fixed one-off application**
- **Designed as an engine surface for future systems, not just a demo**

## Iteration path

## Iteration 8 — Blueprint Shell Prototyping

![Iteration 8 Example World](images/Image1.jpeg)
- Shell Synth

Included example blueprint: `blueprint_octagon.json`

Builds an octagon shell structure where modules can attach.

## Iteration 9 — Game Engine Prototype

<details>
<summary>Click to expand Iteration 9 prototype</summary>

![Synth Grid Engine Prototype](images/Image2.jpeg)

This prototype demonstrates:

- blueprint shell generation
- cube-grid projection mapping
- deterministic seed worlds
- modular system attachment
- spatial execution visualization

The runtime supports loading:

- Shell Blueprints
- Ship Modules
- Scanner Modules
- HUD Modules

</details>

## Iteration 10 — Synth Grid Engine

![Iteration 10 Demo](images/Image3.jpeg)
- Lucid Terminal Master Control Synth #1

A blueprint-driven simulation shell where geometry becomes computation.

This engine is experimental by design, but the direction is serious: modular world runtime, blueprint-authored structure, deterministic simulation, and portable execution.

## Iteration 11 — NEURAL-SYNTH / wetware core / runtime v0.1

![Iteration 11 Demo](images/Image4.jpeg)

## Math-first simulation

All core logic runs in deterministic 2D vector space.

The render layer then projects that simulation into a visually 3D environment using techniques like:

- perspective scaling
- layered sprite depth
- cube-grid projection
- depth shading
- shell geometry overlays

That gives the engine a 3D-feeling spatial surface without requiring a heavyweight full-3D stack.

## NEURAL-SYNTH / wetware core / runtime v0.2

![Iteration 11 Demo](images/Image5.jpeg)


## Voxel Directory

![Iteration 11 Demo](images/Image6.jpeg)

Fully RGB Customizeable with both way reproducible seed, also both 'Voxel Directory' and 'Neural-Synth' are in sync. 

## Controls

| Key | Action |
|---|---|
| `W A S D` | Move master control |
| `Mouse` | Aim vector |
| `C` | Toggle reticle |
| `` ` `` | Toggle debug overlay |
| `R` | Reset |

## Running the engine

1. Download or clone the repository.
2. Open `index.html` in a browser.
3. Load blueprints through the runtime UI.

No server required.

## Recommended load order

1. Shell blueprint  
2. Ship module  
3. Scanner module  
4. HUD module (optional)

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

## Contributing

Ideas, bug reports, architecture suggestions, and module experiments are welcome.

- Open an **Issue** for bugs or concrete work
- Use **Discussions** for ideas, design direction, or architecture talk
- Open a **Pull Request** for improvements

Read [CONTRIBUTING.md](CONTRIBUTING.md) before sending major changes.

## Support the project

If you want to help push this engine further:

- **GitHub Sponsors:** `https://github.com/sponsors/GareBear99`
- **Buy Me a Coffee:** replace the placeholder in this README and in `.github/FUNDING.yml`

Support helps with development time, testing, visuals, documentation, and future releases.

## Community links

- **Issues:** `https://github.com/GareBear99/Synth-Grid-Engine/issues`
- **Discussions:** `https://github.com/GareBear99/Synth-Grid-Engine/discussions`
- **Pull Requests:** `https://github.com/GareBear99/Synth-Grid-Engine/pulls`
- **Releases:** `https://github.com/GareBear99/Synth-Grid-Engine/releases`

## Repo setup checklist

- Enable **Issues**
- Enable **Discussions**
- Add repo **Topics**
- Add a **Description** and **Website** if relevant
- Upload a strong **Social Preview Image**
- Create the first **Release**
- Pin one **Discussion** for roadmap / ideas
- Add repo **Topics** like `html5`, `javascript`, `deterministic-simulation`, `synthwave`, `game-engine`, `procedural`, `2d`, `3d-illusion`

## License

![Polygon](images/Polygon.jpg)



## Voxel Sync Lab — Iteration 11.5 v0.1.2

The repository now includes **Voxel Sync Lab**, the Iteration 11.5 public-facing bridge between Proto-Synth Grid Engine, Voxel Grouping, Cube Matrix, Stonewalker-style tactical mesh entities, Neural Synth dot matrices, and **ARC-Room** micro-room prototyping.

Run directly:

- `Iteration11.5/index.html`
- `Iteration11.5/voxel_sync_lab.html`

No server, install step, build step, API key, or dependency is required.

### Iteration 11.5 role

Iteration 11.5 turns each visible voxel tile into a synchronized **micro tile room**. A tile is no longer just a visual card or grid cell. It is a small room/lab slot with a canonical identity shared across every runtime surface:

```text
tile_id == room_id == cube_id == neural_id
```

When a user selects `tile_0015`, the same selection resolves to:

```text
tile_0015
room_0015
cube_0015
neural_0015
```

That lock propagates through:

- Voxel Grouping View
- Cube Matrix
- Micro ARC-Room / Mesh Intake Lab viewport
- Stonewalker-style mesh entities
- Entity Neural Synth matrix
- Inspector
- Tile Registry
- Command Log
- Scene JSON receipt export

The hard rule is: **no independent tiles**. Every macro tile, cube matrix cell, micro-room viewport, mesh entity set, neural dot cluster, and border gate routes through the same canonical ID spine.

### Micro tile room role

Each micro tile is a tactical room/lab instance. The micro tile room is where objects, entities, mesh actors, markers, and future room-to-room links live.

The design target is:

```text
Voxel Grouping Tile
└── Micro Tile Room
    ├── ARC-Room style object intake
    ├── local mesh/object state
    ├── Stonewalker-style entities
    ├── per-entity Neural Synth dots
    ├── room border gates
    └── exportable scene receipt
```

### ARC-Room as the micro-room prototyping lab

**ARC-Room** is the tactical mesh lab repo used to prototype the micro tile room layer:

- https://github.com/GareBear99/ARC-Room

ARC-Room is the source direction for the object intake/lab behavior that gets embedded into each micro tile. Its role in the Voxel Sync Lab roadmap is to define the room-level workflow:

- upload or spawn mesh/object data
- inspect object transforms
- normalize scale
- duplicate or despawn objects
- show wire/bounds views
- save/load local room state
- export JSON scene state
- drive room operations through commands

In Voxel Sync Lab, this becomes the embedded room inside each voxel tile. Selecting a tile selects its ARC-Room-style micro lab. Selecting a cube selects the same room. Selecting an entity selects a live object/agent inside that room.

### Stonewalker tactical mesh role

The Stonewalker-style layer provides the live tactical mesh/entity side of the room. Inside a micro tile, entities act as mesh agents, object actors, scanners, repair nodes, intake markers, or simulation points.

Each entity can carry:

- `entity_id`
- `tile_id`
- local room position
- role label
- behavior mode
- tracking state
- selected state
- neural matrix link

This is why the Iteration 11.5 viewport uses the tactical mesh lab look: grid floor, wire objects, entity labels, selection rings, command log, and scanner-like state feedback.

### Neural Synth matrix role

The Entity Neural Matrix is the live explanation layer for the selected room/entity set. Dots represent local neural, semantic, signal, or behavior nodes. Lines represent communication between those nodes.

The purpose is to make each room feel like a small thinking system instead of a static viewport:

```text
Entity
├── mesh/body/object state
├── room position
├── behavior role
└── neural dots + communication edges
```

### Cube Matrix role

The Cube Matrix is the synchronized index/control grid. It does not own separate state. It mirrors the same tile IDs used by the Voxel Grouping View and micro rooms.

Selecting `cube_0008` selects:

```text
tile_0008 -> room_0008 -> cube_0008 -> neural_0008
```

This makes the Cube Matrix a compact authority/index layer for navigating the room grid.

### Border linking authority gates

Iteration 11.5 introduces the doctrine for **border linking authority gates**.

Each micro tile has borders. Those borders can be locked, linked, pending, rejected, opened, or sealed. A border gate controls whether one micro room is allowed to connect to a neighboring room:

```text
tile_0004 east  -> tile_0005 west
tile_0008 south -> tile_0012 north
```

When authority allows the connection, the wall between rooms can be lowered, visually opened, or merged into a shared passage. This lets the voxel grid become a linked tactical mesh environment instead of isolated boxes.

Border gates should eventually support:

- locked wall
- authorized link
- pending link
- rejected link
- open passage
- sealed passage
- shared entity crossing
- shared neural communication
- JSON receipt of the authority decision

The purpose of the border gate system is to **bring down walls only when authority allows it**. This keeps room linking deterministic, inspectable, and receipt-ready instead of becoming arbitrary UI state.

### Public-facing status

Voxel Sync Lab is currently a standalone Iteration 11.5 prototype/demo foundation. It is ready for repository presentation, local testing, screenshots, documentation, and next-stage integration with the broader Proto-Synth Grid Engine and ARC-Room workflows.

Docs:

- `Iteration11.5/README.md`
- `docs/VOXEL_SYNC_LAB_ITERATION_11_5_v0_1_2.md`
- `RELEASE_NOTES_v0.1.2.md`

