# Change Log

All notable changes to "Dev Theme Pro" will be documented in this file.

## [0.5.1] - 2026-02-22

### Changed

- Refined core palette — class/type yellow (`#C2B776` → `#BAAF6D`), function green (`#56C98E` → `#45BF80`), keyword purple (`#A46FED` → `#B070FF`) for better contrast
- Removed excessive **bold** styling from semantic tokens (variables, properties, keywords, decorators)
- Focus border made transparent globally; `input.focusBorder` and `dropdown.focusBorder` now carry the accent color independently
- Updated bracket highlight, symbol icon, chart, and terminal ANSI magenta colors to match refined palette

### Added

- `punctuation.accessor.optional` (optional chaining `?.`) added to keyword scopes
- Comma separators, type annotations (`keyword.operator.type.annotation`), and key-value separators added to punctuation scopes
- Enhanced string scopes with `string.quoted.single` and `punctuation.definition.string`
- Explicit no-bold (`fontStyle: ""`) for all JSON-specific token rules + general `source.json` scope
- Made `punctuation.separator.inheritance` language-agnostic (was PHP-only)

## [0.5.0] - 2026-02-15

### Added

- **12 theme variants** — 4 accents × 3 background depths:
  - 🌊 Ocean, 🌌 Nebula, 💎 Emerald, ✨ Amber
  - 🌅 Dusk (lightest), 🌙 Night (default), 🕳️ Void (darkest)
- Background depth system with `lighten()` helper — `bgFloat` and `inlayBg` auto-derived per variant
- Emoji-labeled theme names for easy identification in the theme picker

### Changed

- **Decorators are now blue** (`#6194FC`, bold) — distinct from functions/methods (green `#56C98E`)
- Narrowed TextMate function scopes to avoid coloring constructors in `new X()` as green
- Removed base `function` semantic token — lets TypeScript class constructors fall through to class color (yellow)
- Added TS-specific decorator scope (`source.ts meta.decorator.ts meta.function-call.ts entity.name.function.ts`)
- React/Vue components styled blue bold (matching decorators)
- Classes, types, interfaces, enums remain yellow (`#C2B776`, bold)

### Fixed

- `editorWidget.background` now uses elevated `bgFloat` (derived per variant) instead of hardcoded value
- Widget border opacity increased for better visibility on floating panels

## [0.4.0] - 2026-02-15

### Added

- **4 accent variants**: Ocean, Nebula, Emerald, Amber — same syntax, different UI accents
- JS theme generator (`src/generate.js`) — single source of truth for all variants
- 469 workbench color keys with full accent propagation
- 42 semantic token entries for zero-flash coloring
- React/Vue component tag styling
- New icon

### Changed

- Accent color system — all UI colors derive from single accent hex + opacity
- Minified JSON output, generator source gitignored
- `npm run pack` auto-generates before packaging

### Fixed

- Zero-flash on file open — TextMate and semantic tokens aligned
- Terminal ANSI magenta corrected to purple
- Inlay hint, scrollbar shadow, selection highlight fixes
- Removed dead TextMate scopes and duplicates

### Improved

- Git decoration colors redesigned
- Focus borders rebalanced
- File list selection modernized

## [0.3.0] - 2026-02-15

### Fixed

- Fixed input box border disappearing on focus in Copilot Chat and all other input fields (`focusBorder` was transparent)
- Fixed editor ruler being full opacity (blindingly bright)
- Fixed panel section drop overlay being fully opaque
- Fixed menu separators being full opacity white bars
- Fixed list hover producing zero visual change (same as background)
- Fixed list active selection having no background highlight
- Fixed current find match being nearly invisible (pure black on dark bg)
- Fixed find match highlights being too faint (~6% opacity)
- Fixed find matches being invisible in overview ruler scrollbar
- Fixed badge backgrounds being transparent (floating text, no pill)
- Fixed inactive selection using red tint (looked like error highlights)
- Fixed settings modified indicator blending in with foreground
- Fixed inlay hint background creating harsh dark slots
- Fixed duplicate `keyword.control.flow` scopes (appeared 3 times)

### Added

- Enabled `semanticHighlighting: true` for richer language-server-based coloring
- Added modern `extensionButton.background` / `hoverBackground` keys alongside deprecated equivalents
- Added SUGGESTIONS.md with 200+ missing modern VS Code color keys to implement
- Added IMPROVEMENTS.md documenting all fixes and review notes
- Git tagging for release versioning

### Improved

- Renamed misleading tokenColor rule "Brackets" to "Strings"
- Renamed four duplicate "Shell - Command" rules to distinct names
- Fixed "CSS ID's" typo to "CSS IDs"
- Added `name` property to default token fallback rule
- Updated copyright year to 2026
- Updated LinkedIn profile link

## [0.2.3] - 2025-12-31

### Improved

- Enhanced README with marketplace-ready formatting and structure
- Added catchy header with emoji and cleaner description
- Streamlined installation instructions with marketplace method first
- Added descriptive captions to all screenshot previews
- Simplified customization section for better user experience
- Updated call-to-action section for better engagement
- Improved badge layout and added MIT license badge

## [0.2.2] - 2025-12-29

### Improved

- Optimized screenshot images for faster loading (77% size reduction)
- Converted screenshots from PNG to JPEG format for better performance
- Updated sample files with consistent formatting for better screenshots

## [0.2.1] - 2025-12-29

### Fixed

- Fixed GitHub Actions workflow publishing issues
- Improved workflow reliability and error handling

## [0.2.0] - 2025-12-29

### Added

- GitHub Actions workflow for automated publishing
- Automated extension packaging and marketplace publishing

### Fixed

- Updated copyright dates to 2025
- Improved workflow reliability

## [0.1.0] - 2025-12-29

### Added

- Initial release of Dev Theme Pro
- "Dev Theme Pro Smooth" dark theme variant
- Colorful syntax highlighting for improved code readability
- Optimized for JavaScript, TypeScript, Python, HTML, CSS, and more
- Custom UI colors for a cohesive dark experience
