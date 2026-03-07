# Changelog

## v0.0.4

### Changes
- Decreased **Bed temperature** on PEI Plates from `60°C` to `55°C` to limit heat radiating up from the bed.
- Decreased **Cool Plate (SuperTack)** first layer temperature from `50°C` to the default `45°C` to further reduce ambient heat for the initial layer.
- Reverted **No cooling for the first [X] layers** from `4` back to the default `1` layer to start actively fighting ambient heat earlier in the print.
- Reverted **Max fan speed threshold** layer time from `8s` to the default `4s`.
- Increased **Min fan speed threshold** from `80%` to `100%` to maximize heat dissipation from the plastic and hotend since miniature prints run extremely slow (all layer times take > 80s).
- Removed **Retraction overrides** (previously `Length: 0.8mm`, `Z-hop: 0.8mm`, `Z-hop type: Spiral` inherited from a Bambu A1 open-air profile). Now using P2S defaults: `0.4mm / 0.4mm / Auto`. Halving retraction length significantly reduces the amount of hot plastic dragged up into the heatbreak on each retraction move, directly reducing heat creep risk.

### Reasoning
- In `v0.0.3`, the high speed filament experienced heat creep, softening prematurely and causing the extruder gear to slip and clog. 
- The printing speed for these miniatures using a 0.2mm nozzle is extremely slow (between 30 and 150mm/s). Lowering the bed to 55°C reduces ambient heat near the hotend/extruder, reducing the risk of heat creep without losing PEI plate adhesion capabilities.
- Opening the printer door or removing the top glass will be the primary method for eliminating heat build-up inside the chamber.
- Setting the uncooled layers back to 1 and enforcing a 100% part cooling fan speed regardless of layer time actively pushes hot air away from the melted plastic and heatbreak at all times.
- Will also print a top glass riser so that it goes up about 4cm and can easily be opened: https://makerworld.com/en/models/1924371-p2s-riser-ams-flipper
