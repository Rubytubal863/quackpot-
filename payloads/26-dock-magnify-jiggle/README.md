# dock magnify jiggle

cranks dock magnification huge for ~6s, then puts your settings back.

## how the revert works

the one-liner reads your current `magnification` and `largesize` first, changes them,
waits, then writes the saved values back (or removes the keys if they were unset) and
relaunches the dock. `killall Dock` just restarts the dock process, nothing
destructive.

if you interrupt it mid-run and the dock is still huge, reset to defaults:

```sh
defaults delete com.apple.dock magnification
defaults delete com.apple.dock largesize
killall Dock
```

or toggle magnification back in system settings > desktop & dock.
