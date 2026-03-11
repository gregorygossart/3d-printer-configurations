# Changelog (v0.0.8 -> v0.0.9)

## Process: Miniatures 0.2 nozzle

*   **Quality**
    *   **Overhangs**:
        *   Changed `Make overhangs printable` from `No` to `Yes`. This slightly alters the geometry of small overhangs to make them self-supporting, effectively eliminating the need for support material in those specific areas.
        *   Added `Make overhangs printable - Maximum angle` set to `55°`.
        *   Added `Make overhangs printable - Hole area` set to `0 mm²`.

## Notes
* By enabling `Make overhangs printable`, the slicer makes minor geometry modifications to unsupported edges (for example, small blue overhangs on the edges of the wings) so they can print perfectly on their own. This is a fantastic step because it drastically reduces the number of support trees generated and can help prevent stringing on those previously tricky small overhangs, without completely mutating the overall miniature model.
