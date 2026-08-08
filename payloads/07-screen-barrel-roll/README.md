# screen barrel roll

flips the display 180 for ~4s, then rights it.

## needs intel graphics hotkeys

the rotation uses intel's gpu hotkeys:

- `ctrl+alt+down` rotates 180
- `ctrl+alt+up` rotates back to 0

these come from the intel graphics driver / graphics command center, and only fire on
an intel igpu with hotkeys enabled (graphics command center > system > hot keys). on
amd/nvidia-only machines the chords do nothing, so it's a no-op there.

## revert

automatic, it sends `ctrl+alt+up` after the delay. stuck upside down? press that
yourself, or settings > system > display > display orientation > landscape.

## other platforms

macos: payload 25. linux (x11): payload 31.
