# Arkemis desktop releases

This repository only hosts the **Arkemis** desktop installers and the update metadata that installed copies of Arkemis read. It contains no source code.

- **Download:** [arkemis.space/download](https://arkemis.space/download) or the [latest release](https://github.com/vemulasukrit/arkemis-releases/releases/latest) (`Arkemis-<version>-win-x64.exe`).
- **Website:** [arkemis.space](https://arkemis.space)

## Updates

Installed copies of Arkemis update themselves. Shortly after launch and every few hours, Arkemis checks this repository's latest release, downloads a newer version in the background and shows **Restart to update**. It never restarts on its own; an update you haven't applied installs the next time you quit. You can also use **Settings → Help → Check for updates**.

Each release contains:

| File | Purpose |
| --- | --- |
| `Arkemis-<version>-win-x64.exe` | Windows installer (64-bit) |
| `Arkemis-<version>-win-x64.exe.blockmap` | Lets the updater download only what changed |
| `latest.yml` | Version, size and SHA-512 checksum the updater verifies before installing |

## Windows SmartScreen

Arkemis isn't code signed yet. The first time you run the installer, Windows SmartScreen may show **Windows protected your PC**. Choose **More info → Run anyway**. Every update is checked against the SHA-512 checksum in `latest.yml` before it installs.

## Support

Questions or problems: see [arkemis.space](https://arkemis.space).
