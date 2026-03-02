# Process Configuration

Configured for printer: [Bambu Lab P2S](../versions/printers/Bambu%20Lab%20P2S/v0.0.1/printer.md)
Configured for nozzle: 0.2mm
Configured for filament: [Sunlu PLA+ Grey](../versions/filaments/Sunlu%20PLA+%20Grey/v0.0.1/filament.md)

## Quality

### Layer height

- Layer height: 0.08 mm
- First layer height: 0.1 mm

### Line width

- Default: 0.22 mm
- First layer: 0.25 mm
- Outer wall: 0.22 mm
- Inner wall: 0.22 mm
- Top surface: 0.22 mm
- Sparse infill: 0.22 mm
- Internal solid infill: 0.22 mm
- Support: 0.22 mm

### Seam

- Seam position: Aligned
- Staggered inner seams: No
- Seam gap: 10%
- Scarf joint seam (beta): None
- Role base wipe speed: Yes
- Wipe speed: 80%
- Wipe on loops: No
- Wipe before external loop: No

### Precision

- Slice gap closing radius: 0.049 mm
- Resolution: 0.012 mm
- Arc fitting: Yes
- X-Y hole compensation: 0 mm
- X-Y contour compensation: 0 mm
- Elephant foot compensation: 0 mm
- Precise wall: Yes
- Precise Z height: No
- Convert holes to polyholes: No

### Ironing

- Ironing type: No ironing

### Wall generator

- Wall generator: Classic

### Walls and surfaces

- Walls printing order: Inner/Outer
- Print infill first: No
- Wall loop direction: Auto
- Top surface flow ratio: 1
- Bottom surface flow ratio: 1
- Set other flow ratios: No
- Only one wall on top surfaces: Yes
- One wall threshold: 300%
- Only one wall on first layer: No
- Avoid crossing walls: No
- Small area flow compensation (beta): No

### Bridging

- Bridge flow ratio: 1
- Internal bridge flow ratio: 1
- External bridge density: 100%
- Internal bridge density: 100%
- Thick external bridges: No
- Thick internal bridges: Yes
- Extra bridge layers (beta): Disabled
- Filter out small internal bridges: Filter
- Bridge counterbore holes: None

### Overhangs

- Detect overhang walls: Yes
- Make overhangs printable: No
- Extra perimeters on overhangs: No
- Reverse on even: No

## Strength

### Walls

- Wall loops: 4
- Alternate extra wall: No
- Detect thin walls: No

### Top/bottom shells

- Top shell layers: 7
- Top shell thickness: 0.8 mm
- Top surface density: 100%
- Top surface pattern: Monotonic
- Bottom shell layers: 5
- Bottom shell thickness: 0 mm
- Bottom surface density: 100%
- Bottom surface pattern: Monotonic
- Top/Bottom solid infill/wall overlap: 25%

### Infill

- Sparse infill density: 15%
- Fill Multiline: 1
- Sparse infill pattern: Gyroid
- Sparse infill direction: 45°
- Maximum length of the infill anchor: 20 mm
- Sparse infill anchor length: 400%
- Internal solid infill pattern: Monotonic
- Solid infill direction: 45°
- Apply gap fill: Nowhere
- Filter out tiny gaps: 0 mm
- Infill/wall overlap: 15%

### Advanced

- Align infill direction to model: No
- External bridge infill direction: 0°
- Internal bridge infill direction: 0°
- Minimum sparse infill threshold: 15 mm²
- Infill combination: No
- Detect narrow internal solid infill: Yes
- Ensure vertical shell thickness: All

## Speed

### First layer speed

- First layer: 40 mm/s
- First layer infill: 50 mm/s
- Initial layer travel speed: 100%
- Number of slow layers: 0 layers

### Other layers speed

