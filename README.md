# Recycle Bin File Preview

Enable the native **Windows File Explorer Preview Pane (Alt + P)** for files
in the Recycle Bin, without restoring them.

![Before and after: native Recycle Bin file preview](assets/recycle-bin-file-preview-comparison.png)

*Before: the default Recycle Bin view. After: the same file can be previewed
with Recycle Bin File Preview enabled.*

## Features

- Uses the normal File Explorer Preview Pane, not a separate viewer.
- Works with the file types and preview handlers already supported by Windows.
- Uses normal file associations when Recycle Bin associations fail.
- Does not restore, copy, change, or delete files.
- Requires no setup. Debug logging is the only optional setting, off by default.

## How to use

1. Open the Recycle Bin in File Explorer.
2. Press **Alt + P** to show the Preview Pane.
3. Select a file to view its preview.

## Installation

This mod is being prepared for the official [Windhawk](https://windhawk.net/) catalog.
Until it is available there, install it as a local mod:

1. Open Windhawk and create a new mod.
2. Copy the contents of `recycle-bin-file-preview.wh.cpp` into the editor.
3. Compile and enable the mod.
4. Open the Recycle Bin and press **Alt + P**.

Disable any earlier test mod named `recycle-bin-preview` to avoid running
two similar hooks at the same time.

## Compatibility and limits

- Preview depends on the handlers installed on your PC. A format that has
  no preview in a normal Explorer folder may also have no preview in Recycle Bin.
- The mod does not add codecs or preview handlers.
- The mod does not open deleted folders for navigation.
- Windows updates can change how file previews work.
- Version 1.0.0 still needs final tests on different Windows builds.

## Troubleshooting

Turn on **Debug logging** in the mod settings, reproduce the problem, and
check the Windhawk log for messages starting with `RBP:`. Turn it off after testing.

## Author and license

**Luiz Bizzio**. Licensed under **MIT**; see [LICENSE](LICENSE).
