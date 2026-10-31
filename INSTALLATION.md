# Install Hypes_Market Proxy Print Creator 1.0.15

Download the app for your computer from the [latest release](https://github.com/HypesMarket/Hypes_Market-Proxy-Print-Creator/releases/latest). Choose the named Mac or Windows ZIP; GitHub's automatic Source code archives contain documentation, not the app. No Node.js or developer tools are required.

## Mac with Apple Silicon

1. Download `Hypes_Market-1.0.15-mac-arm64.zip`.
2. Open the ZIP to extract `Hypes_Market.app`.
3. Drag the app into your Applications folder, then open it.

This build targets Apple Silicon (M-series) Macs and has been tested on Apple Silicon macOS. Intel Macs are not supported. The app is ad-hoc signed and is not notarized by Apple, so macOS may display a security prompt or prevent it from opening normally. Contact support if you cannot open the app.

## Windows 11 (x64)

1. Download `Hypes_Market-1.0.15-win-x64.zip`.
2. Right-click the ZIP and choose **Extract All**.
3. Open the extracted folder and launch `Hypes_Market.exe`.

Keep the EXE and every accompanying file and folder together. This is a portable ZIP distribution, not a Windows installer. The build is unsigned and has not yet been runtime-tested on a Windows device; it is offered as a preview. Windows may display an unrecognized-app warning.

## Updating

Close Hypes_Market before replacing its application files. On Mac, replace the app in Applications. On Windows, extract the new version into its own folder and launch the new copy with all its accompanying files.

Saved projects, uploads, and settings use your operating system's application-data folder, separate from the app files. Keep your original artwork and exported decklists as backups. Do not use **Reset App Data** to update; it removes saved project and upload data after confirmation.

Updates are downloaded manually. This version has no automatic update service.

## Your first print

1. Open **Guide** in the app for the full workflow.
2. Upload images, or use **Test Image** to add the bundled offline calibration artwork.
3. Choose the card trim size and layout. For the calibration artwork's size label, use **Standard (63 × 88 mm)**.
4. Configure bleed manually in the right Settings column, then select cutting guides and upscaling. Lanczos and 1400 DPI are the factory defaults; your saved project, preset, and personal default choices are retained.
5. Export a PDF. Print at **100% / Actual Size**, with printer scaling disabled, and measure a test sheet before printing a full deck.

The red −/+ symbols have a visible background on hover or keyboard focus and change screen zoom only. The percentage appears underneath both buttons. The main sheet supports 10%–500% zoom in 10 percentage-point steps.

The back arrow removes the most recently added card and its linked back without changing settings. The right curved arrow duplicates the last card in current sheet order. Use **Cmd/Ctrl + Z** to Undo and **Cmd/Ctrl + Shift + Z** to Redo history actions.

If a large export runs out of memory, try a smaller job or a lower DPI setting. Higher DPI cannot recreate detail missing from the source image.

## Upload folders and source bleed

**Upload Images** is a plain button. **Manage Uploads** opens the local image library. On desktop, Upload Images remembers the last confirmed upload folder; the folder-up button beside it opens that folder's parent. The shortcut becomes available after you have chosen images once. On Mac, **Command + Up Arrow** navigates to the enclosing folder within the picker. Its Back/Forward history starts fresh each time the native picker opens.

New uploads start with no built-in source bleed, with no automatic detection from image dimensions. If your file already includes a margin:

1. Select an uploaded front card on the sheet.
2. Open **Bleed → Uploaded artwork source bleed** in the right Settings column.
3. Check **Artwork already includes bleed** and enter the margin already in the file, in millimeters.
4. Choose **Apply to all copies in this project**. It updates the selected artwork's copies in the current project, including linked backs that use the same artwork. Other projects and saved upload-library records stay unchanged. Keyboard Undo/Redo remains available.

Source bleed of **0 mm** means there is no margin already in the artwork. **Bleed Width** and **Images With/Without Bleed Settings** determine the output margin. To preserve transparent PNG corners, use **0 mm output bleed** or the appropriate **No Bleed** option, and check per-card overrides. Positive generated bleed deliberately fills a square print margin; cutting-guide shapes do not change the artwork's transparency.

## Offline and online features

Local uploads, editing, the bundled test image, the Guide, and PDF generation work without downloading artwork. Online card searches, Identify, deck imports, and remote artwork require an internet connection; card catalog requests may also run automatically. No account or subscription is required to use the app.

## Download verification and help

[SHA256SUMS.txt](https://github.com/HypesMarket/Hypes_Market-Proxy-Print-Creator/blob/main/SHA256SUMS.txt) lists the app ZIP checksums. Use the checksums attached to the same release when verifying an older version.

Email [support@hypesmarket.com](mailto:support@hypesmarket.com), or [open an issue](https://github.com/HypesMarket/Hypes_Market-Proxy-Print-Creator/issues). Include the app version, operating system, and steps to reproduce the problem.
