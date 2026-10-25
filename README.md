# Ghostty Cyberpunk Theme

Ghostty colors matched to [herdr-cyberpunk-theme](https://github.com/liveinknewgithub/herdr-cyberpunk-theme): a violet-black background, neon ANSI palette, slight translucency with blur, and a neon cyan bar cursor.

## What's in `config`

| Setting | Value |
| --- | --- |
| Background / foreground | `#0d0221` / `#e8fdff` |
| ANSI 0–7 | `#1b0b3b` `#ff003c` `#39ff88` `#fcee0a` `#2e9bff` `#ff2bd6` `#00f0ff` `#b9c8f5` |
| ANSI 8–15 | `#7a5fc0` `#ff5980` `#7effb2` `#fdf460` `#77beff` `#ff75e4` `#00ffc6` `#ffffff` |
| Cursor | `#00f0ff` bar |
| Selection | `#4b0f6b` |
| Window | `background-opacity = 0.92`, `background-blur = 20`, `background-opacity-cells = true` |

`background-opacity-cells = true` applies the translucency to cells with explicit backgrounds too, such as Herdr's sidebar and tab bar.

## Install (macOS)

```sh
git clone https://github.com/liveinknewgithub/ghostty-cyberpunk-theme.git
cfg="$HOME/Library/Application Support/com.mitchellh.ghostty/config"
cp "$cfg" "$cfg.bak"   # keep your current config
cp ghostty-cyberpunk-theme/config "$cfg"
```

Reload with Cmd+Shift+, to apply colors and the cursor. On macOS, `background-opacity` only changes after quitting and reopening Ghostty.

`config` is a complete Ghostty config. To keep your other settings, copy only its color, translucency, and cursor lines into your own config.
