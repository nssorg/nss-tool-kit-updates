# NSS TOOL KIT Updates

Public release channel for the NSS TOOL KIT After Effects extension. The owner source repository is private: [nssorg/nss-tool-kit-source](https://github.com/nssorg/nss-tool-kit-source).

## Install

Download the [v1.1.0 installer](https://github.com/nssorg/nss-tool-kit-updates/releases/download/v1.1.0/NSS-TOOL-KIT-Installer.zip), extract it, run `Install NSS TOOL KIT.bat`, then restart After Effects and open **Window > Extensions > NSS TOOL KIT**.

## Updates

The panel checks GitHub when it opens and every 15 minutes while it remains open. A newer release displays **Update now** and **Later**. An update reaches an already-open panel at its next poll; GitHub does not push the notice instantly. Before installation, the updater validates the feed, package URL, extension ID, version, and SHA-256 checksum, and keeps a rollback copy.

The public release assets are `NSS-TOOL-KIT.zip` and `NSS-update.json`. New releases use the same asset names and a new version tag.

## Owner publishing

Use `NSS Update Publisher.bat` from the private source archive. Publish with an owner-only GitHub token stored locally and limited to the two NSS repositories. The publisher builds the package, updates the SHA-256 feed, and publishes the public update release plus a private source snapshot. Never include a GitHub token or API key in the plugin or release ZIP.

## Security and privacy

Private GitHub source limits who can view the repository. The public install package must contain the files users run, so recipients can read or copy the installed plugin code and assets. Client-side files cannot be made inaccessible to a computer owner. Caption engines and models are downloaded separately and are not included in the plugin release ZIP.

## Releases

- [Latest release](https://github.com/nssorg/nss-tool-kit-updates/releases/latest)
- [v1.1.0 release](https://github.com/nssorg/nss-tool-kit-updates/releases/tag/v1.1.0)
- [Private owner source repository](https://github.com/nssorg/nss-tool-kit-source)
