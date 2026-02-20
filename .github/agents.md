# Copilot Agent Guidelines for helix-alabaster

## Alabaster Philosophy

This repo follows Tonsky's Alabaster color scheme philosophy:
- **Only four syntax classes are highlighted**: strings, constants, comments, and global definitions
- Keywords and types are intentionally left as plain foreground — they are obvious and add noise
- `type.builtin` and `variable.builtin` get the constants color (purple) because builtins are "statistically known constants"
- Comments are highlighted (not dimmed) — if someone wrote a comment, it matters

## Theme Structure

- Both themes are **standalone** (no `inherits`) to allow independent palette optimization and consolidation
- Palette keys use **color names** (e.g. `red`, `purple`, `blue`), not scope names (avoid `comment`, `string`, `punctuation` as palette keys)
- Palette must stay **alphabetically sorted** with no duplicate hex values within a theme

## Diagnostic Styling

- `diagnostic.error` and `diagnostic.warning`: **underline-only** (no fg/bg override) — preserve original syntax highlighting colors
- Underline color is explicit (`color = "red"` / `color = "orange"`)
- `diagnostic.hint`: uses fg override (gray) — this is intentional, hints are less important
- Message-level `error`/`warning` styles keep their fg colors for gutter/popup display

## Color Preferences

- Dark theme red should be **desaturated** (soft coral, not pure red)
- Dark theme comment color is a **warm brownish yellow**, not pure yellow
- Light theme warning/orange should be clearly visible (not washed out)