- Outer wall: 60 mm/s
- Inner wall: 150 mm/s
- Small perimeters: 50%
- Small perimeters threshold: 0 mm
- Sparse infill: 100 mm/s
- Internal solid infill: 150 mm/s
- Top surface: 150 mm/s
- Gap infill: 50 mm/s
- Support: 150 mm/s
- Support interface: 80 mm/s

### Overhang speed

- Slow down for overhangs: Yes
- Slow down for curled perimeters: Yes
- Overhang speed (10%): 0 mm/s
- Overhang speed (25%): 60 mm/s
- Overhang speed (50%): 40 mm/s
- Overhang speed (75%): 20 mm/s
- Bridge (External): 50 mm/s
- Bridge (Internal): 150%

### Travel speed

- Travel: 600 mm/s

### Acceleration

- Normal printing: 4000 mm/s²
- Outer wall: 2000 mm/s²
- Inner wall: 0 mm/s²
- Bridge: 50%
- Sparse infill: 100%
- Internal solid infill: 100%
- First layer: 500 mm/s²
- Top surface: 2000 mm/s²
- Travel: 10000 mm/s²

### Jerk(XY)

- Default: 0 mm/s
- Outer wall: 9 mm/s
- Inner wall: 9 mm/s
- Infill: 9 mm/s
- Top surface: 9 mm/s
- First layer: 9 mm/s
- Travel: 12 mm/s

### Advanced

- Extrusion rate smoothing: 0 mm³/s²

## Support

### Support

- Enable support: No
- Type: Tree (auto)
- Style: Default (Grid)
- Threshold angle: 30°
- Threshold overlap: 50%
- First layer density: 90%
- First layer expansion: 2 mm
- On build plate only: No
- Ignore small overhangs: Yes

### Raft

- Raft layers: 0 layers

### Filament for Supports

- Support/raft base: Default
- Support/raft interface: Default

### Support ironing

- Ironing Support Interface: No

### Advanced

- Top Z distance: 0.08 mm
- Bottom Z distance: 0.08 mm
- Support wall loops: 0
- Base pattern: Default
- Base pattern spacing: 2.5 mm
- Pattern angle: 0°
- Top interface layers: 2 layers
- Bottom interface layers: 2 layers
- Interface pattern: Default
- Top interface spacing: 0.5 mm
- Bottom interface spacing: 0.5 mm
- Normal support expansion: 0 mm
- Support/object XY distance: 0.35 mm
- Support/object first layer gap: 0.2 mm
- Don't support bridges: No
- Independent support layer height: Yes

## Multimaterial

### Prime tower

- Enable: Yes
- Skip points: Yes
- Enable tower interface features: No
- Internal ribs: No
- Width: 60 mm
- Prime volume: 45 mm³
- Brim width: Auto
- Infill gap: 150%
- Wall type: Rectangle

### Ooze prevention

- Enable: No

### Flush options

- Flush into objects' infill: No
- Flush into objects' support: Yes

### Advanced

- Use beam interlocking: No
- Interface shells: No
- Maximum width of a segmented region: 0 mm
- Interlocking depth of a segmented region: 0 mm

## Others

### Skirt

- Skirt loops: 0
- Skirt type: Combined
- Skirt minimum extrusion length: 0 mm
- Skirt distance: 2 mm
- Skirt start point: -135°
- Skirt speed: 50 mm/s
- Skirt height: 1 layers
- Draft shield: Disabled

### Brim

- Brim type: Auto
- Brim width: 5 mm
- Brim-object gap: 0.1 mm
- Brim follows compensated outline: No

### Special mode

- Slicing Mode: Regular
- Print sequence: By layer
- Intra-layer order: Default
- Spiral vase: No
- Timelapse: Traditional
- Enable clumping detection: No

### Fuzzy skin

- Fuzzy skin: Disabled

### G-code output

- Reduce infill retraction: Yes
- Add line number: No
- Verbose G-code: No
- Label objects: Yes
- Exclude objects: No
- Filename format: `{input_filename_base}_{filament_type[0]}_{print_time}.gcode`

### Post-processing Scripts

- (None)
