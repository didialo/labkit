# LabKit

**A lightweight browser-based toolkit for Minecraft mod developers.**

LabKit is a collection of small utilities designed to make common mod-development tasks easier. It runs locally in a modern web browser and does not require a backend or installation.

> Current release: **v1.5.0**

## Features

### General utilities
- **JSON Formatter** — format and validate JSON, with additional key-sorting and clearing actions.
- **UUID Generator** — generate UUID v4 values in batches, then copy or download them.
- **Color Converter** — convert HEX colors to RGB and HSL.
- **Changelog Builder** — create changelog text in Markdown.

### Fabric development
- **Fabric Metadata** — create a `fabric.mod.json` file.
- **Fabric Project Generator** — generate a starter Fabric project as a ZIP archive.
- **Client Entrypoint Generator** — optionally include a client initializer in generated projects.
- **Mixin Template Generator** — optionally include a Mixin configuration and starter example.
- **Dependency Checker** — inspect `fabric.mod.json` for common metadata and dependency issues.

### Publishing
- **Modrinth README Generator** — build a Markdown README with project details, features, installation, dependencies, compatibility, credits, and links.

## Getting started

1. Download `LabKit-v1.5.0.html` from the [GitHub Releases](../../releases) page, or download this repository.
2. Open `index.html` in a modern browser.
3. Select a tool from the LabKit interface.

No local server is required for normal use.

## Notes

- LabKit runs in the browser. It does not upload your project files to a LabKit backend.
- ZIP generation uses JSZip loaded from a CDN, so an internet connection is required for that feature.
- Generated Fabric projects are starter templates. They are not compiled automatically.
- Dependency Checker performs basic metadata checks; it does not replace Gradle builds or verify every version's compatibility.
- Mixin templates need to be adapted to the actual target class, method, mappings, and Minecraft version before use.
- Keep backups of important project files before replacing them with generated files.

## Project structure

For GitHub Pages, keep `index.html` in the repository root:

```text
LabKit/
├── index.html
├── README.md
├── CHANGELOG.md
└── LICENSE
```

## Contributing

Bug reports and feature suggestions are welcome through the repository's GitHub Issues page. When reporting a bug, include:
- The tool you were using.
- The steps to reproduce the issue.
- The browser and version.
- Any relevant error message (do not include private information).

## License

LabKit is distributed under the MIT License. See [LICENSE](LICENSE).
