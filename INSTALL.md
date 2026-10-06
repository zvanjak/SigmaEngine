# Install SigmaEngine

SigmaEngine releases are published on the GitHub Releases page:

<https://github.com/zvanjak/SigmaEngine/releases>

Each release includes the available platform packages, `SHA256SUMS.txt`, and release notes.

## Download

1. Open the latest SigmaEngine release.
2. Download the package for your platform.
3. Download `SHA256SUMS.txt` from the same release.
4. Verify the checksum before installing.

## Verify Checksums

### macOS Or Linux

```bash
shasum -a 256 <downloaded-file>
cat SHA256SUMS.txt
```

The checksum output for the downloaded file should match the corresponding line in `SHA256SUMS.txt`.

### Windows PowerShell

```powershell
Get-FileHash .\<downloaded-file> -Algorithm SHA256
Get-Content .\SHA256SUMS.txt
```

The hash output for the downloaded file should match the corresponding line in `SHA256SUMS.txt`.

## macOS

Download the DMG package, open it, then drag `SigmaGUI.app` to `Applications`, or run it directly from the mounted DMG for a quick test.

The current macOS build may be unsigned and not notarized. If macOS blocks the first launch:

1. Open `System Settings`.
2. Go to `Privacy & Security`.
3. Find the blocked SigmaGUI launch message.
4. Choose `Open Anyway`.

You can also Control-click `SigmaGUI.app`, choose `Open`, and confirm the launch.

## Windows

Download the MSI package and run it from File Explorer. If Windows SmartScreen warns about an unsigned or new publisher package, verify the checksum first and then choose the manual run option only if it matches the release checksum.

## Ubuntu Linux

Download the DEB package and install it with `apt` or `dpkg`:

```bash
sudo apt install ./SigmaEngine-*.deb
```

If you use `dpkg` directly and dependency installation is needed, run:

```bash
sudo dpkg -i ./SigmaEngine-*.deb
sudo apt -f install
```

## Reporting Problems

If a release artifact does not download, fails checksum verification, or does not launch, open an issue in this repository and include:

- SigmaEngine version.
- Operating system and architecture.
- Artifact name.
- Exact error message or screenshot.
- Whether checksum verification passed.
