# Current-main evidence for the Hyprland inactive-workspace report

- Build: `73f5486b90b573f5a7b1a0320ecfb21cbb25d5b2` (`main` at test time).
- `7e5b3861e` (merged PR #6779) is an ancestor of that build.
- Test state: ordinary Horizon title screen, Wayland/Hyprland.
- `01`: Horizon title screen and btop on one active workspace.
- `02`: Horizon moved to inactive workspace 10; btop remains on active workspace 9.
- `03`: immediately after returning to Horizon's workspace.

The btop process percentage is normalized to the host's total eight logical CPUs. Its process CPU values should therefore be read as fractions of total system capacity, not as a per-core percentage.
