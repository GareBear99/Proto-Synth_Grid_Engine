# Voxel Sync Lab — Iteration 11.5 v0.1.2

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

## Included files

- `index.html`
- `voxel_sync_lab.html`
- `README.md`
- `CHANGELOG.md`
- `LICENSE`
- `scene_schema.json`
- `package_manifest_v0.1.2.json`
- `images/voxel_sync_lab_iteration_11_5_current.jpeg`

