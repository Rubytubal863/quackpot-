# quackpot

50 harmless usb rubber ducky payloads in duckyscript 3.0. pranks, not malware.

flip the wallpaper and flip it back. make a mac beatbox. blink QUACK in morse on the
caps lock led. a growing pyramid of the word quack. a certificate declaring you a
certified duck handler. every one reverts in about five seconds, and none of them touch
your files, your settings, or anything security-related.

built for the 2022 usb rubber ducky / duckyscript 3.0, compiles in payload studio
(payloadstudio.hak5.org). most degrade fine on the classic ducky too.

## rules

run these on your own machine, or on someone who's said "yeah, prank me." that's the
whole deal. a rubber ducky is a keyboard that types on its own; running one on a
computer without the owner's ok isn't a prank, it's keystroke injection, and plenty of
places treat that as a crime. keep it consensual, revert it, move on.

## what's not in here

no exfil, no keylogging, no keystroke reflection, no loot.bin. no download-and-run, no
droppers. no persistence: nothing in startup, services, scheduled tasks, or the
registry. nothing touching defender, the firewall, uac, or any security setting.
nothing destructive: no mass delete, no rm -rf, no format, no shutdown or bsod spam, no
fork bombs, no ransomware bits. if it can't be undone in five seconds it doesn't belong
here.

## arming one

1. open payload studio (payloadstudio.hak5.org).
2. pick a payload below, open its `payloads/NN-slug/payload.txt`.
3. paste it into a new payload.
4. set the keyboard language to match the target (default is us).
5. download `inject.bin`.
6. drop `inject.bin` at the root of the ducky's microsd, replacing the old one.
7. plug it into a machine you're allowed to prank.

some payloads have their own readme with setup notes (the intel-gpu caveat, gnome bits,
which extension to enable). those are the linked names in the table.

## the 50

23 windows, 11 macos, 10 linux (x11), 6 cross-platform. each payload's `REM Novelty:` line says why it isn't a rehash of anything in
hak5/usbrubberducky-payloads (no rickrolls, no stock hello-world, no re-skins of the
community prank folder).

