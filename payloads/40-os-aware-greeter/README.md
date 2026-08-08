# os-aware greeter

one payload, three greetings. reads `$_OS` and greets whichever host it lands on.

## needs

the os_detect extension, which ships with payload studio, so compile there and `$_OS`
resolves. the `DELAY 1500` up top gives the host time to configure the hid before the
branch runs, don't shorten it.

## per os

- windows: opens notepad (run > `notepad`), types a greeting.
- macos: opens textedit via spotlight, new doc (cmd+n), types a greeting.
- linux (x11): opens a terminal (ctrl+alt+t) and echoes a greeting.

## revert

close notepad/textedit without saving. the linux branch only prints.
