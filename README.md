# UltraSmooth — Minecraft 1.21.11 (Fabric)

This is the first source-code scaffold for the UltraSmooth client-side optimization project.

## Included in this starter
- Fabric client mod entrypoint.
- Press **O** to open the UltraSmooth settings screen.
- Four prototype toggle controls.
- Hover tooltips that explain each setting.

## Important status note
The current switches are **UI scaffolding only**. They do not yet alter Minecraft rendering, chunk loading, particles, memory use, or FPS. Those optimizations must be implemented and benchmarked individually before they are advertised as working features. This starter is not yet a Sodium/OptiFine replacement or a release-ready performance mod.

## Requirements
- Minecraft Java Edition 1.21.11
- JDK 21
- Fabric Loader 0.18.1 or newer compatible with 1.21.11
- Fabric API 0.141.6+1.21.11
- Gradle 9.x (use a Gradle version supported by the selected Loom release)

## Build
From this folder, run:

```bash
gradle build
```

The remapped mod JAR will be created in `build/libs/`.

## Open the settings screen
Launch Minecraft with Fabric and this mod installed, then press **O**. The key can be changed in Minecraft's Controls menu under the UltraSmooth category.

## Next engineering milestones
1. Persist settings to a config file.
2. Add a real frame-time/FPS monitor with low overhead.
3. Implement one measurable optimization at a time.
4. Test against a clean vanilla baseline and other optimization mods using repeatable worlds and settings.
