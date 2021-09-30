# Herod2K Layout

Workman / Colemak DH Layout for OLKB Plank Rev6

## Compiling and flashing

1. Setup your QMK environment locally (https://docs.qmk.fm/#/newbs_getting_started)
2. Copy this folder inside: `qmk_firmware/keyboards/planck/keymaps/`
3. Put the keyboard in reset mode (LWR + RSE + Q)
4. From the project root folder launch the build/fiash using the docker utility:  

```
util/docker_build.sh planck/rev6:herod2k:flash
```

### Edit the currente configuration

Edit the `keyboard-layout.json` and generate a new file
```
qmk json2c -o keymap.c keyboard-layout.json
```

## Changelog (from default)

- Removed all layouts except QWERTY
- Moved Qwerty to level 1
- Configured Workman Layout on level 0
- Configured Colemak DH on level 2
- Added long press on Enter to get Shift
- Switched ESC with TAB
- Moved CTRL to the bottom left
- Moved LEFT ALT on the left of LWR and put FN and OS between them
- Added right CTRL on keypress on the right arrow
- Changed BL Cycle for left Shift + left CTRL on hold and delete on tap

The rest of the configuration follows the default structure

## Instructions

- LWR + RSE + N (on Workman layout): Changes to Workman 
- LWR + RSE + E (on Workman layout): Changes to QWERTY 
- LWR + RSE + O (on Workman layout): Changes to Colemak DH
- LWR + RSE + Q: Reset mode

