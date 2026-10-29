# Screenshots and pictures

What `README.md` shows, and how each picture was made, so none of them is a mystery later.

## On the README

| File | Size | What | How |
|------|------|------|-----|
| `banner.webp` | 1600×480 | the header | rendered from `banner.html` with headless Chromium (`--window-size=1600,480`), which loads the fonts from `crates/horizon-theme/fonts/`; edit the HTML, re-render, re-encode |
| `launcher-play.webp` | 1280×800 | the launcher's Home page | the launcher from `HORIZON_LAUNCHER_HOME` scratch folders, offline name `Steve`; no account or server data in frame |
| `launcher-settings.webp` | 1280×800 | the launcher's Settings page | same run as `launcher-play.webp` |
| `sunset.webp` | 1600×900 | the hero, a savanna village at sunset | the Rust client, vanilla assets, no mods or shaders |
| `survival.webp` | 1600×900 | dusk, a zombie, the HUD | the Rust client, survival |
| `village.webp` | 1600×900 | a plains village and an iron golem | the Rust client, creative |
| `nether.webp` | 1600×900 | a crimson forest | the Rust client, the Nether |
| `underwater.webp` | 1600×900 | a warm ocean reef | the Rust client |
| `distant-terrain.webp` | 1600×900 | LOD Distance on, far past the render distance | the Rust client, seed 1234, spectator at y 165 over the village at (-960, 170), `/time 6000`, HUD hidden (F1), LOD Distance 512 (capped to 128 chunks on the integrated GPU) |

The `.jpg` files beside them are the masters of the same frames, kept so a re-encode does not go
through the game again (`night.jpg` is unused, kept as a spare). Game frames are captured at
1600×900, five times 320×180, so a downscale stays on whole pixels; the launcher is vector and
text, so any 16:10 size is fine.

Captures follow the rule in [AGENTS.md](../../AGENTS.md): fresh `mktemp -d` folders for
`HORIZON_HOME`, `HORIZON_LAUNCHER_HOME`, `XDG_DATA_HOME` and `XDG_CONFIG_HOME`, `HORIZON_NO_AUDIO=1`,
`HORIZON_NO_SELF_UPDATE=1` for the launcher, and nothing written under `~/.local/share`.

## Elsewhere

- `settings-simple.png`, `settings-advanced.png`: the graphics pages, used by [docs/graphics.md](../graphics.md).
- `accessibility-settings.png`, `multiplayer-*.png`, `hand-fov-*.png`, `issue563-*.png`,
  `command-suggestions/`: issue and documentation pictures.
- `brand/`, `icon-256.png`, `logo.*`, `social-preview.jpg`: the mark and its exports, described in
  [brand/README.md](brand/README.md).
