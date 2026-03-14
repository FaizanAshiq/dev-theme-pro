# Change Log

All notable changes to "Dev Theme Pro" will be documented in this file.

---

## [0.5.7] - 2026-03-14

### Fixed

- **Input fields now match across Pure and Wire** — chat boxes, search inputs, and other text fields now use the same depth-based surface in both styles, so they feel consistent no matter which variant you pick
- **Input outlines are gone** — text fields no longer draw borders or focus rings, keeping search, chat, and settings inputs visually clean
- **Floating windows stand apart more clearly** — overlays now cast a stronger shadow, making layered UI easier to separate from the editor behind it
- **Pure overlays read more cleanly over code** — floating windows in Pure mode now cast a much deeper shadow so they no longer blend into the editor text underneath
- **Inputs and floating widgets have clearer separation** — Mist inputs now sit a little deeper, Void inputs a little brighter, and floating pickers/widgets are lifted slightly so each layer reads more distinctly
- **Settings inputs now follow the theme surface tone** — the search box, dropdowns, and text inputs in Settings now use the same theme-controlled input background as the rest of the UI
- **Checkboxes and UI lines now match the theme surface system** — checkbox fills now use the shared control surface, and border intensity across Wire and Pure is driven from one central set of per-variant values for a cleaner, more consistent frame

### Changed

- **Theme lineup now focuses on Mist and Void** — the style split has been removed for now, leaving one Mist and one Void theme per accent for a simpler picker
- **Border tuning is now easier to edit directly** — each depth now carries its own chrome controls in the generator, so line, border, and guide strength can be adjusted in one place while you iterate
- **Theme picker now groups by depth** — Mist variants are listed together first, followed by Void, so the chooser reads Ocean Mist, Nebula Mist, Ocean Void, Nebula Void
- **Focused rows and hover popups read more clearly** — active list states now use richer accent-tinted backgrounds, and hover cards sit slightly more lifted so focused and hovered actions are easier to pick out

## [0.5.6] - 2026-03-07

### Fixed

- **Input fields in chat and overlapping panels** — input boxes no longer look faded or washed out when layered inside panels like the AI chat view
- **Floating panel shadows in Zen variants** — the command palette, suggestion dropdown, hover tooltips, and similar floating panels now cast a stronger shadow, making them easier to distinguish from the editor behind them
- **Breadcrumb shadow removed** — the shadow line below the breadcrumb navigation bar is gone for a cleaner, flatter look
- **Autocomplete dropdown border in Zen** — the suggestion popup now has a visible border in Zen mode, just like Wire
- **Inlay hint and hover popup borders** — type hints and hover tooltips now always show a subtle border regardless of the active style variant

### Changed

- **Input field contrast** — in Zen variants, inputs are now tinted for better separation from the editor: slightly darker in Mist and slightly lighter in Void, matching the background depth
- **Selection highlight unified across all areas** — the focused/selected row in the file tree, command palette, and autocomplete dropdown now all use the same accent-tinted highlight, giving the UI a consistent, intentional look
- **Theme variant names refreshed** — the borderless style is now called **Pure** (was Zen), sorting it before Wire in the picker. Theme icons updated: ☁️ Mist, ✨ Void, 🔮 Nebula

---

## [0.5.5] - 2026-03-01

### Added

- **Zen variants** — a borderless, minimal edition of every theme. All UI borders and separator lines are removed, leaving a clean canvas. The active indent guide and active tab indicator are preserved for orientation
- **Wire variants** — the fully-bordered counterpart to Zen, making the style choice explicit for each accent and depth

### Changed

- **Theme lineup redesigned** — consolidated to two carefully chosen accents:
  - 🌊 **Ocean** (blue, `#0083CF`)
  - 🌌 **Nebula** (purple, `#864DEF`)
    Each accent ships with four depth/style variants: Mist Wire, Mist Zen, Void Wire, Void Zen
- **Accent text vs accent background split** — accent colors used as foreground (terminal ANSI blue/cyan, links, breadcrumbs, search highlights, symbol icons) are now independently brightened for readability on dark backgrounds, while background usages (buttons, badges, scrollbars, selections) retain the original deeper tone
- **Floating UI surfaces elevated in Zen variants** — command palette, quick input, menus, hover widgets, suggest widget, and dropdowns use a subtly lighter background in Zen to compensate for the absence of borders
- **Input fields tinted in Zen variants** — a near-invisible tint distinguishes interactive fields from the editor background
- **Comment brightness increased** — comment color slightly brightened across all variants for improved readability

---

## [0.5.4] - 2026-02-22

### Fixed

- Panel and tree view containers (Explorer, Source Control, etc.) no longer show a focus border when clicked — large view containers now behave like native panels, with the focus ring reserved for interactive controls like inputs and buttons

---

## [0.5.3] - 2026-02-22

### Changed

- CI publishing workflow updated to use `npx @vscode/vsce` directly — removes the need for a separate global install step
- npm scripts corrected — `generate` and `pack` now point to the correct `src/generate.js` path and use `npx @vscode/vsce`

---

## [0.5.2] - 2026-02-22

### Fixed

- **Focus borders now correctly show the accent color** — focused inputs, dropdowns, buttons, and widgets all highlight with your chosen accent. Previously focus borders were invisible across the entire UI
- Extension marketplace buttons now use the full accent color instead of a faded tint
- Toolbar hover and active states were not using accent — now consistent with the rest of the UI

