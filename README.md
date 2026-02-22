# Dev Theme Pro 🌌

A beautiful dark theme with colorful syntax highlighting, designed for developers who love aesthetics and readability. **12 variants** — pick your accent color and background depth.

<p align="center">
  <img src="images/icon.png" alt="Dev Theme Pro" width="120">
</p>

![Dev Theme Pro — 4 Accent Variants](images/window/themes.png)

## Theme Variants

**4 Accents** × **3 Backgrounds** = **12 themes**

| Accent     | Dusk 🌅 (lightest) | Night 🌙 (default) | Void 🕳️ (darkest) |
| ---------- | ------------------ | ------------------ | ----------------- |
| ✨ Amber   | Amber Dusk         | Amber Night        | Amber Void        |
| 💎 Emerald | Emerald Dusk       | Emerald Night      | Emerald Void      |
| 🌌 Nebula  | Nebula Dusk        | Nebula Night       | Nebula Void       |
| 🌊 Ocean   | Ocean Dusk         | Ocean Night        | Ocean Void        |

## Screenshots

### Editor Preview

![Dev Theme Pro — Editor](images/window/code.jpg)

### Syntax Highlighting

**TypeScript** ![TypeScript](images/typescript.jpg)

**React** ![React](images/react.jpg)

**JavaScript** ![JavaScript](images/javascript.jpg)

**HTML & CSS** ![HTML & CSS](images/html-css.jpg)

**Python** ![Python](images/python.jpg)

## Installation

### Marketplace

1. Open VS Code → Extensions (`Ctrl+Shift+X` / `Cmd+Shift+X`)
2. Search `Dev Theme Pro`
3. Click Install
4. Go to `File → Preferences → Color Theme` and pick any **Dev Theme Pro** variant

### Manual

1. Download or clone this repo
2. Copy the folder to your VS Code extensions directory
3. Reload VS Code and select the theme

⭐ **Rate five-stars if you enjoy it!**

## Customize Colors

You can override colors in `settings.json` (replace the variant name as needed):

```json
"workbench.colorCustomizations": {
  "[Dev Theme Pro — 🌊 Ocean 🌙 Night]": {
    "editor.background": "#1a1a2e",
    "sideBar.background": "#1a1a2e"
  }
}
```

### Recommended Settings

```json
"editor.fontFamily": "Lotion, Fira Code, JetBrains Mono",
"editor.fontLigatures": true,
"editor.fontSize": 14,
"editor.lineHeight": 30
```

### Enable Italics

```json
"editor.tokenColorCustomizations": {
  "[Dev Theme Pro — 🌊 Ocean 🌙 Night]": {
    "textMateRules": [
      {
        "scope": ["comment", "keyword", "storage.modifier"],
        "settings": { "fontStyle": "italic" }
      }
    ]
  }
}
```

---

## Changelog

See [CHANGELOG.md](CHANGELOG.md) for release notes.

## Issues & Suggestions

Found a bug or have a feature request?  
👉 [Open an issue on GitHub](https://github.com/FaizanAshiq/dev-theme-pro/issues)

## Author

**Faizan Ashiq** — [LinkedIn](https://www.linkedin.com/in/faizanashiq/) · [GitHub](https://github.com/FaizanAshiq)

## License

MIT © 2025-2026 Faizan Ashiq - [Full License](LICENSE.txt)

---

**Enjoying Dev Theme Pro?** ⭐ Star the repo and share feedback!

If you like this theme, please leave a review on the
[VS Code Marketplace](https://marketplace.visualstudio.com/items?itemName=FaizanAshiq.dev-theme-pro).
