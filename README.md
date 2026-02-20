# Alabaster for Helix

Port of [Alabaster](https://github.com/tonsky/vscode-theme-alabaster) color scheme by Nikita Prokopov (Tonsky) to [Helix](https://helix-editor.com/).
Ported with GitHub Copilot.

Includes both **light** (`alabaster`) and **dark** (`alabaster-dark`) variants.
Both themes are standalone files with no inheritance dependency.

## Installation

Copy (or symlink) theme files into your Helix themes directory:

```sh
mkdir -p ~/.config/helix/themes
cp alabaster.toml alabaster-dark.toml ~/.config/helix/themes/
```

Then set your theme in `~/.config/helix/config.toml`:

```toml
theme = "alabaster"       # light
# theme = "alabaster-dark"  # dark
```

## Credits

- Original theme: [Alabaster](https://github.com/tonsky/sublime-scheme-alabaster) by Nikita Prokopov
- Also see: [VS Code version](https://github.com/tonsky/vscode-theme-alabaster)