### Added

- **Python syntax highlighting** — comprehensive coverage added:
  - Keywords and control flow (`if`, `for`, `with`, `yield`, `async`, etc.)
  - Built-in functions (`print`, `len`, `range`, `super`, `isinstance`, etc.)
  - Built-in types (`int`, `str`, `list`, `dict`, `bool`, etc.)
  - Class names, function and method definitions
  - Decorators (`@property`, `@staticmethod`, custom decorators)
  - Magic methods (`__init__`, `__str__`, `__repr__`, etc.) and magic variables (`__name__`, `__all__`, etc.)
  - `self` and `cls` parameters
  - Exception types, `True` / `False` / `None` constants
  - Type annotations and f-string format specs

- **Broader UI accent coverage** — the following UI elements now correctly pick up the accent color:
  - Checkboxes (background, foreground, border)
  - Toolbar hover and active backgrounds
  - Settings editor focused row border
  - Search editor text input border
  - Extension button separator and foreground
  - Input option hover background (now subtler, was too heavy)

### Changed

- **HTML highlighting improvements:**
  - Tag punctuation (`<`, `>`) de-emphasized to reduce visual noise
  - Attribute `=` signs dimmed — distinct from attribute names and values
  - HTML entities colored consistently as values
  - `<!DOCTYPE>` de-emphasized as boilerplate
  - Embedded `<script>` and `<style>` tag names colored as keywords to signal a language boundary
  - Quote punctuation around attribute values colored consistently with string quotes

- **CSS / SCSS / Less highlighting improvements:**
  - Property names given a distinct color — no longer the same as generic variables
  - Units (`px`, `em`, `rem`, `%`, `vh`, etc.) individually colored
  - At-rules (`@media`, `@keyframes`, `@import`, `@mixin`, etc.) colored as keywords
  - `!important` colored red and bold
  - CSS functions (`rgb()`, `var()`, `calc()`, `linear-gradient()`, etc.) colored green
  - CSS custom properties (`--variable`) colored distinctly with italic
  - SCSS variables (`$var`) and Less variables (`@var`) colored as module references
  - SCSS interpolation brackets `#{...}` colored as keywords
  - ID selectors fixed — previously mapped to the wrong scope
  - Class selector color slightly desaturated for a more balanced palette
  - Vendor-prefixed property names covered

- Default fallback text color updated to a neutral grey — plain unscoped text now looks balanced across all languages

---

## [0.5.1] - 2026-02-22

### Changed

- Core syntax palette tuned — class/type, function, and keyword hues adjusted for improved contrast and visual separation
- Reduced over-use of bold — variables, properties, and keywords are no longer bold by default, keeping bold reserved for truly important distinctions (classes, decorators, `!important`)
- Updated bracket pair colors, symbol icons, chart colors, and terminal ANSI palette to match the refined hues

### Added

- Optional chaining (`?.`) now correctly highlighted as a keyword operator
- Type annotation operators, comma separators, and key-value separators all highlighted consistently
- Single-quoted strings and their surrounding punctuation now covered
- JSON values no longer incorrectly rendered bold
- `extends` / `implements` inheritance separators now language-agnostic

---

## [0.5.0] - 2026-02-15

### Added

- **12 theme variants** — choose your accent and background depth independently:
  - Accents: 🌊 Ocean · 🌌 Nebula · 💎 Emerald · ✨ Amber
  - Backgrounds: 🌅 Dusk (lighter) · 🌙 Night (default) · 🕳️ Void (darkest)
- Floating panels and inlay hints automatically use a subtly elevated background tone per variant

### Changed

- Decorators are now blue and bold — visually distinct from functions (green) and classes (yellow)
- React and Vue component tags styled consistently with decorators (blue bold)
- Class constructors no longer incorrectly colored as functions

### Fixed

- Floating widget backgrounds now correctly reflect the current background depth variant

---

## [0.4.0] - 2026-02-15

### Added

- **4 accent color variants**: 🌊 Ocean, 🌌 Nebula, 💎 Emerald, ✨ Amber
- Full accent propagation across all UI surfaces — status bar, activity bar, badges, buttons, scrollbars, diff gutter, minimap, breadcrumbs, and more
- Rich semantic highlighting for near-instant coloring on file open (no color flash)
- React and Vue component tag styling (blue bold)
- New extension icon

### Fixed

- Color flash on file open eliminated — TextMate and semantic token colors now aligned
- Terminal ANSI magenta corrected to purple
- Scrollbar, selection highlight, and inlay hint color fixes

### Improved

- Git decoration colors redesigned for clarity
- File list selection and hover states modernized
- Focus border balance improved across the UI

---

## [0.3.0] - 2026-02-15

### Fixed

- Input box borders now visible in Copilot Chat, the Search panel, Find widget, and all other inputs
- Find match highlights — current match and other matches are now clearly distinct
- Badge pills now have a visible background (were transparent — text appeared floating)
- List hover and active selection highlights now clearly visible
- Settings modified indicator no longer blends into the foreground text
- Inactive selection highlight fixed (previously had a red tint, looked like an error)
- Editor rulers no longer blindingly bright at full opacity
- Panel drop overlay, menu separators, and list hover backgrounds all corrected
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
