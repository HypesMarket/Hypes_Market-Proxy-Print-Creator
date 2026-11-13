# Install Hypes_Market Proxy Print Creator 1.0.18

Download the app for your computer. No Node.js, developer tools, account, or subscription is required.

- [Apple Silicon Mac ZIP](https://github.com/HypesMarket/Hypes_Market-Proxy-Print-Creator/releases/download/v1.0.18/Hypes_Market-1.0.18-mac-arm64.zip)
- [Windows 11 x64 ZIP](https://github.com/HypesMarket/Hypes_Market-Proxy-Print-Creator/releases/download/v1.0.18/Hypes_Market-1.0.18-win-x64.zip)
- [Latest release and all files](https://github.com/HypesMarket/Hypes_Market-Proxy-Print-Creator/releases/latest)

Choose the named Mac or Windows ZIP. GitHub's automatic **Source code** archives contain this repository's documentation, not the app.

## Mac with Apple Silicon

1. Download `Hypes_Market-1.0.18-mac-arm64.zip`.
2. Open the ZIP to extract `Hypes_Market.app`.
3. Drag the app into Applications, then open it.

This build targets Apple Silicon (M-series) Macs. Intel Macs are not supported. The app is ad-hoc signed and is not notarized by Apple, so macOS may display a security prompt or prevent it from opening normally. Contact support if you cannot open the app.

## Windows 11 (x64)

1. Download `Hypes_Market-1.0.18-win-x64.zip`.
2. Right-click the ZIP and choose **Extract All**.
3. Open the extracted folder and launch `Hypes_Market.exe`.

Keep the EXE and all accompanying files and folders together. This is a portable ZIP, not a Windows installer. The build is unsigned, so Windows may display an unrecognized-app warning.

Version 1.0.18 was packaged and audited but was not run on a Windows device during release preparation. Version 1.0.15 received focused workflow checks and physical print testing on Windows 11. Those earlier checks do not cover every workflow in this release, duplex printing, or every printer configuration.

## Updating

Close Hypes_Market before replacing application files. On Mac, replace the app in Applications. On Windows, extract the new version into its own folder and launch it with all accompanying files.

Saved projects, uploads, presets, and settings use your operating system's application-data folder, separate from the app files. Keep original artwork and exported decklists as backups. Do not use **Reset App Data** to update; it removes saved project and upload data after confirmation.

Updates are downloaded manually. This version has no automatic update service.

## Your first print

1. Open **Guide** in the app for the full workflow.
2. Use **Upload Images**, drag files from Finder or File Explorer onto the sheet, or click **Test Image** for the bundled offline calibration artwork. Dropped images fill the next available tiles; existing cards remain in place.
3. Choose a card trim size and layout. Use **Standard (63 × 88 mm)** to check the calibration card's printed size label.
4. Configure bleed manually in the right Settings column, then choose cutting guides and upscaling. Lanczos and 1400 DPI are the factory defaults; saved project, preset, and personal default choices are retained.
5. Export a PDF. Print at **100% / Actual Size**, with printer scaling disabled, and measure a test sheet before printing a full deck.

Screen zoom does not change exported or printed dimensions. The lower-left back arrow removes the most recently added card and its linked back without changing settings. The right curved arrow duplicates the last card in current sheet order. Use **Cmd/Ctrl + Z** to Undo and **Cmd/Ctrl + Shift + Z** to Redo history actions.

## Export quality

**Bicubic** and **Lanczos** apply the selected **Minimum export DPI (per card)** during PDF and card image export. Lower-resolution artwork is enlarged directly once using local native processing; artwork already at or above the minimum retains its native resolution. Bleed and effects use that full export resolution, without a 1200 DPI intermediate reduction.

At a 1400 DPI minimum, 300 DPI artwork goes directly to 1400, while 1800 DPI artwork stays at 1800. **No upscaling** instead uses an **Export DPI ceiling (per card)**: the lower of the source resolution and the selected ceiling.

Printed card dimensions stay the same. Previews are separate from export processing, and original source files remain unchanged. Source resolution depends on the file's pixel dimensions at the chosen physical size; editing DPI metadata does not add detail, and enlargement cannot recreate missing detail.

## Large exports

Higher-resolution artwork can create larger files and require more memory and processing time. Each card is checked against processing limits. If the app cannot preserve the required resolution, it reports the problem instead of silently reducing quality.

For memory errors, close other applications or export a smaller job. **Lowering the Bicubic/Lanczos minimum will not reduce a source already above it.** If an individual source is too large, use a smaller copy of the original or select **No upscaling** with a lower DPI ceiling. Keep your original artwork as a backup.

## Upload folders and source bleed

**Manage Uploads** opens the local image library. On desktop, **Upload Images** remembers the last confirmed upload folder; the folder-up button beside it opens that folder's parent. Choose images once to enable this shortcut. On Mac, **Command + Up Arrow** also opens the enclosing folder inside the picker. Picker Back/Forward history starts fresh each time it opens.

New uploads start with no built-in source bleed; there is no automatic detection from image dimensions. If your file already includes a margin:

1. Select an uploaded front card on the sheet.
2. Open **Bleed → Uploaded artwork source bleed** in the right Settings column.
3. Check **Artwork already includes bleed** and enter the existing margin in millimeters.
4. Choose **Apply to all copies in this project**. This updates copies of that artwork in the open project, including linked backs using the same artwork. Other projects and upload-library records stay unchanged. Undo/Redo is available.

Source bleed of **0 mm** means there is no margin already in the artwork. **Bleed Width** and **Images With/Without Bleed Settings** control the output margin. To retain transparent PNG corners, use **0 mm output bleed** or the appropriate **No Bleed** option, and check per-card overrides. Positive generated bleed deliberately fills a square print margin. Cutting-guide shapes do not change image transparency. Guide colors render at full opacity in previews and PDFs.

## Find exported PDFs

The **Recent PDF downloads** button immediately right of the theme button lists the last 20 completed PDFs saved by the app, newest first, with filenames, dates, and sizes. A green dot marks a new save. Click a PDF to show it in Finder or File Explorer.

History stays on this device across restarts. Cancelled or failed saves and PDFs saved before version 1.0.16 are excluded. If a file was moved or deleted outside the app, a message explains why it cannot be shown.

## Offline and online features

Local uploads, editing, Test Image, the Guide, and PDF generation work without downloading artwork. Optional searches, Identify, online artwork, and deck imports contact external services; card catalog requests may also run automatically. The app contains no ads or usage telemetry.

## Download verification and help

[SHA256SUMS.txt](https://github.com/HypesMarket/Hypes_Market-Proxy-Print-Creator/blob/main/SHA256SUMS.txt) lists the current app ZIP checksums. Use checksums attached to the same release when verifying an older version.

Email [support@hypesmarket.com](mailto:support@hypesmarket.com) or [open an issue](https://github.com/HypesMarket/Hypes_Market-Proxy-Print-Creator/issues). Include your app version, operating system, and steps to reproduce the problem.

Optional support: [Buy Me a Coffee](https://buymeacoffee.com/hypesmarket) · [Ko-fi](https://ko-fi.com/hypesmarket). Every feature remains free.
