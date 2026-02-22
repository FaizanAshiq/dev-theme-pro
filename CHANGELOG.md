# Change Log

All notable changes to "Dev Theme Pro" will be documented in this file.

---

## [0.5.3] - 2026-02-22

### Fixed

- Panel and tree view containers (Explorer, Source Control, etc.) no longer show a bright accent border when clicking on empty whitespace — focus ring is now subtle and unobtrusive while remaining visible on inputs and interactive controls

### Changed

- CI publishing workflow updated to use `npx @vscode/vsce` directly — removes the need for a separate global install step

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
