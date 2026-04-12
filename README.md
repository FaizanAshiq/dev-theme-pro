# Dev Theme Pro

> One install. Six daily tools: a polished dark theme, Markdown preview, Mermaid support, table tools, export workflows, and shareable code snapshots.

<p align="center">
  <img src="images/icon.png" alt="Dev Theme Pro" width="120">
</p>

Dev Theme Pro is built for people who want their workspace to look better and do more without stitching together a pile of separate extensions.

## 6-in-1 Toolkit

| Tool                 | What you get                                                                                        |
| -------------------- | --------------------------------------------------------------------------------------------------- |
| **Theme**            | Six tuned dark variants with cleaner syntax contrast and a consistent workbench accent              |
| **Markdown Preview** | A styled reading view with headings, code blocks, tables, task lists, and TOC support               |
| **Mermaid Diagrams** | In-preview rendering with quick copy/export actions and reliable PDF output                         |
| **Table Preview**    | CSV, TSV, PSV, DSV, SSV, and TAB files with sorting, filtering, resize, and export                  |
| **Export Tools**     | HTML, PDF, and PNG flows that keep the Dev Theme Pro look instead of falling back to generic output |
| **Code Snapshot**    | A live snapshot panel for clean, theme-matched images you can share in seconds                      |

## Why People Keep It Installed

- **It replaces extension clutter** — theme, document preview, Mermaid workflow, table inspection, and snapshots all live in one package
- **Previews follow your active variant** — Ocean, Nebula, and Solar stay in sync across Markdown, tables, diagrams, and snapshots
- **The UI is built for real work** — table filtering, Mermaid copy/export, and PDF output are part of the daily workflow, not afterthoughts
- **Shared output looks deliberate** — exported docs, diagrams, tables, and snapshots keep the same visual system as the editor

## Theme Variants

Dev Theme Pro ships with six variants:

- **Ocean Mist** — blue accent on the lighter dark base
- **Nebula Mist** — purple accent on the lighter dark base
- **Solar Mist** — warm gold accent on the lighter dark base
- **Ocean Void** — blue accent on the deepest base
- **Nebula Void** — purple accent on the deepest base
- **Solar Void** — warm gold accent on the deepest base

If you want the fastest default: **Mist** is the easier long-session pick, while **Void** is the denser, deeper canvas.

## Installation

1. Open **Extensions** in VS Code (`Ctrl+Shift+X` / `Cmd+Shift+X`)
2. Search for **Dev Theme Pro**
3. Click **Install**
4. Open **File → Preferences → Color Theme** and choose your variant

## Markdown + Mermaid

Open any Markdown file in a reading view that feels like part of the theme instead of a generic browser page.

| Action                        | How                                                                                                      |
| ----------------------------- | -------------------------------------------------------------------------------------------------------- |
| Preview to the side           | Click the preview button in the editor title bar, or press `Cmd+K V` / `Ctrl+K V`                        |
| Preview in the current editor | Click the render button in the title bar, or press `Cmd+K Cmd+V` / `Ctrl+K Ctrl+V`                       |
| Open With picker              | Right-click the file in the Explorer and choose **Open With… → 🔮 Dev Theme Pro Markdown Preview**       |
| Right-click shortcut          | Right-click the file in the Explorer or the editor tab and choose **🔮 Open With Dev Theme Pro Preview** |

What you get:

- **Theme-matched reading layout** — headings, code blocks, tables, and long-form text feel native to the active variant
- **Mermaid built in** — diagrams render in preview and can be copied or exported directly from the panel
- **Better export output** — HTML and PDF keep the same look, with Mermaid diagrams included in the final file
- **Table of contents sidebar** — jump through large docs without losing your place
- **Presentation mode** — turn heading sections into slides for demos or walkthroughs

PDF and image export use Chrome or Chromium automatically. If VS Code cannot find it, set `devThemePro.chromePath` in Settings.

