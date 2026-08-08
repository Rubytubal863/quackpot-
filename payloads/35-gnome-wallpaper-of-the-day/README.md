# wallpaper of the day (gnome)

paints the desktop solid hot-pink for 6s, then restores your real wallpaper.

## needs

- gnome (`gsettings` on `org.gnome.desktop.background`).
- a terminal on `ctrl+alt+t`.

## revert

nothing to do. it saves `picture-uri`, `picture-options` and `primary-color` first and
writes all three back after 6s. want a different colour? change `#ff69b4`.
