
- You need to have your Bootloader Unlocked. Check how to do it [here](HOW_TO_UNLOCK_BOOTLOADER.md).
- Grab TWRP for this device from [this page](https://github.com/khazar-os-linux/My-Galaxy-A02s-Journey/raw/refs/heads/main/resources/twrp-3.7.1-a02q-unofficial.img.tar). This is recommended one.
- Enter [download mode](HOW_TO_UNLOCK_BOOTLOADER.md) on your phone.
- Plug your phone into your computer.
- Flash the downloaded TWRP file with odin or brokkr.
  Odin:
    Enter `odin4 -a /path/to/twrp.img.tar` from terminal.

   Brokkr:
	Put your `twrp.img.tar` file into the AP section and click to `START` button.

- Once it finishes, you need to **IMMEDIATELY** enter TWRP with **Power + Vol+** once the `Download Mode` closes. Otherwise the Stock OS will overwrite it with the Stock Recovery.

Congrats! You now have TWRP installed on your device.
You can now reboot to your system.

# FAQ
### It Replaced TWRP with the Stock Recovery Even Though I Entered TWRP Immediately. How Can I Fix it?
Just re-flash TWRP. It's not your fault.

### There Are A Lot Of Mount Errors. How To Fix them?
Samsung made most of the part of the filesystem read-only. You can try re-flashing TWRP again.

### Is There Any OrangeFox Builds For This Device?
Unofficial OFox builds are dead for this device. 