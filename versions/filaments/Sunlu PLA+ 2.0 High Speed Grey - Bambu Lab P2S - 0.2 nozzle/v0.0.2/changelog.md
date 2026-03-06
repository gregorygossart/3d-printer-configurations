# Changelog

## v0.0.2

### Changes
- Changed **Nozzle (First layer)** from `200°C` to `215°C`.
- Changed **Nozzle (Other layers)** from `195°C` to `215°C`.

### Reasoning
- Based on the temperature tower test from v0.0.1, the filament performs best at 215°C. It offers the best compromise between preserving printed details and maintaining tight bridges (ceiling) on overhangs, without the significant stringing seen at higher temperature. 
- Removed the +5°C offset for the first layer that was present in the original ObscuraNox profile. It is typical to just run the same constant temperature across all layers unless there are specific adhesion issues.
- **Next steps**: With the optimal temperature found, Flow Rate and Pressure Advance calibrations will need to be performed on top of this.
