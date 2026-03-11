# Changelog (v0.0.5 -> v0.0.6)

## Process: Miniatures 0.2 nozzle

* **Support**
    * **Advanced**:
        * Decreased `Support wall loops` from `2` to `1` (Reducing from the rigid double-wall trunks of v0.0.5 to a single wall should make branches significantly easier to break and remove while still providing more stability than the 0 walls of v0.0.4).
        * Increased `Top Z distance` from `0.18 mm` to `0.24 mm` (Provides exactly 4 layers of gap at 0.06mm layer height, ensuring a cleaner break-away than the previous 3 layers).
        * Decreased `Top interface layers` and `Bottom interface layers` from `3 layers` to `2 layers` (Thinner interface layers are easier to peel away and reduce the total contact area that can fuse).
        * Increased `Support/object XY distance` from `0.7 mm` to `1.5 mm` (Maximum clearance to force branches to take a wide detour around delicate parts).
        * Increased `Threshold angle` from `40°` to `50°` (Reduces unnecessary branches by only supporting more extreme overhangs).
        * Increased `Top interface spacing` from `0.8 mm` to `1.2 mm` (Makes the connection points even sparser for a "hair-thin" bond, reducing fusion on bottom surfaces).
    * **Tree supports**:
        * Decreased `Tip diameter` from `0.6 mm` to `0.5 mm` (Smaller contact points).
        * Decreased `Tree support branch diameter` from `1.2 mm` to `1.1 mm` (A lean diameter that still offers enough rigidity to prevent wobbling during high-speed printing).
        * Decreased `Branch diameter angle` from `4°` to `2°` (A subtle taper that provides stability at the base without creating a crowded "forest" effect).
        * Increased `Tree support branch distance` from `2 mm` to `4 mm` (Prevents branch merging).
        * Decreased `Branch density` from `30%` to `20%` (Reduces the overall density of the support structure to make it less "solid" and easier to extract parts).

## Notes
* The main focus of this version is addressing the "too strong" supports of v0.0.5 that caused breakage on thin parts like spears and legs. By reducing the wall count, density, and increasing the distances, we aim to maintain successful geometry support while drastically improving ease of removal.
