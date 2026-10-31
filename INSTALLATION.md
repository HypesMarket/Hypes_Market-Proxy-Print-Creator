# Install Hypes_Market Proxy Print Creator 1.0.12

Download the app for your computer from the [latest release](https://github.com/HypesMarket/Hypes_Market-Proxy-Print-Creator/releases/latest). Choose the named Mac or Windows ZIP; GitHub's automatic Source code archives contain documentation, not the app. No Node.js or developer tools are required.

## Mac with Apple Silicon

1. Download `Hypes_Market-1.0.12-mac-arm64.zip`.
2. Open the ZIP to extract `Hypes_Market.app`.
3. Drag the app into your Applications folder, then open it.

This build targets Apple Silicon (M-series) Macs and has been tested on Apple Silicon macOS. Intel Macs are not supported. The app is ad-hoc signed and is not notarized by Apple, so macOS may display a security prompt or prevent it from opening normally. Contact support if you cannot open the app.

## Windows 11 (x64)

1. Download `Hypes_Market-1.0.12-win-x64.zip`.
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
4. Select cutting guides and upscaling. Lanczos and 1400 DPI are the factory defaults; your saved project, preset, and personal default choices are retained.
5. Export a PDF. Print at **100% / Actual Size**, with printer scaling disabled, and measure a test sheet before printing a full deck.

The transparent −/+ controls change screen zoom only. The percentage appears underneath both buttons. The main sheet supports 10%–500% zoom in 10 percentage-point steps.

The back arrow removes the most recently added card and its linked back without changing settings. The right curved arrow duplicates the last card in current sheet order. Use **Cmd/Ctrl + Z** to Undo and **Cmd/Ctrl + Shift + Z** to Redo history actions.

If a large export runs out of memory, try a smaller job or a lower DPI setting. Higher DPI cannot recreate detail missing from the source image.

## Offline and online features

Local uploads, editing, the bundled test image, the Guide, and PDF generation work without downloading artwork. Online card searches, Identify, deck imports, and remote artwork require an internet connection; card catalog requests may also run automatically. No account or subscription is required to use the app.

## Download verification and help

[SHA256SUMS.txt](https://github.com/HypesMarket/Hypes_Market-Proxy-Print-Creator/blob/main/SHA256SUMS.txt) lists the app ZIP checksums. Use the checksums attached to the same release when verifying an older version.

Email [support@hypesmarket.com](mailto:support@hypesmarket.com), or [open an issue](https://github.com/HypesMarket/Hypes_Market-Proxy-Print-Creator/issues). Include the app version, operating system, and steps to reproduce the problem.