| # | payload | os | gag |
|---|---------|----|-----|
| 01 | [magnifier disco](payloads/01-magnifier-disco/) | windows | strobes the windows magnifier in and out on a beat, then closes it. |
| 02 | [clippy's comeback](payloads/02-clippy-comeback/) | windows | opens notepad, clippy comes back to help, rambles, then admits it's a ducky. |
| 03 | [sapi sea shanty](payloads/03-sapi-sea-shanty/) | windows | sings a short duck sea shanty out loud through the built-in sapi voice. |
| 04 | [beep symphony](payloads/04-beep-symphony/) | windows | plays a six-note phrase on the system beep. no volume change, no files. |
| 05 | [emoji picker parade](payloads/05-emoji-picker-parade/) | windows | opens notepad and walks a row of animal emoji in through the win+. picker. |
| 06 | [virtual desktop carousel](payloads/06-virtual-desktop-carousel/) | windows | makes three virtual desktops, surfs across them, then closes the ones it made. |
| 07 | [screen barrel roll](payloads/07-screen-barrel-roll/) | windows | flips the screen 180 for a few seconds, then rights it. |
| 08 | [invert-o-vision](payloads/08-invert-o-vision/) | windows | inverts the screen colours through magnifier for a few seconds, then restores. |
| 09 | [typewriter duck ode](payloads/09-typewriter-duck-ode/) | windows | types a short ode to the rubber duck with an old-typewriter cadence. |
| 10 | [clipboard quackpot](payloads/10-clipboard-quackpot/) | windows | replaces the clipboard so the next paste is a quack instead. |
| 11 | [fake loading bar](payloads/11-fake-loading-bar/) | windows | types an ascii progress bar up to 100%, then admits it was nothing. |
| 12 | [rubber duck debugger](payloads/12-rubber-duck-debugger/) | windows | the duck debugs your code by asking the usual rubber-duck questions, then shouts the punchline. |
| 13 | [certified duck handler](payloads/13-duck-handler-certificate/) | windows | prints an ascii certificate naming you a certified duck handler. |
| 14 | [wholesome web detour](payloads/14-wholesome-web-detour/) | windows | opens the browser to pointerpointer, a pointless-but-harmless site. |
| 15 | [five tabs, one cat](payloads/15-same-cat-five-tabs/) | windows | opens the same bouncing-cat page in five tabs via a loop. |
| 16 | [goofy search drive-by](payloads/16-goofy-search-drive-by/) | windows | opens the browser straight to an absurd search. |
| 17 | [on-screen keyboard cameo](payloads/17-osk-cameo/) | windows | pops the on-screen keyboard onto the desktop for no reason. |
| 18 | [konami notepad](payloads/18-konami-notepad/) | windows | types the konami code into notepad and grants 30 lives. |
| 19 | [binary whisper](payloads/19-binary-whisper/) | windows | types a line of binary, pauses, then reveals it spells QUACK. |
| 20 | [quack certificate popup](payloads/20-quack-certificate-popup/) | windows | pops a friendly windows dialog awarding you a quack, dismissed with ok. |
| 21 | [spotlight sonnet](payloads/21-spotlight-sonnet/) | macos | types a short duck poem into spotlight, then escapes out. nothing runs. |
| 22 | [say duck opera](payloads/22-say-duck-opera/) | macos | performs a tiny duck opera out loud with say. |
| 23 | [say beatbox](payloads/23-say-beatbox/) | macos | makes the mac beatbox boots-and-cats through say. |
| 24 | [mission control mambo](payloads/24-mission-control-mambo/) | macos | runs a short mission-control and show-desktop dance. |
| 25 | [invert-o-vision (mac)](payloads/25-invert-o-vision-mac/) | macos | inverts the whole display for a few seconds, then flips it back. |
| 26 | [dock magnify jiggle](payloads/26-dock-magnify-jiggle/) | macos | cranks dock magnification huge for ~6s, then puts your settings back. |
| 27 | [textedit typewriter confession](payloads/27-textedit-typewriter-confession/) | macos | textedit slowly types a confession that turns out to be from the duck. |
| 28 | [stickies love note](payloads/28-stickies-love-note/) | macos | drops a short wholesome duck sticky on the desktop. |
| 29 | [volume serenade](payloads/29-volume-serenade-mac/) | macos | ramps the volume up in steps with a ping at each, then restores the exact original level. |
| 30 | [mac emoji picker parade](payloads/30-emoji-picker-mac/) | macos | opens textedit and walks emoji in through the character viewer. |
| 31 | [xrandr barrel roll](payloads/31-xrandr-barrel-roll/) | linux | flips the x11 display 180 for five seconds, then rights it. |
| 32 | [spd-say robo-poet](payloads/32-spd-say-robopoet/) | linux | reads a short robotic ode to rubber ducks out loud. |
| 33 | [notify-send duck parade](payloads/33-notify-send-duck-parade/) | linux | fires a few friendly desktop notifications, then they expire. |
| 34 | [cursor theme swap (gnome)](payloads/34-cursor-theme-swap-gnome/) | linux | saves the gnome cursor theme, swaps it for eight seconds, then restores the exact one. |
| 35 | [wallpaper of the day (gnome)](payloads/35-gnome-wallpaper-of-the-day/) | linux | saves your gnome background, paints it solid hot-pink for six seconds, then restores it. |
| 36 | [ascii duck pond](payloads/36-ascii-duck-pond-terminal/) | linux | prints an ascii duck pond into the terminal. |
| 37 | [figlet-or-echo banner](payloads/37-figlet-echo-banner/) | linux | prints a big QUACK banner with figlet, or plain text if figlet isn't installed. |
| 38 | [xdg-open wholesome detour](payloads/38-xdg-open-wholesome/) | linux | opens the browser to a useless-but-harmless site via xdg-open. |
| 39 | [cowsay fortune duck](payloads/39-cowsay-fortune-duck/) | linux | a cowsay duck reads a fortune, with plain-text fallbacks if the tools aren't installed. |
| 40 | [os-aware greeter](payloads/40-os-aware-greeter/) | cross-platform | reads $_OS and greets you per platform: notepad on windows, textedit on macos, an echo on linux. |
| 41 | [build your own duck](payloads/41-build-your-own-duck/) | cross-platform | types a note explaining it was a ducky prank, plus how to build your own. |
| 42 | [button encore](payloads/42-button-encore/) | cross-platform | opens notepad and arms the ducky's button so each press types a random duck joke. |
| 43 | [ghost in the machine](payloads/43-jitter-typewriter-ghost/) | windows | a ghost types an eerie note with glitchy static, then reveals it's just a duck. |
| 44 | [duck fortune cookie](payloads/44-fortune-cookie-rng/) | windows | rolls one of five duck fortunes into notepad, different each run. |
| 45 | [dice duel vs the duck](payloads/45-dice-duel-rng/) | macos | you and the duck each roll a die into textedit, and it calls the winner. |
| 46 | [quack pyramid](payloads/46-quack-pyramid/) | windows | builds a growing pyramid of the word quack, one more per line. |
| 47 | [function duck chorus](payloads/47-function-duck-chorus/) | linux | opens nano on an empty buffer and sings a verse/chorus duck song from two functions. |
| 48 | [ducky traffic light](payloads/48-led-traffic-light/) | cross-platform | runs a red-then-green routine on the ducky's own onboard led. types nothing. |
| 49 | [caps-lock morse: quack](payloads/49-caps-morse-quack/) | cross-platform | blinks the caps lock led in morse to spell QUACK. |
| 50 | [the duck of theseus](payloads/50-duck-of-theseus/) | cross-platform | opens a throwaway editor, muses about a duck whose quacks all get replaced, then says how to disarm it. |

## duckyscript 3.0 bits used

decent spread if you're learning 3.0: STRING/STRINGLN, DELAY timing, DEFAULTCHARDELAY,
chords, HOLD/RELEASE, the onboard LED_R/LED_G/LED_OFF, caps-lock led tricks, RANDOM_CHAR
and the $_RANDOM_MIN / $_RANDOM_MAX / $_RANDOM_INT integer rng, VAR and DEFINE,
IF/ELSE IF/ELSE, single and nested WHILE, FUNCTION, BUTTON_DEF, jitter
($_JITTER_ENABLED / $_JITTER_MAX), and $_OS branching via the os_detect extension.

## contributing

more harmless gags welcome. to keep it clean:

- stay inside the "what's not in here" list. reversible, traceless, good-natured, or it
  gets closed.
- one folder per payload: `payloads/NN-slug/payload.txt`, kebab-case slug, plus a
  `README.md` in the folder only if the gag needs setup notes.
- keep the header block on every payload.txt: title, description, target os, novelty,
  revert, author.
- make it new. check the table and the hak5 repo first.
- compile it in payload studio before the pr, and use real delays (let the hid
  enumerate, let apps open).

## license

mit, see LICENSE.
