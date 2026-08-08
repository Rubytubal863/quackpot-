# button encore

opens notepad and waits. every press of the ducky's own button types a random duck
joke.

## how it works

- `BUTTON_DEF ... END_BUTTON` is the press handler; it runs on every press, rolls a new
  number, and picks one of three jokes.
- `$pick` is declared once up top; the handler only reassigns it, so nothing gets
  re-declared inside the repeatedly-fired block.
- the `WHILE (TRUE)` at the end keeps the payload alive so it stays armed. without it
  the payload would end and the button would do nothing.

keep a text field (notepad) focused so the jokes land somewhere.

## revert / stop

unplug the ducky. it stays armed between presses, so unplugging is how you stop it.
close notepad without saving.
