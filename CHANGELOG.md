## [1.0.22] - 2026-11-14

### Added

- Hover over a Recent Images thumbnail to see a larger preview from the original image. Move away to close it.

## [1.0.21] - 2026-11-14

### Added

- Recent Images shows thumbnails from the original files beside their folder locations.

## [1.0.20] - 2026-11-14

### Changed

- Replaced Manage Uploads with Recent Images. The history remembers original file locations for reuse and reads the current file when adding it to a sheet.
- Removing a history entry or clearing the list leaves original files and saved sheets intact. A new profile starts with an empty history, and existing sheets can still use their saved copies.

## [1.0.19] - 2026-11-14

### Changed

- Removed the legacy artwork from the built-in cardback library. Blank is the default, and saved sheets that refer to a retired back now use Blank.
- The Test Image button adds the geometric print calibration card.

## [1.0.18] - 2026-11-12

### Fixed

- Cutting guides use the full opacity of the selected RGB color in sheet previews and PDFs, including when a pasted color contains transparency.

## [1.0.17] - 2026-11-10

### Fixed

- Removed the 1200 DPI intermediate reduction from PDF and card image export bleed/effect processing, preserving high-resolution source detail.
- Added per-card resource checks that report failures instead of silently reducing export resolution.
- Preserved unedited PNG pixels and transparency when embedding artwork in PDFs.
- Preserved image proportions when fitting wide or tall artwork, and removed thin transparent edges caused by bleed rounding.

### Changed

- Bicubic and Lanczos now treat selected export DPI as a per-card minimum: lower-resolution artwork is enlarged directly once, while artwork already at or above the minimum retains its native resolution. No upscaling retains the lower-of-source-and-selected-DPI ceiling.
- Clarified the DPI control labels, Upscaling help, Guide, and README. The 1400 DPI default, shortcuts, and printed card dimensions remain unchanged. Preview images are separate from export processing, original source files are unchanged, and higher-resolution output may create larger PDFs.

## [1.0.16] - 2026-11-04

### Fixed

- Fixed mostly translucent PNG artwork becoming invisible when bleed was generated, in both previews and PDF exports.
- Refreshed derived image caches so previously imported artwork uses the corrected processing automatically.

### Added

- Drag images from Finder or File Explorer onto the sheet to add them to the next available tiles. Multiple images are supported, with a visible drop highlight and existing cards retained.
- Added Recent PDF downloads immediately to the right of the light/dark mode button. It keeps the last 20 completed PDFs on this device, shows a notification for new saves, and opens the containing folder when a PDF is clicked.
- Updated the Guide for drag-and-drop uploads and recent PDF downloads.

## [1.0.15] - 2026-10-31

### Changed

- Removed the settings gear and bleed-mode dropdown from Upload Images, keeping the parent-folder shortcut.
- Renamed My Uploads to Manage Uploads.
- Removed automatic bleed detection from image uploads and processing. New uploaded artwork starts with no built-in source bleed; bleed is configured manually in the right Settings column.
- Added manual source-bleed controls on the right for selected uploaded artwork, with an explicit action applying to all copies in the current project and Undo/Redo support.
- Respected manually entered 0 mm source bleed, and corrected cache/import handling so explicit source-bleed choices take effect immediately.
- Updated the Guide for the simplified upload workflow and manual bleed controls.

## [1.0.14] - 2026-10-31

### Changed

- Made the zoom minus and plus symbols red, with visible button backgrounds on hover and keyboard focus in light and dark mode.
- Added a native desktop image picker that remembers the last confirmed upload folder and an Upload from parent folder shortcut beside Upload Images. The shortcut reaches neighbouring card folders without navigating again from the top.
- Updated the Guide with the folder shortcut, native picker navigation keys, and zoom appearance. macOS starts a new Back/Forward history when each native picker opens; the parent-folder shortcut works independently of that history.

## [1.0.13] - 2026-10-31

### Fixed

- Preserved transparent and partially transparent PNG pixels in previews and exports when no new bleed is generated. Rounded uploaded corners no longer become opaque square corners at zero bleed.
- Refreshed derived image and effect caches so saved artwork uses the corrected transparency processing without re-uploading originals.

### Changed

