# SigmaEngine

SigmaEngine is an early desktop release of the Sigma mathematical computing environment.

It combines an interactive calculator-style workflow, typed mathematical function definitions, numerical analysis tools, symbolic expression support, and C++ code generation in a wxWidgets desktop app.

The source project is currently developed privately. This public repository is the release home for downloadable installers, checksums, release notes, and user-facing documentation.

## What It Does

- Evaluate scalar, vector, matrix, and polynomial expressions.
- Define reusable mathematical functions, including typed scalar and vector functions for numerical analysis.
- Run numerical operations such as differentiation, integration, root finding, gradients, and Jacobians.
- Work with symbolic expressions, including differentiation and simplification.
- Generate C++ from an interactive Sigma session for use with the MML math library.
- Use a notebook-style desktop GUI for exploratory calculations.

## Current Release

The first public release is `v0.1.0`:

- Release page: <https://github.com/zvanjak/SigmaEngine/releases/tag/v0.1.0>
- macOS Apple Silicon DMG: `SigmaEngine-v0.1.0-macOS-arm64.dmg`
- Checksums: `SHA256SUMS.txt` on the release page

This is an early preview release. The macOS app is unsigned and not notarized, so macOS Gatekeeper may require manual approval on first launch.

## Download And Install

See [INSTALL.md](INSTALL.md) for download, checksum verification, and first-launch instructions.

## Platform Status

See [SUPPORTED_PLATFORMS.md](SUPPORTED_PLATFORMS.md) for the current packaging status.

At the moment, only macOS Apple Silicon has a published installer. Windows and Linux packages are planned.

## Release Notes

Each GitHub release contains release notes with supported artifacts, validation status, known issues, and checksums. A reusable template is kept in [docs/RELEASE_NOTES_TEMPLATE.md](docs/RELEASE_NOTES_TEMPLATE.md).

## Project Status

SigmaEngine is pre-1.0 software. User-facing behavior, file formats, generated code shape, and packaging details may change between early releases.

## License

License information has not been published yet. Do not redistribute SigmaEngine artifacts outside the GitHub releases unless a future release explicitly states redistribution terms.