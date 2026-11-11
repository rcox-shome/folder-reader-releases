# Install the experimental preview

Folder Reader v0.1.2 supports **Apple silicon Macs running macOS 14 or later**. This package is a release-mode prototype, ad-hoc signed and not notarized. It is not an Intel or universal build.

1. Download **FolderReader-0.1.2-macOS-arm64.zip** from the [v0.1.2 release](https://github.com/rcox-shome/folder-reader-releases/releases/tag/v0.1.2). GitHub's automatically generated “Source code” archives contain this showcase repository, not the application.
2. Unzip it and move **Folder Reader.app** into Applications or your user Applications folder.
3. Launch it and choose **Open Folder**, or drop a folder into its window.

## First-launch security

The preview is not Developer ID signed or notarized, so macOS may block it. If you choose to run it after reviewing its provenance, follow [Apple's instructions for opening an app from an unidentified developer](https://support.apple.com/en-us/102445). Do not disable Gatekeeper globally.

A published SHA-256 checksum lets you check that your ZIP matches this release. It does not replace notarization.

```sh
shasum -a 256 FolderReader-0.1.2-macOS-arm64.zip
```

Expected checksum: see [SHA256SUMS.txt](SHA256SUMS.txt).

## Finder integration

Launch the app once from its permanent location. Right-click a folder and choose **Open in Folder Reader**; macOS may place it under **Services**.

If it is missing, look under **System Settings → Keyboard → Keyboard Shortcuts → Services → Files and Folders** and enable the service. Choose one folder at a time.

## Updates and removal

There is no automatic updater. New previews will appear on this repository's Releases page.

To remove the app, quit it and move it to the Trash. Your reading history remains at `~/Library/Application Support/FolderReader/history.json`; removing the app does not delete your documents.
