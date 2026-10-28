# Oldbook themes

This repository is the portable archive of the Space Ghost / Oldbook desktop
themes and their artwork.  It was split from
[`Spaceghost/.files`](https://github.com/Spaceghost/.files) so theme history and
large image assets can evolve independently from machine configuration.

Every theme is a complete desktop design, not a color preset.  A descriptor
must provide a semantic palette; rendered profiles may add typography,
geometry, effects, cursors, icons and application-specific overrides.  Missing
application overrides inherit the shared renderer.  The semantic palette stays
the source of truth.

## Layout

- `themes/` contains descriptors, complete generated profiles, the active-theme
  marker and design documentation.
- `gallery/` contains theme-associated paintings and their sidecar metadata.
- `archive/` contains retained historical theme descriptors.
- `metadata/` contains gallery indexes, prompt catalogs and artwork provenance.
- `SHA256SUMS` records every published file other than itself and Git metadata.

The live theme engine currently writes to `~/.files/alpine/themes`; this
repository is a publication/archive boundary, not yet the live mutable state
directory.  Keep the dotfiles copy until the engine accepts a separate theme
root.  Personal journals, Scripture history, credentials, radio policy, camera
or audio captures are intentionally outside this repository.

## Coverage contract

Themes cover Sway/SwayFX, Waybar, SwayNC, swaynag, wlogout, GTK 3/4, Qt 6,
Ghostty, Foot, btop, Cava, Conky, Fuzzel, Neovim, fastfetch, satty, Starship,
Claude Code, Firefox, STRATA, cursor/icon assets, the lock screen and boot
palette.  Hover, focus, selected, disabled, urgent and failure states are part
of that coverage.  The original Ghost badge colors are an explicit branding
exception.

Artwork provenance remains beside the images.  Do not add generated media
without its metadata, and do not add personal or unfiltered capture media.
