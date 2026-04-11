# Change Log

All notable changes to "Dev Theme Pro" will be documented in this file.

---

## [0.6.1] - 2026-04-11

### Added

- **Solar accent variants** — the warm yellow option now ships in both Mist and Void, so you can keep the same accent while choosing between the lighter and deepest dark base

### Changed

- **Previews now match the active variant** — Markdown, tables, Mermaid exports, and code snapshots now follow Ocean, Nebula, or Solar instead of staying locked to one accent
- **Solar is a little softer on the eyes** — the yellow accent was darkened slightly so highlights feel smoother without changing the overall character of the variant
- **Void now uses the deepest dark base** — the old deepest canvas is now the standard Void backdrop, with inputs kept slightly lighter so fields still separate cleanly
- **Mist inputs are now pure black** — form fields and similar controls sit darker against the lighter Mist canvas for stronger separation

---

## [0.6.0] - 2026-04-11

### Added

- **Open With support for every preview type** — Markdown, CSV, TSV, and PSV files now surface a Dev Theme Pro preview option in VS Code's Open With flow
- **Right-click preview shortcuts in more places** — Explorer and editor-tab menus now let you reopen supported files straight into the matching Dev Theme Pro preview

### Changed

- **Preview labels are now more consistent** — Markdown and table previews now use the same 🔮 Dev Theme Pro naming across menus and picker entries

---

## [0.5.9] - 2026-04-11

### Added

- **Built-in Markdown preview** — open Markdown in a Dev Theme Pro reading view with matching typography, spacing, and colors
- **Flexible preview opening options** — open the preview beside your file, in the current editor, or through Open With
- **PDF and HTML export for Markdown** — save polished documents straight from the preview toolbar
- **Mermaid-ready Markdown docs** — diagrams render inside the preview, download as PNG, and export to PDF without blank spacer pages above them
- **Theme-matched document previews** — tables, code blocks, task lists, and long-form docs now read like part of the theme instead of a generic renderer
- **Table of contents sidebar** — jump through long documents with a collapsible heading navigator
- **Presentation mode** — turn heading-based sections into slides with keyboard navigation
- **CSV and TSV preview** — inspect data files with sorting, filtering, column resize, and row numbers
- **Table export tools** — save data previews as PDF, PNG, or standalone HTML
- **Code snapshot tool** — capture selected code as a styled PNG with a live preview before saving
- **Whole-file snapshot fallback** — if nothing is selected, the snapshot tool captures the entire file automatically
- **Theme-matched snapshots** — exported images use Dev Theme Pro styling instead of a generic dark theme
- **Cleaner snapshot presentation** — snapshots use a minimal filename bar for a more refined look
- **Unified right-click tools menu** — all Dev Theme Pro actions now live under one submenu in the editor context menu
- **Cleaner preview interactions** — preview export actions work reliably, and browser-style context menus stay disabled inside previews
- **Faster-scanning commands** — toolbar actions, menus, and command palette entries now use clearer icons and emoji labels

### Fixed

- **Large Mermaid exports keep the full diagram frame** — wide diagrams no longer lose the right edge during image export
- **Mermaid PNG exports stay sharper on bigger diagrams** — export quality now scales more evenly for dense, wide layouts
- **Wide Mermaid diagrams fit exported PDFs more reliably** — large diagrams are now rendered to the printable page width before PDF export so the right side is less likely to get cut off
- **PDF Mermaid diagrams keep more even side spacing** — wide diagrams now normalize their internal SVG bounds before export so the right side stays aligned more like the left

### Changed

- **Diagram download now stays in the preview itself** — the editor right-click menu no longer duplicates the Mermaid export action
- **Mermaid PNG downloads now save at a lighter size** — diagram exports still adapt to each layout, but now come out at roughly half the previous resolution

---

## [0.5.8] - 2026-03-20

### Fixed

- **Settings rows no longer show a focus border** — removed the accent outline from the active row in the Settings editor
- **Source Control history is easier to scan** — branch refs, remote refs, and graph hover labels now read more clearly at a glance

---

## [0.5.7] - 2026-03-14

### Fixed

- **Inputs feel more consistent across the UI** — chat, search, Settings, and other text fields now share the same depth-based surface treatment in Pure and Wire, with outlines removed for a cleaner look
- **Floating surfaces separate more clearly** — stronger shadows, deeper Mist inputs, brighter Void inputs, and slightly lifted pickers/widgets make layered UI easier to read
- **Settings and controls now follow the same surface system** — Settings inputs, checkbox fills, and surrounding UI lines now use the shared theme surface and border tuning for a cleaner, more consistent frame

### Changed

- **Theme selection is simpler** — the lineup now focuses on Mist and Void, grouped by depth in the picker as Ocean Mist, Nebula Mist, Ocean Void, and Nebula Void
- **Focused rows and hover popups read more clearly** — active list states use richer accent-tinted backgrounds, and hover cards sit slightly higher above the editor

## [0.5.6] - 2026-03-07

### Fixed

- **Layered inputs no longer look washed out** — chat and other overlapping input fields now keep their intended surface contrast
- **Floating UI is easier to distinguish in Zen** — command palette, suggestions, and hover popups now use stronger separation with clearer shadows and borders where needed
- **Small visual distractions are removed** — the breadcrumb shadow is gone, while autocomplete, inlay hints, and hover popups now keep consistent borders

### Changed

- **Zen input contrast is better balanced** — inputs are now tinted to separate more clearly from the editor in both Mist and Void
- **Selection highlights are now unified** — focused rows in the tree, command palette, and autocomplete all use the same accent-tinted highlight
- **Variant naming is cleaner** — Zen is now called Pure, and the theme icons were refreshed for Mist, Void, and Nebula

