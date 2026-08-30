# 📝 Addon Patch Notes | [Home](../index.md)

This project tracks add-on source and configuration files, but omits native binaries. This file records project-specific modifications that must be preserved when an add-on is upgraded.

---

## 🛠️ GEVP (Godot Easy Vehicle Physics)

!!! abstract "Core Modifications"
    The base GEVP plugin was patched to support the **Hourbloom** deterministic steering and state persistence architecture.

- **`vehicle.gd` Patch**: Exposed internal torque and suspension parameters to the `Vehicle3D` wrapper.
- **Steering Fix**: Added a safety clamp to the steering speed correction denominator in `process_steering()` to prevent division by zero when the vehicle is stationary.
- **Wheel Raycast Fix**: Modified the raycast calculation to handle [Terrain3D](../rendering/terrain3d_rendering.md) positive coordinate grids more accurately.

!!! warning "Reproducibility"
    If you reinstall the GEVP addon, you must re-apply these patches documented in this section to avoid breaking the vehicle physics integration.

---

## 🎨 Terrain3D

!!! success "Runtime Painting Integration"
    `SoilLayerService` batches Terrain3D control-map writes and performs one final GPU map update after large field-generation operations. This integration does not require a patched Terrain3D native library.

!!! warning "Project-specific Importer"
    Preserve `addons/terrain_3d/tools/importer.tscn` when upgrading Terrain3D. It references Hourbloom's terrain assets and import settings.
