# Install SigmaEngine

SigmaEngine releases are published on the GitHub Releases page:

<https://github.com/zvanjak/SigmaEngine/releases>

## macOS Apple Silicon

The current macOS package is built for Apple Silicon:

```text
SigmaEngine-v0.1.0-macOS-arm64.dmg
```

1. Download the DMG from the `v0.1.0` release page.
2. Download `SHA256SUMS.txt` from the same release.
3. Verify the checksum:

```bash
shasum -a 256 SigmaEngine-v0.1.0-macOS-arm64.dmg
cat SHA256SUMS.txt
```

The checksum output for the DMG should match the line in `SHA256SUMS.txt`.

4. Open the DMG.
5. Drag `SigmaGUI.app` to `Applications`, or run it from the mounted DMG for a quick test.

## First Launch On macOS

The current macOS build is unsigned and not notarized. If macOS blocks the first launch:

1. Open `System Settings`.
2. Go to `Privacy & Security`.
3. Find the blocked SigmaGUI launch message.
4. Choose `Open Anyway`.

You can also Control-click `SigmaGUI.app`, choose `Open`, and confirm the launch.

## Windows

Windows packages are planned but not published yet.

## Linux

Linux packages are planned but not published yet. The package format has not been finalized.

## Reporting Problems

If a release artifact does not download, fails checksum verification, or does not launch, open an issue in this repository and include:

- SigmaEngine version.
- Operating system and architecture.
- Artifact name.
- Exact error message or screenshot.
- Whether checksum verification passed.
