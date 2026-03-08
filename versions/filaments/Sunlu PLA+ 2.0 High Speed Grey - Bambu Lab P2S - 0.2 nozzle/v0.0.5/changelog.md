# Changelog

## v0.0.5

### Changes
- Increased **Nozzle (First layer)** from `215°C` to `220°C`.
- Increased **Nozzle (Other layers)** from `215°C` to `220°C`.

### Reasoning
- In `v0.0.4`, a temperature tower was printed with all heat-creep mitigations active (bed at 55°C, 4cm glass riser open, 100% min fan speed from layer 1, P2S default retraction). Under these cooler ambient conditions the results clearly shifted:
  - **220°C**: Best — no bridge issues, no stringing, crisp details.
  - **225°C**: Very minor bridge issues and barely visible stringing — close second.
  - **210°C**: Slight stringing begins — acceptable third.
  - **≤205°C**: Noticeable detail degradation and worsening stringing.
  - **195°C**: Severe oozing and bridge failures.
- The original 215°C optimum (found in v0.0.1) was established in a warmer enclosure (bed at 60°C, no glass riser, fewer fan layers). The cooler environment created by v0.0.4's mitigations means the plastic now needs +5°C to reach the same melt quality.
- Using the same temperature for first layer and other layers, consistent with the approach established in v0.0.2.
- No other settings are changed — this is a focused single-variable update.
- **Next steps**: Proceed to Flow Rate and Pressure Advance calibrations.
