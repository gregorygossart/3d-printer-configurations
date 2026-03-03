# Changelog (v0.0.3 -> v0.0.4)

## Process: Miniatures 0.2 nozzle

* **Quality**
    * **Walls and surfaces**:
        * Changed `Avoid crossing walls` from `No` to `Yes` (To combat the oozing issue under the chin and on the wings by forcing travel movements to stay inside the already printed parts, reducing open-air drooling).
* **Support**
    * **Advanced**:
        * Increased `Top interface spacing` from `0.5 mm` to `0.8 mm` (To weaken the bond between the support interface and the model. Spacing out the interface lines will give less surface area for the tail to melt into, making peeling much easier).
    * **Tree supports**:
        * Decreased `Tree support branch diameter` from `1.5 mm` to `1 mm` (To make the branches thin and crushable again, preventing them from swallowing delicate 0.2mm details like weapons. `Avoid crossing walls` should now mitigate mid-print snapping).
        * Increased `Tree support branch distance` from `1 mm` to `2 mm` (To force tree branches to stay further apart from one another, preventing them from fusing into uncrushable clusters around delicate parts like the weapons).
