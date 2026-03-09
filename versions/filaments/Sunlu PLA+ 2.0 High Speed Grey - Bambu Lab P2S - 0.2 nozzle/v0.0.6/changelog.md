# Changelog

## v0.0.6

### Changes
- Updated **Flow ratio** stays at `1.0`.
- Updated **Enable pressure advance** from `No` to `Yes`.
- Updated **Pressure advance** from `0` to `0.225`.
- Added **Setting Override — Retraction Length**: `0.4mm`.
- Added **Setting Override — Retraction Speed**: `30mm/s`.
- Added **Setting Override — Wipe while retraction**: `Yes`.
- Added **Setting Override — Long retraction when cut (beta)**: `Yes`.
- Added **Setting Override — Retraction distance when cut**: `18`.

### Reasoning
- In `v0.0.5`, four calibration tests were performed now that the temperature was stabilized at 220°C:
  - **Max Volumetric Speed**: Tested 1–4 mm³/s in 0.10 steps. Results looked perfect at every height. Kept at default `2 mm³/s` — no reason to push higher for this use case.
  - **Pressure Advance**: Optimal result fell between `0.2` and `0.25`. Chosen value: `0.225`. This replaces the previous estimate of `0`, which was not calibration-tested.
  - **Flow Rate**: Dozens of tests across `0.95–1.05`. With PA correctly set, all values produced excellent results with almost no underextrusion. Choosing `1.0` (default) as values were effectively indistinguishable to the naked eye.
  - **Retraction**: Stringing stopped at `0.2mm`. A safe margin of `0.4mm` was chosen. Retraction speed explicitly set to `30mm/s`, and wipe while retraction enabled for cleaner travel moves.
- These overrides are applied at the filament level to make them apply consistently regardless of the process profile used.
- **Next steps**: Validate these calibration settings with a real print (e.g. a miniature).
