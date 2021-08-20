# LLKeyboard
**(Keypad layout for Linear Logic)**

This describes how to configure your keyboard to get direct access to the main utf-8 symbols for linear logic. The input of linear logic formulas becomes as easy as for arithmetic expressions.

*The following instructions have been tested on Linux Ubuntu 18.04 only.
Fell free to tell us if it works under other distributions or how to adapt it, or to report any trouble by submitting an issue or a pull-request on GitHub.*

The generated keymap is depicted in [map_utf8.txt](map_utf8.txt).

## Ubuntu 18.04

Use files from the directory corresponding to the language you want to rely on. Only the keypad is modified (other keys correspond to the selected keyboard layout).
Currently available languages are:

 * fr (French)
 * us (English US)

Installation instructions are:

 * copy the `ll` file in `/usr/share/X11/xkb/symbols/`
 * add the lines from `evdev_lines.xml` to `/usr/share/X11/xkb/rules/evdev.xml` in the layout part, that is between `<layoutList>` and `</layoutList>` (for example just before `</layoutList>`)
 * add the line from `evdev_lines.lst` to `/usr/share/X11/xkb/rules/evdev.lst`
 * reboot
 * the new layout can be activated in `System Settings` (`Region and Language` / `Input Sources`): click on the `+` button, select the language and select `Keypad for Linear Logic`
 * you can use keyboard switching on the panel
