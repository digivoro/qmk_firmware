# Default keymap for Sofle Keyboard

Modificacion del default Sofle Keyboard, con Dvorak programador en lugar de Colemak.

Features:

-   Symmetric modifiers (CMD/Super, Alt/Opt, Ctrl, Shift)
-   Various modes, can be switched (using Adjust layer and the selected one is stored in EEPROM.
-   Modes for Qwerty and Dvorak support
-   Modes for Mac vs Linux/Win support -> different order of modifiers and different action shortcuts on the "UPPER" layer (the red one in the image). Designed to simplify transtions when switching between operating systems often.
-   The OLED on master half shows selected mode and caps lock state and is rotated.
-   Left encoder controls volume up/down/mute. Right encoder PGUP/PGDOWN.

# for pro micro-based builds

qmk flash -kb sofle/rev2 -km digivoro -bl avrdude-split-left
qmk flash -kb sofle/rev2 -km digivoro -bl avrdude-split-right

# for Elite C or dfu bootloader builds

qmk flash -kb sofle/rev2 -km digivoro -bl dfu-split-left
qmk flash -kb sofle/rev2 -km digivoro -bl dfu-split-right
