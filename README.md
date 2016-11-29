This is a xterm script to get simh-pdp8 to work with WPS-8.

On the [xterm](http://invisible-island.net/xterm/xterm.faq.html) website there is a script named `vmsterm`. This implements key remapping so that the numeric isle on your keyboard mimics the PF1-PF4 keys, it remaps the Backspace to send the correct RUB OUT CHAR (ascii 127) and other specific keys. It is intended for usage with VMS (PDP11 -> VAX -> VMS).

I used this script and the `showkey` command on my own `vt220` in `vt52` mode to get the correct keycodes for the numeric function keys. It works in the specific `vt52` mode required for WPS-8. It remaps the arrow keys as well:

- UP: LINE
- DOWN: LINE
- LEFT: BACKUP
- RIGHT: ADVANCE

See the WPS-8 guide on [my site](https://raymii.org) for a full explanation on the meaning of these specific keys. This mapping allows you to use left and right to go back one character and left/right + up/down to advance or go back one line at a time.


