# Changelog

## v0.0.7

### Changes
- Updated **No cooling for the first** from `1` to `4` layers.
- Updated **Full fan speed at layer** from `0` (disabled) to `10`.
- Updated **Auxiliary part cooling fan speed** from `70%` to `35%`.

### Reasoning
- In `v0.0.6`, sub-1mm support structures were getting swept away during miniature prints.
- Two fans are responsible:
  - The **auxiliary fan** (side-mounted) blows horizontally across the plate at a constant 70% from layer 2 onward — the most likely culprit for toppling tiny support stubs.
  - The **part cooling fan** (head-mounted) was also jumping to 100% immediately after the first no-cooling layer.
- `No cooling for the first` raised from `1` to `4`: delays both fans entirely for the first 4 layers, giving tiny support structures time to solidify and adhere before any airflow hits them.
- `Full fan speed at layer` set to `10`: the part cooling fan now ramps linearly from 0% (at layer 5) up to 100% by layer 10, instead of jumping to full speed instantly.
- `Auxiliary fan speed` reduced from `70%` to `35%`: the aux fan cannot be ramped natively in OrcaSlicer — it always jumps to its set speed when cooling activates. Halving the speed significantly reduces the lateral force on small features when it does kick in.
- **Note**: Per OrcaSlicer documentation, the auxiliary fan is explicitly disabled during the layers defined by `No cooling for the first`, making this the correct and supported mechanism to delay it.
- **Next steps**: Validate on a miniature with small support structures. If supports still get swept, consider reducing aux fan further or extending the no-cooling zone to 6 layers.
