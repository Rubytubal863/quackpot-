# xrandr barrel roll

flips the x11 display 180 for 5s, then rights it.

## needs

- x11. uses `xrandr`. under wayland it's a no-op or a harmless error.
- a terminal on `ctrl+alt+t` (gnome default, common elsewhere). if nothing opens, swap
  that step for your desktop's open-terminal shortcut.

## revert

nothing to do, `xrandr -o normal` runs after the 5s. by hand: `xrandr -o normal`.
