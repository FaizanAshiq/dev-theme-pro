# Change Log

All notable changes to "Dev Theme Pro" will be documented in this file.

---

## [0.6.2] - 2026-04-12

### Added

- **Built-in delimited file coloring** — CSV, TSV, PSV, DSV, SSV, and TAB files now color columns directly in the editor, so structured text stays readable without extra extensions

### Fixed

- **Preview right-click menus stay out of the way** — Markdown, table, and snapshot previews no longer surface the default copy/cut/paste webview menu
- **Export progress is now visible inside the preview** — longer copy and export actions now show an animated in-panel loading notice before switching to the final success message
- **Code Snapshot now waits for a real selection** — the panel opens with a clear prompt instead of grabbing the whole file, and it works from more editor types
- **Snapshot exports are tighter and cleaner** — copied and saved images now keep a slimmer frame with a softer accent border around the card
- **Mermaid actions stay visible** — diagram copy and export buttons remain available in the preview instead of hiding until hover
- **Markdown PDF export includes Mermaid diagrams again** — rendered diagrams now stay in the final PDF instead of disappearing during export

### Changed

- **Table tools cover more delimited formats** — preview and export commands now follow the same flow for additional structured text files beyond the original CSV, TSV, and PSV set

---

## [0.6.1] - 2026-04-11

### Added

- **Solar variants** — the warmer accent now ships in both Mist and Void

### Changed

- **Previews follow the active variant** — Markdown, tables, Mermaid exports, and code snapshots now match Ocean, Nebula, or Solar
- **Variant balance was refined** — Solar, Void, and Mist each got calmer contrast tuning for easier daily use

---

## [0.6.0] - 2026-04-11

### Added

- **Open With preview support** — Markdown and table files can open straight into Dev Theme Pro previews
- **More quick entry points** — Explorer and tab menus now expose preview shortcuts in more places

### Changed

- **Preview naming is more consistent** — preview actions now use clearer Dev Theme Pro labels across menus and pickers

---

## [0.5.9] - 2026-04-11

### Added

- **Built-in document tools** — Markdown preview, table preview, HTML/PDF export, Mermaid support, and code snapshots all landed in one release
- **Navigation helpers** — table of contents, presentation mode, and cleaner action menus make long docs easier to work with
- **Table utilities** — sorting, filtering, resizing, and multiple export options arrived for delimited data files

### Fixed

- **Mermaid exports hold their shape better** — larger diagrams keep more of their frame and spacing across PNG and PDF output

### Changed

- **Diagram actions stay inside the preview** — Mermaid export is handled from the preview UI instead of duplicated elsewhere

---

## [0.5.8] - 2026-03-20

### Fixed

- **Settings and Source Control read more cleanly** — focus rows, refs, and history details were softened for easier scanning

---

## [0.5.7] - 2026-03-14

### Fixed

- **Inputs and floating panels feel more consistent** — chat, search, Settings, and layered surfaces now separate more clearly across variants

### Changed

- **Theme selection is simpler** — the lineup now centers on Mist and Void with cleaner focus and hover states

## [0.5.6] - 2026-03-07

### Fixed

- **Layered UI is easier to read** — overlapping inputs, hover surfaces, autocomplete, and other floating elements now separate more cleanly

### Changed

- **Variant naming and highlights were cleaned up** — Pure replaced Zen, and shared selection states now feel more unified

---

## [0.5.5] - 2026-03-01

### Added

- **Pure and Wire variants** — each accent/depth combo now comes in both borderless and bordered styles

### Changed

- **The lineup was redesigned** — the extension shifted to a cleaner Ocean and Nebula family with stronger accent balance

---

## [0.5.4] - 2026-02-22

### Fixed

- **Panel focus borders are gone** — large containers now behave more like native VS Code panels

---

## [0.5.3] - 2026-02-22

### Changed

- **Release packaging was cleaned up** — publishing and build scripts were corrected behind the scenes

---

## [0.5.2] - 2026-02-22

### Fixed

- **Accent focus states now show properly** — focused controls and accent-driven buttons read more clearly across the UI

### Added

- **Python highlighting and wider accent coverage** — language color support and UI accent reach both expanded noticeably

### Changed

- **Front-end syntax colors were refined** — HTML, CSS-family files, and fallback text became more balanced

---

## [0.5.1] - 2026-02-22

### Changed

- **Core syntax colors were refined** — major token groups separate more clearly, with cleaner emphasis rules

### Added

- **More language details are covered** — smaller syntax cases now highlight more consistently

---

## [0.5.0] - 2026-02-15

### Added

- **12 theme variants** — four accents and three depths landed in the first big lineup expansion
- **Floating surfaces adapt by variant** — panels and secondary surfaces started following the active depth

### Changed

- **Decorator and constructor styling was corrected** — framework-heavy code reads more cleanly

### Fixed

- **Floating widgets now match the selected depth** — popups and overlays stay closer to the chosen variant

---

## [0.4.0] - 2026-02-15

### Added

- **4 accent variants** — Ocean, Nebula, Emerald, and Amber launched
- **Accent color reached more of the UI** — bars, badges, buttons, scrollbars, and editor chrome became more cohesive
- **Semantic highlighting arrived** — files color in faster and component tags read more distinctly

### Fixed

- **Color flashes and a few rough UI tones were corrected** — opening files and scanning the interface feels steadier

### Improved

- **Git and list states are clearer** — file trees and source control details got easier to scan

---

## [0.3.0] - 2026-02-15

### Fixed

- **Core UI visibility issues were fixed** — inputs, selections, badges, and several harsh UI colors were cleaned up
- **Inlay hints blend better** — hint backgrounds no longer create harsh dark slots

### Added

- **Semantic highlighting support** — richer language-server coloring was enabled

---

## [0.2.3] - 2025-12-31

### Improved

- **Marketplace presentation was improved** — the README was reorganized for a cleaner first impression

---

## [0.2.2] - 2025-12-29

### Improved

- **Marketplace assets were optimized** — screenshots became lighter and cleaner for faster loading

---

## [0.2.1] - 2025-12-29

### Fixed

- **Publishing reliability improved** — release automation became more dependable

---

## [0.2.0] - 2025-12-29

### Added

- **Automated marketplace publishing** — releases can now ship through GitHub Actions

---

## [0.1.0] - 2025-12-29

### Added

- **Initial release** — Dev Theme Pro launched with its first dark-theme foundation

### Added

- Initial release of Dev Theme Pro
- Dark theme with colorful, high-contrast syntax highlighting
- Optimized for JavaScript, TypeScript, Python, HTML, CSS, and more
- Custom UI colors for a cohesive dark editor experience
