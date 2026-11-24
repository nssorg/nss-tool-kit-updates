# NSS TOOL KIT Updates

This repository distributes checksum-validated updates for the NSS TOOL KIT After Effects panel. The private source repository is `nssorg/nss-tool-kit-source`.

## Install

For a first install, download `NSS-TOOL-KIT-Installer.zip` from the latest release, extract it, and run `Install NSS TOOL KIT.bat`. Restart After Effects and open **Window > Extensions > NSS TOOL KIT**.

## Updates

The panel checks when it opens and every 15 minutes while open. When it sees a newer GitHub release, it shows **Update now** and **Later**. GitHub Releases are polled, so an update prompt appears at the next check rather than being pushed instantly.

Before installation, the updater validates the HTTPS package URL, extension ID, version, and SHA-256 checksum. It keeps a rollback copy during installation.

## Current version

**v1.2.0** adds 41 imported presets (17 CC, 12 text animations, 8 shake, 4 transitions). Seven image/video previews are cropped or cover-fit to the card's 16:9 size. Existing text animation In/Out/Loop groups remain.

## Security and privacy

The private source repository is owner-only. Files inside the public release ZIP, including the plugin source and supplied preset assets, are readable and copyable by users who download it. Caption models are downloaded separately and are not included. Never put API keys or publishing credentials in the plugin package.