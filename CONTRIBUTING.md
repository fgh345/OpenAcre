# Contributing to OpenAcre

Thank you for your interest in contributing to **OpenAcre**! We welcome contributions of all forms, from bug reports to new features. 

Documentation is available at: [https://openacre-project.github.io/OpenAcre/](https://openacre-project.github.io/OpenAcre/)

## How to Contribute

### 1. Reporting Bugs
- Use the [GitHub Issue Tracker](https://github.com/OpenAcre-Project/OpenAcre/issues).
- Provide a clear description and steps to reproduce.

### 2. Feature Requests
- Open an issue to discuss your idea first.

### 3. Pull Requests
- Fork the repository.
- Create a new branch for your feature or bugfix (e.g., `feat/my-new-feature` or `fix/issue-description`).
- Submit a Pull Request to the `main` branch.
- Ensure your code follows the project's coding standards.

## Development Setup

1. Clone the repository.
2. Install an official [Godot 4.7.x](https://godotengine.org/) build.
3. Download [Terrain3D 1.0.2](https://github.com/TokisanGames/Terrain3D/releases/tag/v1.0.2-stable) and copy only its `addons/terrain_3d/bin/` directory into the repository's existing Terrain3D directory.
4. Open the project and wait for the initial import to finish. The project uses Godot's built-in Jolt integration, so the legacy `godot-jolt` GDExtension must not be installed.

## Coding Style
- Follow the official [GDScript style guide](https://docs.godotengine.org/en/stable/tutorials/scripting/gdscript/gdscript_styleguide.html).
- Keep simulation logic decoupled from visuals where possible.

## License
By contributing, you agree that your contributions will be licensed under the project's license (GPLv3 and CC BY-SA 4.0 for assets).
