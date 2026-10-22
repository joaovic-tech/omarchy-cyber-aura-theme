# Cyber Aura

A neon cyberpunk theme for [Omarchy](https://omarchy.org), tuned for reading text in the terminal.

> Requires **Omarchy 4** or newer.

## Quick Install

```bash
omarchy theme install https://github.com/joaovic-tech/omarchy-cyber-aura-theme
```

Or use *Install › Style › Theme* in the Omarchy menu and paste the URL.

## Previews

![Cyber Purple](./previews/0-preview.png)
![Ninja Oni Mask](./previews/1-preview.png)
![Cyber Assassin Girl](./previews/preview.png)
![Neon Rain City](./previews/3-preview.png)

## Colors

Every ANSI color has its own hue and reaches at least 4.5:1 contrast against the background.

| Role | Color | Hex |
|------|-------|-----|
| Background | ![#09090e](https://placehold.co/16/09090e/09090e) | `#09090e` |
| Surface | ![#151521](https://placehold.co/16/151521/151521) | `#151521` |
| Selection | ![#3d1035](https://placehold.co/16/3d1035/3d1035) | `#3d1035` |
| Muted (comments) | ![#7a7a9e](https://placehold.co/16/7a7a9e/7a7a9e) | `#7a7a9e` |
| Foreground | ![#e0e6f0](https://placehold.co/16/e0e6f0/e0e6f0) | `#e0e6f0` |
| Accent | ![#ff007f](https://placehold.co/16/ff007f/ff007f) | `#ff007f` |
| Red | ![#ff2a6d](https://placehold.co/16/ff2a6d/ff2a6d) | `#ff2a6d` |
| Orange | ![#ff9e3d](https://placehold.co/16/ff9e3d/ff9e3d) | `#ff9e3d` |
| Yellow | ![#ffe700](https://placehold.co/16/ffe700/ffe700) | `#ffe700` |
| Green | ![#00ff9f](https://placehold.co/16/00ff9f/00ff9f) | `#00ff9f` |
| Cyan | ![#00f0ff](https://placehold.co/16/00f0ff/00f0ff) | `#00f0ff` |
| Blue | ![#4d94ff](https://placehold.co/16/4d94ff/4d94ff) | `#4d94ff` |
| Purple | ![#c561ff](https://placehold.co/16/c561ff/c561ff) | `#c561ff` |

The active window border is a pink → cyan gradient.

## Transparent terminal with blur

Omarchy ignores terminal configs shipped by themes installed from git, so transparency lives in your own config. Blur is off by default in Omarchy 4.

`~/.config/hypr/looknfeel.lua`:

```lua
hl.config({
  decoration = {
    blur = { enabled = true, size = 8, passes = 3, new_optimizations = true, xray = false, vibrancy = 0.2 },
  },
})
```

`~/.config/foot/foot.ini` (only the background becomes transparent, text stays fully opaque):

```ini
[colors-dark]
alpha=0.85
```

## Notes

- When installed from git, Omarchy drops `neovim.lua` and generates the Neovim colors from `colors.toml` instead. To use the hand-tuned Neovim highlights, clone the repo somewhere else and symlink it into `~/.config/omarchy/themes/cyber-aura`.

---

This theme is under the **MIT** license. If you like it, please leave a ⭐ on the repository!
