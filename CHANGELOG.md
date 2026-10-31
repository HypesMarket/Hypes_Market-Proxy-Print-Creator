# Hypes_Market release history

User-facing changes since version 1.0.7. See the [releases page](https://github.com/HypesMarket/Hypes_Market-Proxy-Print-Creator/releases) for downloads.

## 1.0.15 — October 31, 2026

- Simplified **Upload Images** to a plain button with the parent-folder shortcut retained. Removed its settings gear, bleed-mode menu, and automatic bleed detection.
- Renamed **My Uploads** to **Manage Uploads**.
- New uploads start with no built-in source bleed. Configure bleed manually in the right Settings column.
- Added **Uploaded artwork source bleed** controls with an explicit **Apply to all copies in this project** action, including Undo/Redo. Other projects, saved library records, and output settings are preserved.
- Respected manually entered **0 mm** source bleed and refreshed processing/import handling so manual choices take effect.
- Updated the Guide for the simplified upload and manual bleed workflow.

## 1.0.14 — October 31, 2026

- Made the −/+ zoom symbols red, with visible hover and keyboard-focus backgrounds in both themes.
- Added a native desktop image picker that remembers the last confirmed upload folder, plus **Upload from parent folder** beside Upload Images.
- Preserved multiple-file selection, cancellation, repeated selection, and project guards. The parent shortcut works independently of the native picker's Back/Forward history.
- Updated the Guide with folder navigation and zoom appearance.

## 1.0.13 — October 31, 2026

- Preserved transparent and partially transparent PNG pixels in previews and exports when no new bleed is generated. Rounded corners stay transparent at zero bleed.
- Refreshed derived image and effect caches from original artwork so saved projects use the correction without re-uploading images.
- Clarified card dimensions, transparent corners, generated bleed, and cutting guides in the Guide. Positive generated bleed keeps its square print margin.

## 1.0.12 — October 31, 2026

- The lower-left back arrow is now **Remove last card**. It removes the most recently added front and its linked back, without undoing settings.
- Card addition order is preserved independently of tile rearrangement. Older cards without addition history use their saved sheet order as the initial removal order.
- Keyboard Undo and Redo remain available for history actions, including restoring removed cards and changing settings.
- The Guide explains the removal arrow, Duplicate arrow, and keyboard history actions.

## 1.0.11 — October 30, 2026

- Replaced the hover zoom slider with always-visible transparent −/+ buttons and the current percentage centered underneath both buttons.
- Main-sheet zoom remains 10%–500%, with 10 percentage-point button steps.
- The lower-left right curved arrow now duplicates the last card into the next tile. Keyboard Redo remains available.
- Updated the Guide with zoom controls and keyboard shortcuts.

## 1.0.10 — October 30, 2026

- Moved **Clear Cards** directly below Duplicate, retaining its confirmation warning. Test Image follows Clear Cards.
- Made **Lanczos** the factory upscaling default for new projects without personal defaults. Explicit saved upscaling choices are retained; the factory DPI remains 1400.
- Updated the Guide for card clearing, button order, and default upscaling.

## 1.0.9 — October 30, 2026

- Centered **Donate** at the top of the app, retaining its soft halo and optional donation links.
- Duplicate is grey and unavailable when there is no usable card artwork to copy, and green when available.
- Test Image is purple to match Export Card Images.
- Updated the Guide's quick start, calibration instructions, and donation information.

## 1.0.8 — October 30, 2026

- Added **Duplicate** in the Upload column to append the last card on the current sheet, retaining its artwork, edits, and linked back.
- Added **Test Image** to append bundled Hypes_Market calibration artwork without an image download. Repeated clicks add separate cards.
- Added a pin button immediately left of the theme button to keep the desktop app above other ordinary windows. Click again to unpin; new app sessions start unpinned.
- Added Undo and Redo support for the new card actions and updated the Guide.
