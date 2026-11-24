# NSS TOOL KIT — Updates

This public repository hosts versioned release metadata and installer packages for the NSS TOOL KIT After Effects panel. The source repository is private and owner controlled.

## First installation

No updater release has been published yet. After the owner publishes the first version, first-time users can install with **NSS-TOOL-KIT-Installer.zip** from the [Releases](https://github.com/nssorg/nss-tool-kit-updates/releases) page.

## Updates after installation

The panel checks GitHub when it opens and every six hours. When a newer version is available, it shows release notes and offers **Update now** or **Later**. The updater downloads **NSS-TOOL-KIT.zip**, checks its SHA-256 value from **NSS-update.json**, replaces the extension files, and reloads the panel. Presets, caption settings, and saved user data are stored outside the extension folder.

## Owner publishing workflow

1. Open **NSS Update Publisher.bat** from the private source archive.
2. Create a fine-grained GitHub token limited to **nssorg/nss-tool-kit-source** and **nssorg/nss-tool-kit-updates** with **Contents: Read and write**. Paste it only into the local publisher; it is not shipped with the plugin.
3. Enter a newer version in **major.minor.patch** format, add release notes, then choose **Build and publish update**.
4. The publisher creates the public update release and a private source snapshot. Share the installer asset with first-time users; existing installs will see the update prompt automatically.

## Repository and release safety

- Keep the source code private. This repository is public so plugin users can download releases.
- Never put GitHub tokens, API keys, or private credentials in this repository or in a release package.
- Anyone who receives an installable plugin package can inspect or copy its files. Private GitHub source protects the repository; it cannot make files on a user computer inaccessible to that user.
- The caption engine and speech model are downloaded separately to Documents/NSS TOOL KIT/engine and are not included in the plugin release ZIP.

Private source: [nssorg/nss-tool-kit-source](https://github.com/nssorg/nss-tool-kit-source)  
Public releases: [nssorg/nss-tool-kit-updates/releases](https://github.com/nssorg/nss-tool-kit-updates/releases)
