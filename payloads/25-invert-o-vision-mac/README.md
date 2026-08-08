# invert-o-vision (mac)

inverts the whole display for ~4s, then flips it back with the same shortcut.

## the shortcut might be off

it uses control+option+command+8 (the "invert colors" accessibility shortcut). on some
macos versions that's disabled by default. if nothing happens, turn it on:

system settings > keyboard > keyboard shortcuts > accessibility > "invert colors"

then run it again. if it stays off, the payload just does nothing.

## revert

automatic, it toggles back after ~4s. stuck inverted? press control+option+command+8
yourself.
