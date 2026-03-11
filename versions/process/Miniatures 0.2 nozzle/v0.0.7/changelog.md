# Changelog (v0.0.6 -> v0.0.7)

## Process: Miniatures 0.2 nozzle

*   **Support**
    *   **Advanced**:
        *   Decreased `Top Z distance` from `0.24 mm` to `0.18 mm` (Goldilocks zone: Tight enough for good detail, loose enough for clean removal).
        *   Decreased `Support/object XY distance` from `1.5 mm` to `0.7 mm` (Reverted to the original distance that worked structurally in v0.0.5).
        *   Increased `Top interface layers` from `2` to `3` (Provides a more solid foundation for the model to land on).
        *   Decreased `Top interface spacing` from `1.2 mm` to `0.4 mm` (Dense enough to force the slicer to generate patterns, but sparse enough to avoid fusion).
        *   Changed `Interface pattern` to `Concentric` (A clean, smooth interface style).
        *   Added `Support critical regions only: No` and `Max bridge length: 0 mm` (Forces the slicer to stop filtering support geometry).
    *   **Tree supports**:
        *   Increased `Tip diameter` from `0.5 mm` to `0.6 mm` (Deliberately avoiding larger 1.2+ mm tips that trigger dense padding but ruin fine details. We rely purely on these point-contacts).
        *   Decreased `Tree support branch distance` from `4 mm` to `2 mm` (Clusters branches closer under large overhanging parts).
        *   Decreased `Tree support branch diameter` from `1.1 mm` to `1.1 mm` (Back to baseline).
    *   **Speed**:
        *   Decreased `Support speed` from `150 mm/s` to `120 mm/s` (Better stability for branches).
        *   Decreased `Support interface speed` from `80 mm/s` to `60 mm/s` (Higher precision on the critical connection layers).

## Notes
* This version abandons the attempt to force dense "Interface Pads" (dark green in the slicer). We learned that Orca Slicer requires a massive 1.2 mm tip diameter to generate pads on a 0.2 mm nozzle. Such large tips would fuse to delicate miniature features. Instead, this version relies completely on **Point Contacts**. The tiny 0.6 mm tips securely hold the details but snap away cleanly due to the carefully calibrated 0.18 mm `Top Z distance`.
