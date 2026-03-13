# Changelog (v0.0.7 -> v0.0.8)

## Filament: Sunlu PLA+ 2.0 High Speed Grey

*   **Extrusion Control & Precision**
    *   **Calibrated Pressure Advance**:
        *   Updated `Pressure advance` from `0.225` to `0.25` based on calibration. This aims to resolve "spikes" or blobs seen at the borders/turns, especially in the second half of complex prints.
*   **Cooling & Slow Printing**
    *   **Reduced Minimum Speed**:
        *   Reduced `Min print speed` from `20 mm/s` to `10 mm/s`. This allows the slicer to slow down even more for extremely small features, ensuring better cooling and layer bond for tiny details.

## Notes
* These changes are specifically targeted at improving detail fidelity and reducing artifacting (spikes) on the borders of the miniature.
* The Pressure Advance value of 0.25 should provide cleaner corners and stops.
