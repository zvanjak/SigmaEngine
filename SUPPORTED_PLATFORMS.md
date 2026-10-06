# Supported Platforms

SigmaEngine platform support is tied to published release artifacts. A platform is considered supported for a release only when that release includes an installer or package, a checksum entry, release notes, and validation notes.

| Platform | Architecture | Package | Status |
|----------|--------------|---------|--------|
| macOS | arm64 | DMG | Published in recent releases |
| Windows | x64 | MSI | Published in recent releases |
| Ubuntu Linux | x64 | DEB | Published in recent releases |

Always check the specific GitHub release for the exact artifact set:

<https://github.com/zvanjak/SigmaEngine/releases>

## macOS

The macOS package is distributed as a DMG for Apple Silicon. Current builds may be unsigned and not notarized, so macOS Gatekeeper can require manual approval on first launch.

## Windows

The Windows package is distributed as an x64 MSI installer. Current builds may trigger SmartScreen warnings until the publisher reputation matures.

## Ubuntu Linux

The Ubuntu package is distributed as an x64 DEB package.

## Future Platform Notes

Future releases may add:

- macOS universal builds.
- Additional Linux package formats such as AppImage, RPM, or tarball archives.
- Signed and notarized desktop artifacts.
