# the duck of theseus

types a short philosophical bit, credits the prank, and says how to disarm it.

## needs

- the os_detect extension (`$_OS`), bundled with payload studio, so compile there.
- the top `DELAY 1500` covers hid enumeration and gives `$_OS` time to populate. don't
  shorten it.

## per os

- windows: notepad via run.
- macos: textedit via spotlight, new doc (cmd+n).
- linux (x11): a terminal, printed via a single-quoted `cat` heredoc.

## revert

windows/macos: close the editor without saving. linux: it only printed, nothing to
undo.
