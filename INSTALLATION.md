# Install Hypes_Market Proxy Print Creator

## Mac with Apple Silicon

1. Download `Hypes_Market-1.0.7-mac-arm64.zip` from the release page.
2. Open the ZIP to extract `Hypes_Market.app`.
3. Drag the app into your Applications folder, then open it.

This build targets Apple Silicon (M-series) Macs. It is ad-hoc signed and is not notarized by Apple. Intel Macs are not supported. No Node.js installation is required.

## Windows 11 (x64)

1. Download `Hypes_Market-1.0.7-win-x64.zip` from the release page.
2. Right-click the ZIP and choose **Extract All**.
3. Open the extracted folder and launch `Hypes_Market.exe`.

Keep the EXE and all the files and folders beside it together. This is a portable ZIP distribution, not a Windows installer. No Node.js installation is required. The build is unsigned and has not yet been runtime-tested on a Windows device; it is offered as a preview.

## Updating

Close Hypes_Market before replacing the application files. Keep your original artwork and exported decklists as backups. Saved projects and settings use your operating system's application-data folder, separate from the extracted application. Do not use **Reset App Data** to update the app; it removes saved application data after confirmation.

## Your first print

Use **Guide** in the app for the full workflow. Upload images, choose the trim size and layout, select guides and upscaling, then export a PDF. 1400 DPI is the default DPI setting. Print at **100% / Actual Size**, with printer scaling disabled, and measure a test sheet before printing a full deck.

If a large export runs out of memory, try a smaller job or a lower DPI setting. Higher DPI cannot recreate detail missing from the source image.

## Help

Email [support@hypesmarket.com](mailto:support@hypesmarket.com), or open an issue on this repository. Include the app version, operating system, and steps to reproduce the problem.
