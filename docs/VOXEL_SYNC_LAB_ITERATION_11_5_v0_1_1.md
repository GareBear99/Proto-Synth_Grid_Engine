# Voxel Sync Lab — Iteration 11.5 v0.1.1

`Iteration11.5/voxel_sync_lab.html` is the named public demo entrypoint for the Iteration 11.5 synchronized voxel lab.

## What it demonstrates

Voxel Sync Lab locks five UI/runtime surfaces to one canonical state spine:

1. Voxel Grouping View
2. Cube Matrix
3. Micro ARC-Room / Mesh Intake Lab
4. Stonewalker-style entity set
5. Entity Neural Synth matrix

The current v0.1.1 package preserves the screenshot-aligned layout: macro tiles on the left, room/lab viewport in the center, cube matrix and inspector on the right, neural matrix and command/event logs along the bottom.

## Canonical ID rule

Every selected tile controls the matching room, cube, neural matrix, registry entry, and entity cluster.

```text
tile_0015 -> room_0015 -> cube_0015 -> neural_0015
```

The package is local-first and runs by opening the HTML directly.

## Public-facing package status

- Version: `0.1.1`
- Iteration: `11.5`
- Demo name: `Voxel Sync Lab`
- Entrypoints:
  - `Iteration11.5/index.html`
  - `Iteration11.5/voxel_sync_lab.html`
- Screenshot:
  - `Iteration11.5/images/voxel_sync_lab_iteration_11_5_current.jpeg`
- Scene schema:
  - `Iteration11.5/scene_schema.json`
- Manifest:
  - `Iteration11.5/package_manifest_v0.1.1.json`

## Not production backend

This is a public prototype UI/runtime foundation, not a completed simulation backend. It is ready for repo presentation, demo use, and next-stage integration.
