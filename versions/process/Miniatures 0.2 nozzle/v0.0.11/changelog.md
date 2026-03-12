# Changelog (v0.0.10 -> v0.0.11)

## Process: Miniatures 0.2 nozzle

*   **Support**
    *   **Geometry Stability (The XY Fix)**:
        *   Decreased `Support/object XY distance` from `0.8 mm` to `0.5 mm`. This setting was experimentally found to resolve the issue where tree support trunks would fail to "close" or "cap" at the top. 
        *   At `0.5 mm` (2.5x the 0.2mm nozzle width), the trees can grow more vertically without needing complex detours. This keeps the merged "trunk bowls" small enough for the slicer to reliably generate a solid roof/cap, preventing the "floating branch" artifacts seen at higher clearances.

## Notes
* Version 0.0.11 incorporates the major discovery that a **0.5mm XY distance** is optimal for maintaining tree structural integrity on a 0.2mm nozzle. It provides enough gap to prevent fusion while ensuring the slicer can physically finish the support geometry.
* This version retains the reinforced foundation fixes (5mm expansion, 100% first layer density) and the successful `Make overhangs printable` setting.
