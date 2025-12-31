# Dev Theme Pro 🌌

A sleek, developer-friendly VS Code theme for modern coding with beautiful syntax highlighting and smooth color
transitions.

![Version](https://img.shields.io/visual-studio-marketplace/v/FaizanAshiq.dev-theme-pro?style=for-the-badge&colorA=1e1e2e&colorB=A46FED&label=VERSION)
![Downloads](https://img.shields.io/visual-studio-marketplace/d/FaizanAshiq.dev-theme-pro?style=for-the-badge&colorA=1e1e2e&colorB=cc866a&label=DOWNLOADS)
![Rating](https://img.shields.io/visual-studio-marketplace/r/FaizanAshiq.dev-theme-pro?style=for-the-badge&colorA=1e1e2e&colorB=56C98E&label=RATING)
![License](https://img.shields.io/badge/license-MIT-green?style=for-the-badge)

<p align="center">
  <img src="images/icon.png" alt="Dev Theme Pro" width="120">
</p>

## Screenshots

**TypeScript Preview** ![TypeScript](images/typescript.jpg)

**React Preview** ![React](images/react.jpg)

**JavaScript Preview** ![JavaScript](images/javascript.jpg)

**HTML & CSS Preview** ![HTML & CSS](images/html-css.jpg)

**Python Preview** ![Python](images/python.jpg)

## Installation

### Marketplace

1. Open VS Code → Extensions (`Ctrl+Shift+X` / `Cmd+Shift+X`)
2. Search `Dev Theme Pro`
3. Click Install
4. Go to `File → Preferences → Color Theme` and select **Dev Theme Pro Smooth**

### Manual

1. Download or clone this repo
2. Copy the theme to your VS Code extensions folder
3. Reload VS Code and select the theme

⭐ **Rate five-stars if you enjoy it!**

## Customize Colors

You can override colors in `settings.json`:

```json
"workbench.colorCustomizations": {
  "[Dev Theme Pro Smooth]": {
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
  "[Dev Theme Pro Smooth]": {
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

**Faizan Ashiq** — [LinkedIn](https://www.linkedin.com/in/faizan-ashiq/) · [GitHub](https://github.com/FaizanAshiq)

## License

MIT © Faizan Ashiq - [Full License](LICENSE.txt)

---

**Enjoying Dev Theme Pro?** ⭐ Star the repo and share feedback!

If you like this theme, please leave a review on the
[VS Code Marketplace](https://marketplace.visualstudio.com/items?itemName=FaizanAshiq.dev-theme-pro).
