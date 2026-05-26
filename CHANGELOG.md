# Changelog

## 2026.05.26

### What Changed
- Replaced picom with **fastcompmgr** as the compositor. Boot launch and the toggle now use fastcompmgr, and the compositor-toggle keybind moved to the unified `super + g` (was `super + alt + o`).

### Technical Details
- `rc.lua`: autostart `picom -b --config $HOME/.config/awesome/picom.conf` → `fastcompmgr -c`; toggle key changed from `{ modkey1, altkey }, "o"` to `{ modkey }, "g"`.
- `scripts/picom-toggle.sh` renamed to `fastcompmgr-toggle.sh` (simple on/off toggle — fastcompmgr takes no config file).
- Deleted the now-unused `picom.conf`.

### Files Modified
- etc/skel/.config/awesome/rc.lua
- etc/skel/.config/awesome/scripts/fastcompmgr-toggle.sh (created, replaces picom-toggle.sh)
- etc/skel/.config/awesome/scripts/picom-toggle.sh (deleted)
- etc/skel/.config/awesome/picom.conf (deleted)

## 2026.05.21

### What Changed
- Initial markdown scaffold added per the ecosystem MD-scaffold rule ([HQ/CLAUDE.md](/home/erik/Insync/Kiro/Kiro-HQ/CLAUDE.md#required-markdown-scaffold-every-repo)).
- Stubs created for `CHANGELOG.md`, `CLAUDE.md`, `IDEAS.md`, `TODO.md` (whichever were missing).
- README rewritten with real install/usage content (replaced earlier one-line stub) where applicable.

### Files Modified
- CHANGELOG.md (created)
- CLAUDE.md (created where missing)
- IDEAS.md (created where missing)
- TODO.md (created where missing)
- README.md (rewritten where it was a stub)
