# Changelog (v0.0.11 -> v0.0.12)

## Process: Miniatures 0.2 nozzle

*   **Safety & Stability (The "Flying Miniature" Fix)**
    *   **Travel Speed Control**:
        *   Reduced `Travel speed` from `600 mm/s` to `400 mm/s`. Lowering the travel speed reduces the kinetic energy during any minor nozzle-to-print clips, helping prevent miniatures from being knocked off while maintaining reasonable print times.
    *   **Support Interface Stability**:
        *   Decreased `Top interface spacing` from `1.0 mm` to `0.8 mm`. This provides a slightly denser support roof for the 45-degree tilted miniature to rest on, increasing stability without significantly impacting removal difficulty.
    *   **XY Clearance Adjustment**:
        *   Increased `Support/object XY distance` from `0.5 mm` to `0.65 mm`. The previous 0.5mm setting was found to be too tight for the 0.2mm nozzle, increasing collision risk on tilted models.


## Notes
* Version 0.0.12 focuses on the mechanical causes of the "flying miniature": travel momentum and tight XY clearances. By reducing the travel speed and easing the XY gap, we provide more safety margin for 45-degree tilted prints.
