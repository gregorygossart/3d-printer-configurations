# Changelog (v0.0.9 -> v0.0.10)

## Process: Miniatures 0.2 nozzle

*   **Support**
    *   **Foundation (Inspiration from stable v0.0.5)**:
        *   Increased `First layer expansion` from `2 mm` to `5 mm`. 
        *   Increased `First layer density` from `90%` to `100%`.
        *   Reverted `Branch diameter angle` to `4°` (from v0.0.9's `2°`). Version 0.0.5 used this wider angle to create a pyramid-shaped base, which is much sturdier for tall miniature supports and likely would have prevented the tip-over failure in v0.0.9.
    *   **Internal Strength**:
        *   Increased `Branch density` from `15%` to `20%`. While 15% was easy to remove, it might have been too hollow to survive high-speed moves. 20% is a safe middle ground.
        *   Slightly increased `Tree support branch diameter` to `1.2 mm`.

## Notes
* By looking back at v0.0.5 (which was stable but too close to the model) and v0.0.9 (which had great clearance but fell over), we've engineered v0.0.10 to take the best of both. We are keeping the wide support clearances and "Make overhangs printable" logic, but restoring the v0.0.5 "sturdy base" geometry and 100% foundation density.
