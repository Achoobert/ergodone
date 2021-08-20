# ErgoDox EZ Default Configuration

## to build
// inside wsl2
// cp -R <source_folder> <destination_folder>
// copy these files into wsl// cp -R /mnt/d/schubert.dev/qmk_firmware/keyboards/ergodone/keymaps/Achoobert /home/achoobert/qmk_firmware/keyboards/ergodone/keymaps
// qmk compile -kb ergodone -km Achoobert
// copy back // cp -R /home/achoobert/qmk_firmware/.build/ergodone_Achoobert.hex /mnt/d/schubert.dev/qmk_firmware/.build

// activate the hardware's writable mode with rightmost key of left side
// https://github.com/qmk/qmk_firmware/blob/master/keyboards/ergodone/readme.md
// need old ".\hid_bootloader_cli.exe"
// run command using powershell
// cd qmk_firmware/.build/
// ./hid_bootloader_cli.exe -mmcu=atmega32u4 ergodone_Achoobert.hex

## Changelog

* Aug 18, 2021 (V1.2): 
  * Base config is colemac mod-dh
  * holding right-pinky key enables a 
    * print screen
    * right-hand home-row arrow keys
    * left-hand home-row 'opener' keys: '{' '[' '(' 
  * Top inner keys on each side change workspace in windows
  * Bottom left key toggles QWERTY gaming layer
    * has esc key
    * has tab, ctrl more accessable 
  * Experimenting with 
    * shift being on a thumb key. I liked that backspace was accessable, but it made accuracy feel less important.
* Feb 2, 2016 (V1.1): 
  * Made the right-hand quote key double as Cmd/Win on hold. So you get ' when you tap it, " when you tap it with Shift, and Cmd or Win when you hold it. You can then use it as a modifier, or just press and hold it for a moment (and then let go) to send a single Cmd or Win keystroke (handy for opening the Start menu on Windows).
* Sep 22, 2016:
  * Created a new key in layer 1 (bottom-corner key) that resets the EEPROM.
* Dec 2016:
  * Added LED keys
  * Refreshed layout graphic, comes from http://configure.ergodox-ez.com now.

This is what we ship with out of the factory. :) The image says it all:

![Default](https://i.imgur.com/Be53jH7.png)