---

## [0.5.5] - 2026-03-01

### Added

- **Zen variants** — a borderless version of every theme with separators removed, while keeping the active indent guide and active tab indicator for orientation
- **Wire variants** — a fully bordered counterpart to Zen for each accent and depth

### Changed

- **Theme lineup was redesigned** — the extension now centers on Ocean and Nebula, each available in Mist Wire, Mist Zen, Void Wire, and Void Zen
- **Accent usage is more readable** — accent text is brighter on dark surfaces, while accent backgrounds keep a deeper tone for buttons, badges, scrollbars, and selections
- **Zen surfaces read more clearly** — floating UI is slightly elevated, inputs carry a subtle tint, and comments are a bit brighter across all variants

---

## [0.5.4] - 2026-02-22

### Fixed

- **Panel focus borders are gone** — Explorer, Source Control, and other large containers now behave like native panels, leaving focus rings for interactive controls instead

---

## [0.5.3] - 2026-02-22

### Changed

- **Packaging and publishing scripts were corrected** — CI and npm scripts now use `npx @vscode/vsce` directly and point to the right generator path

---

## [0.5.2] - 2026-02-22

### Fixed

- **Focus borders now correctly show the accent color** — focused inputs, dropdowns, buttons, and widgets all highlight with your chosen accent. Previously focus borders were invisible across the entire UI
- **Accent-driven controls are more consistent** — marketplace buttons now use the full accent color, and toolbar hover and active states match the rest of the UI

### Added

- **Python syntax highlighting** — added broad coverage for keywords, built-ins, types, classes, functions, decorators, magic members, `self` and `cls`, constants, type annotations, and f-string format specs
- **Broader UI accent coverage** — checkboxes, toolbar states, Settings focused rows, Search input borders, extension buttons, and input option hover states now pick up the accent more consistently

### Changed

- **HTML highlighting is cleaner** — tag punctuation, `=` signs, entities, `<!DOCTYPE>`, embedded script/style tags, and attribute quote punctuation now read more consistently
- **CSS, SCSS, and Less highlighting is broader** — property names, units, at-rules, `!important`, functions, custom properties, variables, interpolation, ID selectors, class selectors, and vendor-prefixed properties now have clearer coverage and balance
- **Fallback text color is more neutral** — plain unscoped text now feels more balanced across languages

---

## [0.5.1] - 2026-02-22

### Changed

- **Core syntax colors were refined** — class, type, function, and keyword hues now separate more clearly
- **Bold is used more selectively** — variables, properties, and keywords are no longer bold by default, leaving stronger emphasis for classes, decorators, and `!important`
- **Supporting UI colors were aligned** — bracket pairs, symbol icons, charts, and terminal ANSI colors now match the refined palette

### Added

- **More syntax details are covered** — optional chaining, type annotation operators, separators, single-quoted strings, JSON values, and `extends` / `implements` now highlight more consistently

---

## [0.5.0] - 2026-02-15

### Added

- **12 theme variants** — mix four accents with three background depths: Ocean, Nebula, Emerald, and Amber across Dusk, Night, and Void
- **Floating surfaces adapt to each variant** — panels and inlay hints automatically use a subtly elevated background tone

### Changed

- **Decorators stand out more clearly** — they are now blue and bold, with React and Vue component tags styled to match
- **Constructors are colored correctly** — class constructors no longer appear as functions

### Fixed

- **Floating widget backgrounds now match the selected depth** — each variant carries the right background tone into floating UI

---

## [0.4.0] - 2026-02-15

### Added

- **4 accent variants** — Ocean, Nebula, Emerald, and Amber
- **Accent color now reaches the full UI** — status bar, activity bar, badges, buttons, scrollbars, diff gutter, minimap, breadcrumbs, and more all follow the chosen accent
- **Semantic highlighting was added** — files now color in almost instantly on open, with React and Vue component tags styled distinctly and a new extension icon included

### Fixed

- **File-open color flash is gone** — TextMate and semantic token colors now align
- **Several UI colors were corrected** — terminal magenta, scrollbars, selection highlights, and inlay hints now render more consistently

### Improved

- **Git and list states are clearer** — git decorations, file list selection and hover states, and focus border balance were all improved

---

## [0.3.0] - 2026-02-15

### Fixed

- **Core UI visibility issues were fixed** — input borders now show correctly in chat, search, find, and other inputs, and current versus other find matches are easier to distinguish
- **Selection and status states are clearer** — badge pills, list hover and active states, the Settings modified indicator, and inactive selection highlights now read properly
- **Several harsh or incorrect UI colors were corrected** — editor rulers, panel drop overlays, menu separators, and list hover backgrounds now feel balanced
- Inlay hints no longer create harsh dark slots behind them

### Added

- Semantic highlighting enabled for richer language-server-powered coloring

---

## [0.2.3] - 2025-12-31

### Improved

- README fully rewritten for the marketplace — cleaner layout, better structure, improved installation guide, descriptive screenshot captions

---

## [0.2.2] - 2025-12-29

### Improved

- Screenshot images optimized — 77% smaller file sizes for faster marketplace loading
- Screenshots converted to JPEG format
- Sample files updated for cleaner screenshots

---

## [0.2.1] - 2025-12-29

### Fixed

- Automated publishing workflow reliability improvements

---

## [0.2.0] - 2025-12-29

### Added

- GitHub Actions workflow for automated marketplace publishing

---

## [0.1.0] - 2025-12-29

### Added

- Initial release of Dev Theme Pro
- Dark theme with colorful, high-contrast syntax highlighting
- Optimized for JavaScript, TypeScript, Python, HTML, CSS, and more
- Custom UI colors for a cohesive dark editor experience