## Table Preview

Open delimited files in a proper inspection view instead of scanning raw rows.

Supported files: `.csv`, `.tsv`, `.psv`, `.dsv`, `.ssv`, `.tab`

| Action               | How                                                                                                            |
| -------------------- | -------------------------------------------------------------------------------------------------------------- |
| Preview to the side  | Click the table preview button in the editor title bar, or press `Cmd+K V` / `Ctrl+K V`                        |
| Preview in place     | Use `Cmd+K Cmd+V` / `Ctrl+K Ctrl+V` on a supported data file                                                   |
| Open With picker     | Right-click the file in the Explorer and choose **Open With… → 🔮 Dev Theme Pro Table Preview**                |
| Right-click shortcut | Right-click the file in the Explorer or the editor tab and choose **🔮 Open With Dev Theme Pro Table Preview** |

What you get:

- **Sorting** — click any column header to sort ascending or descending
- **Filtering** — search large datasets instantly
- **Column resize** — fit the view around the data you care about
- **Row numbers** — keep references stable while reviewing larger files
- **Built-in column text coloring** — structured text is easier to scan directly in the editor
- **Export options** — save the table as PDF, PNG, or standalone HTML

## Code Snapshot

Create a clean, shareable image from your code without leaving VS Code.

1. Open any code file.
2. Select the lines you want to capture.
3. Press `Cmd+Shift+S` / `Ctrl+Shift+S`, or use **🔮 Dev Theme Pro → 📸 Code Snapshot** from the editor context menu.
4. Review the live preview in the side panel.
5. Copy or save the final PNG.

If nothing is selected, the snapshot panel opens with a clear prompt instead of grabbing the whole file automatically.

## Commands

| Command                          | Mac           | Windows / Linux |
| -------------------------------- | ------------- | --------------- |
| Open Markdown Preview (side)     | `Cmd+K V`     | `Ctrl+K V`      |
| Open Markdown Preview (in-place) | `Cmd+K Cmd+V` | `Ctrl+K Ctrl+V` |
| Open Table Preview (side)        | `Cmd+K V`     | `Ctrl+K V`      |
| Open Table Preview (in-place)    | `Cmd+K Cmd+V` | `Ctrl+K Ctrl+V` |
| Code Snapshot                    | `Cmd+Shift+S` | `Ctrl+Shift+S`  |

All commands are also available in the **Command Palette**. Search for **Dev Theme Pro**.

## Tools Menu

All preview and export actions are grouped under one **🔮 Dev Theme Pro** submenu in the editor context menu.

- **Markdown files** — open preview, export PDF, export HTML
- **Delimited files** — open table preview, export PNG, export HTML
- **Code files** — open the snapshot workflow

Matching **Open With…** entries are also available from the Explorer and editor tabs.

## Settings

| Setting                  | Type     | Default | Description                                                                          |
| ------------------------ | -------- | ------- | ------------------------------------------------------------------------------------ |
| `devThemePro.chromePath` | `string` | `""`    | Path to Chrome or Chromium for PDF and image export. Leave empty for auto-detection. |

## Screenshot

![Dev Theme Pro — Editor](images/code.jpg)

## Changelog

See [CHANGELOG.md](CHANGELOG.md) for release notes.

## Issues & Suggestions

Found something off or want another feature?
→ [Open an issue on GitHub](https://github.com/FaizanAshiq/dev-theme-pro/issues)

## Author

**Faizan Ashiq** — [LinkedIn](https://www.linkedin.com/in/faizanashiq/) · [GitHub](https://github.com/FaizanAshiq)

## License

MIT © 2025–2026 Faizan Ashiq — [Full License](LICENSE.txt)

---

**If Dev Theme Pro is part of your daily setup, a review on the [VS Code Marketplace](https://marketplace.visualstudio.com/items?itemName=FaizanAshiq.dev-theme-pro) helps a lot.**
