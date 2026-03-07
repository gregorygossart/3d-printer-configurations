# Print Feedback

## Print Outcome
- **Success**: [ ] Yes / [x] No / [ ] Partial
- **Better than previous?**: [ ] Yes / [x] No / [ ] N/A

## Observations
- **Visual Quality**: N/A
- **Dimensional Accuracy**: N/A
- **Strength/Durability**: N/A
- **Issues Encountered**: The extruder keeps clogging. Normal PLA works fine, but High Speed filament conducts heat faster from the nozzle, softening the filament prematurely before it reaches the hotend. The extruder gear then fails to grip the soft filament correctly, causing a clog (Heat Creep). 
This especially happens because the current print speeds (30 - 150 mm/s) are much slower than the filament's recommended speeds (150–300 mm/s) for the current 215°C nozzle temperature, due to printing miniatures with a 0.2mm nozzle.

## Photos
<!-- Insert photo links here -->
No photos available.

## Notes
- Need to consider lowering the bed temperature (currently 60°C) and nozzle temperature (currently 215°C) to prevent the heat creep out of the hotend.
- Filament recommended 200–215°C for 50–150 mm/s speeds. Lowering the temp would help fit the miniature-printing speeds.