- Clarified printed card dimensions, transparent corners, generated bleed, and cutting-guide shapes in the Guide. Positive generated bleed retains its existing square print margin.

## [1.0.12] - 2026-10-31

### Changed

- Changed the lower-left back arrow to remove only the most recently added card and its linked back, without undoing setting changes. Its label is now Remove last card.
- Preserved addition order independently of tile rearrangement. Existing cards use their saved sheet order as the initial removal order.
- Kept keyboard Undo and Redo for history actions, including restoring removed cards and changing settings.
- Updated the Guide to distinguish the back arrow, Duplicate arrow, and keyboard history actions.

## [1.0.11] - 2026-10-30

### Changed

- Replaced the hover zoom slider with always-visible transparent minus and plus buttons, with the current zoom percentage centered beneath them.
- Changed the lower-left right curved arrow to duplicate the last card into the next tile, using the same action as Duplicate. The left arrow remains Undo; keyboard Redo remains available.
- Updated the Guide with the zoom controls, zoom shortcuts, and curved-arrow actions.

## [1.0.10] - 2026-10-30

### Changed

- Moved Clear Cards directly below Duplicate in the Upload column, with its confirmation warning retained. Test Image now follows Clear Cards.
- Made Lanczos the default upscaling method for factory settings and new projects without personal defaults. Saved upscaling choices are retained.
- Updated the Guide to explain the new button order, clearing cards, and default upscaling method.

## [1.0.9] - 2026-10-30

### Changed

- Renamed the support button to Donate and centered it at the top of the application, retaining its hover halo and donation links.
- Duplicate remains non-clickable and grey when there is no card artwork to copy, and becomes green to match Export to PDF when available.
- Test Image is purple to match Export Card Images.
- Updated the Guide's Quick start, card actions, calibration-sheet instructions, and donation information.

## [1.0.8] - 2026-10-30

### Added

- Duplicate below Upload Images copies the last card on the current sheet into the next tile, retaining artwork, edits, and its linked back.
- Test Image below Duplicate adds a bundled Hypes_Market calibration card on every click, with no image download required.
- A pin button immediately left of the theme button keeps the desktop app above other ordinary windows on macOS and Windows. Click again to unpin; new app sessions start unpinned.
- The new card actions support Undo and Redo, and the Guide explains the new controls.

## [1.0.0] - 2026-02-22

### Changes

