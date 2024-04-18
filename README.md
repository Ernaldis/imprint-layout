# ZMK Configuration Template
Bluetooth firmware configuration for Cyboard keyboards using ZMK firmware.
More information can be found here: [ZMK Documentation](https://zmk.dev/docs)
Click "use this template" to create a copy of this repository for your own use.

# Changing your Keymap in ZMK Keymap Editor (Beta)
1. Navigate to [https://nickcoutsos.github.io/keymap-editor/](https://nickcoutsos.github.io/keymap-editor/)
2. Sign into github and link to this repository.
3. Make changes to the layout and press "Commit Changes."
[more info can be found here](https://github.com/nickcoutsos/keymap-editor/wiki/Features)

# Changing your Keymap in ZMK text files
1. Make the desired edits to `cyboard.keymap` and commit them.

# Flashing the firmware to your Cyboard
1. GitHub will automatically run an Action to build your firmware. this takes approximately 2 minutes for most changes.
2. Once the Action is successful, there will be a firmware Artifact in the Action which you can download and unzip.
3. Connect the "central" (left) half of your Cyboard to your computer via USB.
4. Put your Cyboard in bootloader mode by double tapping the reset button next to the USB C port. Pro Tip:  The keycap puller that comes with your Cyboard will fit in the reset hole!
5. Copy the .uf2 file into the USB device named Nice Nano.
6. You're done! You can now disconnect your Cyboard from your computer.

# Hardware Notes
To enter bootloader mode, double tap the reset button on the back of your Cyboard.
The battery switch is a physical disconnect switch, so your battery *will not charge* if the switch is off (away from the USB port).  The switch is intended as a way to disconnect the battery for travel to avoid accidental keypresses that would drain the battery while it is in your bag.  For most other times, it can just be left connected (towards the USB port), and your Cyboard will sleep after 15 minutes of inactivity to conserve battery.
