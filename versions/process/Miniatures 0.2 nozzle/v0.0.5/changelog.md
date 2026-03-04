# Changelog (v0.0.4 -> v0.0.5)

## Process: Miniatures 0.2 nozzle

* **Support**
    * **Advanced**:
        * Increased `Support wall loops` from `0` to `2` (By printing the tree branches with 2 perimeters instead of 1, the trunks become incredibly stiff and strong inwardly, preventing the snapping seen in v0.0.4 without expanding their outward size and risking fusion with the model).
    * **Tree supports**:
        * Increased `Tree support branch diameter` from `1 mm` to `1.2 mm` (A slight increase to prevent the extreme fragility of v0.0.4, but kept smaller than v0.0.3's 1.5mm so they don't overwhelm fine details).
        * Decreased `Branch diameter angle` from `5°` to `4°` (Reducing this ensures the trunks stay slim all the way down toward the build plate, avoiding massive chunks. The structural strength now comes from the double walls).

## Notes
* The `Avoid crossing walls` (`Yes`) and `Top interface spacing` (`0.8 mm`) settings from v0.0.4 have been carried over to continue addressing the oozing and tail fusing issues. The core strategy to prevent spaghetti is to reinforce the internal walls of the tree supports, allowing them to be both thin and extremely durable.