- 22844974 fix: align guides (#182)
- 4e2661c1 feat: upload library, release:major
- 0a755a11 fix: export enhancement effect to pdf (#178)
- abcb1eb1 fix: colorpicker going null on some cases
- 3412c7c6 added tips for silouhette registration marks
- a68cb900 fix: resolve failing unit tests (#166)
- 99b722ee fix: replace back art and update release to tagged only (#164)
- 44bdd528 feat: set filter and adjust card back preview  (#162)
- 5c6e74a8 chore: bump version to 0.0.2 (#160)
- 6638f326 fix: have release automation just run on serate branch, will need manual PRs/merge (#159)
- 4ae0eace feat: add Silhouette Cameo print & cut support (#153)
- 94d3a619 fix: cards with built in bleed had double trim applied (#156)
- 4d1ecb8c fix: improve import language settings (#154)
- 42f3f02f feat: auto detect built in bleed (#152)
- f54384c1 feat: export displayed (#150)
- 06ac5a11 fix: print population, dfc linking, search reliability (#149)
- 86e1f1cc fix: mixed content (#146)
- c8c0e9ac fix: correctly trim bleed for cards with built in bleed on export (#145)
- 7f91c137 fix: bleed generation uses built in bleed for pdf (#141)
- 58313a3e fix: cut guide and darken pixels settings for PDF export (#139)
- a471af59 fix: dfc card back replaces correctly after replacing error card (#135)
- d00b5364 fix: make blank cardback load correctly (#134)
- c41014a5 fix: update prerender to not include localhost in output (#133)
- c6390163 feat: add SEO improvements for better Google indexing (#131)
- 323ca7cb fix: make sure editor sliders are visible (#130)
- 13da1923 table migrations
- 620a20f5 minor fix to create cardback folder if it does not exist
- 14e645c6 Fix/cleanup bundle (#127)
- e1dd1c35 feat: add project switch/sharing, unifiy import infra, plus more (#126)
- 4804a92c feat: back face specific offset (#122)## [0.1.0] - 2026-02-08

### Changes

- 44bdd528 feat: set filter and adjust card back preview  (#162)
- 5c6e74a8 chore: bump version to 0.0.2 (#160)
- 6638f326 fix: have release automation just run on serate branch, will need manual PRs/merge (#159)
- 4ae0eace feat: add Silhouette Cameo print & cut support (#153)
- 94d3a619 fix: cards with built in bleed had double trim applied (#156)
- 4d1ecb8c fix: improve import language settings (#154)
- 42f3f02f feat: auto detect built in bleed (#152)
- f54384c1 feat: export displayed (#150)
- 06ac5a11 fix: print population, dfc linking, search reliability (#149)
- 86e1f1cc fix: mixed content (#146)
- c8c0e9ac fix: correctly trim bleed for cards with built in bleed on export (#145)
- 7f91c137 fix: bleed generation uses built in bleed for pdf (#141)
- 58313a3e fix: cut guide and darken pixels settings for PDF export (#139)
- a471af59 fix: dfc card back replaces correctly after replacing error card (#135)
- d00b5364 fix: make blank cardback load correctly (#134)
- c41014a5 fix: update prerender to not include localhost in output (#133)
- c6390163 feat: add SEO improvements for better Google indexing (#131)
- 323ca7cb fix: make sure editor sliders are visible (#130)
- 13da1923 table migrations
- 620a20f5 minor fix to create cardback folder if it does not exist
- 14e645c6 Fix/cleanup bundle (#127)
- e1dd1c35 feat: add project switch/sharing, unifiy import infra, plus more (#126)
- 4804a92c feat: back face specific offset (#122)
- a88fb73d fix: Correct brightness scaling (#120)
- ea75dafb fix: artwork modal fixes and UI/UX improvments
- 8475351d fix: improve DFC handling with custom cards
- 9180484c feat: improve token support to enable token import, search, and replace
- abbf9b7e feat: Add automatic token import linked from cards
- e484b31c fix: add back source grouping
- 95bb7971 fix: filter bar settings stay the same when navigating between cards# Changelog

## [0.0.2] - 2026-02-07

### Changes

- 6638f326 fix: have release automation just run on serate branch, will need manual PRs/merge (#159)
- 4ae0eace feat: add Silhouette Cameo print & cut support (#153)
- 94d3a619 fix: cards with built in bleed had double trim applied (#156)
- 4d1ecb8c fix: improve import language settings (#154)
- 42f3f02f feat: auto detect built in bleed (#152)
- f54384c1 feat: export displayed (#150)
- 06ac5a11 fix: print population, dfc linking, search reliability (#149)
- 86e1f1cc fix: mixed content (#146)
- c8c0e9ac fix: correctly trim bleed for cards with built in bleed on export (#145)
- 7f91c137 fix: bleed generation uses built in bleed for pdf (#141)
- 58313a3e fix: cut guide and darken pixels settings for PDF export (#139)
- a471af59 fix: dfc card back replaces correctly after replacing error card (#135)
- d00b5364 fix: make blank cardback load correctly (#134)
- c41014a5 fix: update prerender to not include localhost in output (#133)
- c6390163 feat: add SEO improvements for better Google indexing (#131)
- 323ca7cb fix: make sure editor sliders are visible (#130)
- 13da1923 table migrations
- 620a20f5 minor fix to create cardback folder if it does not exist
- 14e645c6 Fix/cleanup bundle (#127)
- e1dd1c35 feat: add project switch/sharing, unifiy import infra, plus more (#126)
- 4804a92c feat: back face specific offset (#122)
- a88fb73d fix: Correct brightness scaling (#120)
- ea75dafb fix: artwork modal fixes and UI/UX improvments
- 8475351d fix: improve DFC handling with custom cards
- 9180484c feat: improve token support to enable token import, search, and replace
- abbf9b7e feat: Add automatic token import linked from cards
- e484b31c fix: add back source grouping
- 95bb7971 fix: filter bar settings stay the same when navigating between cards
- e37454d3 fix: make sure search uses selected art source
- 7bab0b99 fix: have release automation make a separate branch and pr instead of direct to main
