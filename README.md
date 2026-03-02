# 3D Printing Configuration Tracker

This project is designed to help you find the perfect 3D printing configuration through iterative improvements.

## Folder Structure

- `templates/`: Contains the base markdown files for your configurations and feedback.
- `vX.Y.Z/`: Versioned folders containing your specific settings.
  - `printer.md`: Your printer hardware setup.
  - `filament.md`: Material-specific settings.
  - `process.md`: Slicer and print-specific settings.
  - `prints/`: Records of individual prints using this configuration.

## Versioning Rules

We use a `Semantic Versioning` inspired approach:

- **Z (Patch)**: `v0.0.1` -> `v0.0.2`. Any minor change to a configuration file.
- **Y (Minor)**: `v0.0.2` -> `v0.1.0`. A version that has been **validated** by a successful, high-quality print.
- **X (Major)**: `v0.1.0` -> `1.0.0`. Reserved for when you consider a configuration "Perfect" or a stable baseline.

## Workflow

1. **Start a new version**: Copy the previous version's files or templates into a new `vX.Y.Z` folder.
2. **Tweak settings**: Modify `printer.md`, `filament.md`, or `process.md`.
3. **Print**: Run a test print.
4. **Log Feedback**: Create a new folder in `prints/` (e.g., `print_20240101_1200/`) and fill out `feedback.md`.
5. **Analyze**: Use the feedback to decide the next increment.

## Feedback

When providing feedback (text or photos), fill out the `feedback.md` in the respective print folder. Be sure to check the box if the print was better than the previous one!
