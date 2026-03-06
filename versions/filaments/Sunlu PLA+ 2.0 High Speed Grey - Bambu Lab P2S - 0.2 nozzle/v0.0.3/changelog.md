# Changelog

## v0.0.3

### Changes
- Changed **Max volumetric speed** from `5mm³/s` to `2mm³/s`.

### Reasoning
- In version `v0.0.2`, the extruder got stuck during the print and required cold pulls to unlock and clean the nozzle. 
- A lower max volumetric speed allows the extruder slightly more time to melt the filament uniformly before pushing it out of the tiny 0.2mm nozzle, preventing the extruder gears from stripping or jamming from excessive backpressure. By locking the max volumetric speed to `2mm³/s`, it drastically reduces strain inside the nozzle.
- **Next steps**: Do a test print with these settings to confirm the extruder no longer jams and that the stringing remains controlled at 215°C with the new volumetric speed constraint. After that, perform Flow Rate and PA calibrations.
