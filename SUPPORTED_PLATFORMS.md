# Supported Platforms

SigmaEngine platform support is tied to published release artifacts. A platform is considered supported for a release only when that release includes an installer or archive, a checksum entry, release notes, and validation notes.

| Platform | Architecture | Package | Status |
|----------|--------------|---------|--------|
| macOS | arm64 | DMG | Published in `v0.1.0` |
| Windows | x64 | MSI | Planned |
| Linux | TBD | TBD | Planned |

## macOS

The first public package is an Apple Silicon DMG:

```text
SigmaEngine-v0.1.0-macOS-arm64.dmg
```

Known macOS caveat: the app is currently unsigned and not notarized, so macOS Gatekeeper may require manual approval on first launch.

## Windows

Windows packaging is planned as an MSI installer. It is not available in the current public release.

## Linux

Linux packaging is planned. The package format is still undecided.

## Future Platform Notes

Future releases may add:

- macOS universal builds.
- Windows x64 MSI packages.
- Linux AppImage, DEB, RPM, or another distribution format.
- Signed and notarized desktop artifacts.
