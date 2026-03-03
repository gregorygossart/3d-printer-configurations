# Changelog (v0.0.2 -> v0.0.3)

## Process: Miniatures 0.2 nozzle

* **Support**
    * **Support**:
        * Decreased `Threshold angle` from `50°` to `40°` (To only generate supports for more critical overhangs, which should reduce the clutter and the number of supports trying to squeeze into hard-to-reach places like behind the belt or between the legs).
    * **Advanced**: 
        * Increased `Top Z distance` from `0.12 mm` to `0.18 mm` (To prevent support sections from melting/fusing with the miniature's delicate overhangs like the weapons. This is exactly 3 times the 0.06mm layer height).
        * Increased `Support/object XY distance` from `0.5 mm` to `0.7 mm` (To increase the gap between the supports and the sides of the model, preventing lateral fusion and making it easier to snap them off the flanks and legs).
    * **Tree supports**: 
        * Increased `Tree support branch diameter` from `1 mm` to `1.5 mm` (To make the branches slightly sturdier so they don't break during the print process).

## Notes
* **Stringing**: The stringing was mostly limited to the first 2-3mm between support trees. Since this doesn't impact the miniature's amazing details, no drastic changes to retraction or travel speed were made. Any adjustments to those might cause underextrusion on fine details.
* **Slicer Tip - Manual Supports**: If certain areas remain extremely difficult to reach (e.g., behind the belt), it might be better to selectively paint out support placement in Orca Slicer using the "Support Painting" tool to tell the slicer to ignore those specific crevices.
