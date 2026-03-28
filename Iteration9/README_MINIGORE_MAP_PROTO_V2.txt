MINIGORE MAP PROTOTYPE v2 (FULL-SPHERE BIOMES)
=============================================

Run:
- Open minigore_map_proto_v2.html
- Auto-loads the embedded octagon blueprint after ~250ms if you don't upload one.
- Optional: Upload HUD Module -> module_hud_minigore_mapshader_v2.json

What's new vs v1:
- FULL-SPHERE biome fill (all tiles, not just routeTiles).
- Biome borders (thicker outlines where biome changes) - same-face neighbors for stability/cheapness.
- Shoreline foam (beach tiles adjacent to ocean).
- Route overlay still visible on top.

Critical fix included:
- Initializes sh.pivotVerified at blueprint load (prevents black screen when blueprint becomes active).

Next steps to reach CubeWorld "stacked" look:
- Add height field -> draw cliff walls on biome/height transitions.
- Add water depth gradient + specular band.
- Add seam-aware neighbor lookup across cube face edges (for perfect borders).
- Add scanner-driven "focus biome" sky tint and bloom.

Controls:
- Upload Blueprint JSON: bring your own planet configs.
- Toggle Debug (D): see internal logs/seed.