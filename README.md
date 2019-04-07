<p align="center">
  <a href="https://horizontheme.com/">
    <img alt="horizon banner" src="https://i.imgur.com/bbznMuY.png">
  </a>
</p>

---

This is a fork of [Horizon Theme](https://marketplace.visualstudio.com/items?itemName=jolaleye.horizon-theme-vscode) that combines its UI colors with Dark+ (the default theme) token colors.

---

<p align="center">
  <!-- marketplace version -->
  <a href="https://marketplace.visualstudio.com/items?itemName=jolaleye.horizon-theme-vscode">
    <img alt="marketplace version" src="https://img.shields.io/vscode-marketplace/v/piousdeer.horizon-theme-vscode-default-token-colors.svg?maxAge=3600&style=for-the-badge&colorA=1C1E26&colorB=FAB38E">
  </a>
  <!-- downloads -->
  <a href="https://marketplace.visualstudio.com/items?itemName=piousdeer.horizon-theme-vscode-default-token-colors">
    <img alt="downloads" src="https://img.shields.io/visual-studio-marketplace/d/piousdeer.horizon-theme-vscode-default-token-colors.svg?maxAge=3600&style=for-the-badge&colorA=1C1E26&colorB=FAB38E">
  </a>
  <!-- rating -->
  <a href="https://marketplace.visualstudio.com/items?itemName=piousdeer.horizon-theme-vscode-default-token-colors">
    <img alt="rating" src="https://img.shields.io/visual-studio-marketplace/stars/piousdeer.horizon-theme-vscode-default-token-colors.svg?maxAge=86400&style=for-the-badge&colorA=1C1E26&colorB=FAB38E">
  </a>
</p>

<p align="center">
  <img alt="preview" src="https://i.imgur.com/8IqkjhH.png" width="90%">
</p>

> The preview above shows the _Horizon Default_ theme with the _Dank Mono_ font.

## Installation

1. Open the **Extensions** sidebar in VS Code
2. Search for `Horizon Theme Default`
3. Click **Install**
4. Open the **Command Palette** with `Ctrl+Shift+P` or `⇧⌘P`
5. Select **Preferences: Color Theme** and choose `Horizon Default`.
6. Enjoy! 🎉 Also, check out some of the personalization options below...

> Visit the [Horizon Homepage](https://horizontheme.com/) for some nice previews :)

## Personalization

Tastes change all the time. Fortunately, VS Code makes it easy to customize just about every aspect of your editor.
If you want to change something, open the **Command Palette** and select **Preferences: Open Settings (JSON)**. Here, you can override VS Code's defaults or Horizon's colors.
Check out some of the personalization options below to customize Horizon to suit your taste.

_For more info on theming, visit the [Theme Authoring Guide](https://code.visualstudio.com/api/extension-capabilities/theming) and [Theme Color Reference](https://code.visualstudio.com/api/references/theme-color)._

### Sidebar Contrast

```
"workbench.colorCustomizations": {
  "activityBar.background": "#1E2028",
  "activityBar.border": "#1E2028",
  "sideBar.background": "#1E2028",
  "sideBar.border": "#1C1E26"
}
```

### Italics

The normal theme only uses italics in a few places: comments, parameters, and some special keywords (e.g. `this`). If you would prefer no italics at all, you can configure this in your settings...

```
"editor.tokenColorCustomizations": {
  "textMateRules": [
    {
      "name": "No italics",
      "scope": ["comment", "variable.language", "variable.parameter"],
      "settings": {
        "fontStyle": ""
      }
    }
  ]
}
```

### Tag Brackets `<>`

For gray rather than red brackets around HTML tags...

```
"editor.tokenColorCustomizations": {
  "textMateRules": [
    {
      "name": "HTML tag brackets",
      "scope": ["punctuation.definition.tag"],
      "settings": {
        "foreground": "#BBBBBB"
      }
    }
  ]
}
```

## Contributing

### [Code of Conduct](CODE_OF_CONDUCT.md)

Always try your best to make a positive impact on this project and its community. By participating, you are expected to uphold the Code of Conduct.

### [Contributing Guide](CONTRIBUTING.md)

Read the contributing guide to learn about how you can report issues and contribute to changes.

## Color Reference

### UI Colors

|                            Color                            | Usage                                              |
| :---------------------------------------------------------: | -------------------------------------------------- |
| ![](https://via.placeholder.com/10/1C1E26?text=+) `#1C1E26` | Primary background                                 |
| ![](https://via.placeholder.com/10/232530?text=+) `#232530` | Light background (popups & widgets)                |
| ![](https://via.placeholder.com/10/2E303E?text=+) `#2E303E` | Selection, highlights, input field background      |
| ![](https://via.placeholder.com/10/6C6F93?text=+) `#6C6F93` | Accents (e.g. scrollbar, drag and drop highlights) |
| ![](https://via.placeholder.com/10/F43E5C?text=+) `#F43E5C` | Errors, deletion highlights                        |
| ![](https://via.placeholder.com/10/E95378?text=+) `#E95378` | Accents (e.g. active tab, badges)                  |
| ![](https://via.placeholder.com/10/FAB38E?text=+) `#FAB38E` | Debugging status bar                               |
| ![](https://via.placeholder.com/10/FAC39A?text=+) `#FAC39A` | Modified Git decoration (explorer)                 |
| ![](https://via.placeholder.com/10/21BFC2?text=+) `#21BFC2` | Modified highlights (gutter & scrollbar ruler)     |
| ![](https://via.placeholder.com/10/27D797?text=+) `#27D797` | Warning highlights, untracked resources            |
| ![](https://via.placeholder.com/10/09F7A0?text=+) `#09F7A0` | Addition highlights                                |

## License

[MIT](LICENSE) © [Jonathan Olaleye](https://github.com/jolaleye)
