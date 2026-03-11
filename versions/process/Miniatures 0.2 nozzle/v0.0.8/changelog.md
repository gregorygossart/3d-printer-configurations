# Changelog (v0.0.7 -> v0.0.8)

## Process: Miniatures 0.2 nozzle

*   **Support**
    *   **Advanced**:
        *   Changed `Support critical regions only` from `No` to `Yes`. This prevents the slicer from building large trees for tiny, non-critical overhangs that the printer can easily bridge.
        *   Changed `Ignore small overhangs` from `No` to `Yes`. This forces the generation algorithm to skip tiny droplet-like bumps on textures, reducing unneeded pillars.
        *   Increased `Top interface spacing` from `0.2 mm` to `1.0 mm`. The dense contact pad of v0.0.7 made removal very difficult. Spreading it to 1.0 mm creates a sparse connection that tears away effortlessly.
        *   Decreased `Normal support expansion` from `0.1 mm` to `0 mm`. This prevents the slicer from artificially widening the required support area over edges, keeping the support footprint tight.
        *   Increased `Support/object XY distance` from `0.4 mm` to `0.8 mm`. This is the primary fix for the "miniature engulfed by support" issue, providing a safer buffer so support walls do not cling to delicate parts.
        *   Changed `Max bridge length` from `0 mm` to `999 mm`. Setting this to 0 meant *all* bridges had to be supported. A large value effectively tells the slicer "don't support bridges," allowing parts like wings to self-support naturally again without massive columns.
    *   **Tree supports**:
        *   Decreased `Tip diameter` from `0.6 mm` to `0.5 mm`. Reduces the contact point further for easier snapping.
        *   Increased `Tree support branch distance` from `2 mm` to `4 mm`. Forces the tree trunks to stay separate and not cluster together into a thick cast around the miniature.
        *   Decreased `Branch density` from `25%` to `15%`. Hollows out the support structures internally, dramatically reducing their rigidity when crushing/bending them away from the miniature.

## Notes
* The previous version (v0.0.7) achieved great details, but the dense clustering (`0.2 mm` top interface spacing, `2 mm` branch distance, low `0.4 mm` XY distance, and `0 mm` max bridge length) wrapped a thick shell of plastic entirely around delicate thin pieces like spears and feet. Taking off this "cast" inherently breaks the thin pieces inside. By massively increasing the branch distance, ensuring we only generate support for critical regions/ignoring small overhangs, and adding more clearance horizontally, we aim to drastically reduce the sheer number of trees so parts snap off cleanly without threatening the print.
