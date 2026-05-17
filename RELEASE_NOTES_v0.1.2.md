# Release Notes — Voxel Sync Lab Iteration 11.5 v0.1.2

This package updates the Proto-Synth Grid Engine documentation to explain the Iteration 11.5 architecture clearly and publicly.

## Updated

- Root `README.md` now explains the Voxel Sync Lab Iteration 11.5 role.
- `Iteration11.5/README.md` now documents the micro tile room model.
- Added ARC-Room as the tactical mesh object intake / micro-room prototyping lab reference.
- Added the border linking authority gate doctrine for bringing down walls between adjacent micro rooms only when authority allows it.
- Added `docs/VOXEL_SYNC_LAB_ITERATION_11_5_v0_1_2.md`.
- Added `Iteration11.5/package_manifest_v0.1.2.json`.

## Core doctrine

```text
tile_id == room_id == cube_id == neural_id
```

No independent tiles. Every macro tile, Cube Matrix cell, ARC-Room-style viewport, mesh entity set, Neural Synth dot cluster, and border gate routes through the same canonical ID spine.

## ARC-Room reference

ARC-Room is the tactical mesh lab repo used to prototype the micro tile room layer:

- https://github.com/GareBear99/ARC-Room

## Status

This is still a standalone prototype/demo foundation, not a completed backend. It is packaged for public repo presentation and next-stage integration work.
