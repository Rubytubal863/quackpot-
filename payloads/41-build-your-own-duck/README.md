# build your own duck

types a note explaining the target just got pranked by a ducky, then three steps to
build their own.

## setup

- branches on `$_OS` (os_detect extension, bundled with payload studio). compile there.
  the `DELAY 1500` up top lets `$_OS` populate before the branch.
- edit the repo url at the bottom of `note_body()` to wherever you host these.

## revert

close the editor without saving. the linux branch only prints.
