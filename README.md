<div align="center">

<img src="icon.svg" alt="Hourbloom sunflower icon" width="160"/>

<!-- Keywords: Hourbloom, open-source farming simulator, Godot 4, survival simulation, systemic game design -->

# Hourbloom
**A Hardcore, Open-Source Agricultural Life Simulator built in Godot 4.**

[![Version](https://img.shields.io/badge/Version-v_1.2-green)](#)
[![Docs](https://img.shields.io/badge/Documentation-v_1.2-blue)](https://fgh345.github.io/Hourbloom/)
[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](LICENSE)
[![License: CC BY-SA 4.0](https://img.shields.io/badge/License-CC%20BY--SA%204.0-lightgrey.svg)](Assets/README.md)

</div>

---

## 🌾 About the Project

**Hourbloom** is an open-source agricultural life simulator derived from [OpenAcre](https://github.com/OpenAcre-Project/OpenAcre). Here, survival is the ultimate metric. The game is built around a moddable, system-first engine where players manage personal needs, maintain complex machinery, and build functional infrastructure. If your tractor breaks down, your crops die. If your crops die, you starve.

Our goal is to push the boundaries of open-source life simulation, seamlessly blending minute-to-minute manual labor with long-term infrastructure strategy.

### ✨ Key Features
* ⚙️ **System-Driven Survival:** Manage personal stats alongside complex vehicle telemetry like fuel, engine temperature, and mechanical wear.
* 🚜 **Advanced PTO Physics:** A custom Vehicle-to-World Bridge for realistic implement attachment, stabilization, and dynamic land terraforming.
* 🧠 **Universal Entity Streaming (UESS):** A headless Event/Signal Bus that enables complex background logic (crop growth, AI routines) even in unloaded chunks.
* 🗺️ **Dual-View Gameplay:** Seamlessly switch between a tactical 2D map for land management and immersive 3D third/first-person manual labor.

---

## 🚀 Quick Start & Installation

> [!WARNING]  
> **Regarding ADD-ONS:**
> Hourbloom targets **Godot 4.7** and uses **Terrain3D 1.0.2**. Add-on source and project-specific files are tracked in this repository, while native libraries are not. Godot 4.7's built-in Jolt integration is used; do not install the legacy `godot-jolt` GDExtension.

**To run Hourbloom locally:**
1. Clone this repository and install an official **Godot 4.7.x** build.
2. Download the [Terrain3D 1.0.2 release](https://github.com/TokisanGames/Terrain3D/releases/tag/v1.0.2-stable).
3. Copy the release's `addons/terrain_3d/bin/` directory into the existing `addons/terrain_3d/` directory. Do not replace the project-specific add-on files.
4. Open `project.godot`, wait for the initial import to finish, and restart the editor once.

---

## 🗺️ Upstream Project

Hourbloom currently follows OpenAcre's simulation architecture. Upstream changes can be reviewed on the [OpenAcre project board](https://github.com/orgs/OpenAcre-Project/projects/1) and selectively merged into this fork.

---

## 🏛️ Project Architecture & Docs
Because Hourbloom is built as an extensible simulation engine, strict architectural guidelines are enforced.
* Please see the [Architecture Guidelines](docs/architecture/overview.md) for details on script layouts, avoiding Autoload clutter, and UESS implementation.
* Want to help build the engine? Read our [CONTRIBUTING.md](CONTRIBUTING.md) before submitting a Pull Request!

---

## ⚖️ Licensing

Hourbloom is derived from OpenAcre and retains its open-source licensing requirements:

| Project Component | License | What It Guarantees |
| :--- | :--- | :--- |
| **Client Code & Engine** | **[GPLv3](LICENSE)** | Any derivatives or mods distributed to players must remain open-source. |
| **Server/Backend Code** | **AGPLv3** | Anyone running modified servers must share their backend code. |
| **Art, Audio, Models** | **[CC BY-SA 4.0](Assets/README.md)** | Anyone modifying our assets must credit the project and share their new assets freely. |

---

## 💖 Credits

Hourbloom is based on [OpenAcre](https://github.com/OpenAcre-Project/OpenAcre), created by Jovi Koikkara and its contributors. See [AUTHORS.md](AUTHORS.md) for attribution.

---
### Key Asset Credits: 

* World Map inspired by [Elmcreek](https://www.farming-simulator.com/mod.php?mod_id=335352&title=fs2025).
* Player Assets from [Playable Workshop](https://playableworkshop.com/videos/action-adventure-series-ep-3).
* Textures from [ambientCG](https://ambientcg.com/).
