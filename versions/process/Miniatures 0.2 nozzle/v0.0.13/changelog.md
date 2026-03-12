# Changelog (v0.0.12 -> v0.0.13)

## Process: Miniatures 0.2 nozzle

*   **Rock Solid Support Stability**
    *   **Perimeter Scaffolding**:
        *   Set `Support critical regions only` to `No`. This adds a robust perimeter of supports around the tilted base, providing much-needed structural integrity for the "diving board" geometry.
    *   **Branch Rigidity**:
        *   Increased `Support wall loops` from `1` to `2`. This doubles the wall thickness of the tree support branches, making them significantly stiffer and preventing the "wobbling" or "flexing" that caused the base to move during nozzle passes.
    *   **Solid Cradle**:
        *   Reduced `Top interface spacing` from `0.8 mm` to `0.0 mm`. This creates a solid "roof" of plastic for the miniature to sit on, providing superior adhesion and ensuring a cleaner release (peeling off as a sheet).
    *   **Increased Support Density**:
        *   Reduced `Tree support branch distance` from `4 mm` to `2 mm`. This doubles the number of support branches reaching up to the base, distributing the weight and impact forces across more points.

## Notes
* Version 0.0.13 focuses on the mechanical root cause of the "moving base" failure. By stiffening the branches (2 loops) and providing a continuous solid shelf (0mm spacing), the miniature should remain perfectly stationary even with the 45-degree leverage.
* We keep the `Tip diameter` at `0.5 mm` to avoid marking the actual miniature, as the stiffer branches provide the necessary stability.
