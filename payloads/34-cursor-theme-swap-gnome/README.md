# cursor theme swap (gnome)

swaps the mouse cursor theme for 8s, then restores the exact one you had.

## needs

- gnome (`gsettings` on `org.gnome.desktop.interface`).
- a terminal on `ctrl+alt+t`.

## making the swap visible

it swaps to `Adwaita`. if that's already your theme you won't see anything. change that
one word to another installed theme, e.g. `Bibata-Modern-Ice` or `DMZ-White`. list
what's installed:

```sh
ls /usr/share/icons ~/.icons ~/.local/share/icons 2>/dev/null
```

(a folder counts if it has a `cursors/` dir.)

## revert

nothing to do, the original is saved and written back after 8s.
