# How To Install A GSI?
- Install TWRP with [this guide](HOW_TO_INSTALL_TWRP.md).
- Install ADB & Fastboot with [this guide](HOW_TO_INSTALL_ADB_FASTBOOT.md).
- Choose a working GSI from either [my list](README.md) or from the [Offical TrebleDroid GSI List](https://github.com/TrebleDroid/treble_experimentations/wiki/Generic-System-Image-(GSI)-list).
- Download the GSI and extract it. It needs to be a `.img`.
- Reboot into TWRP.
- Wipe Data, Dalvik/ART Cache, and other stuff that needs to be cleaned.
  > It might show mount errors, just don't mind them and continue.
- Wipe the Internal Storage.
> [!IMPORTANT]
> ***DO NOT WIPE THE sdcard SECTION. IF YOU WIPE IT, YOUR PHONE WILL ENTER QDL MODE AFTER YOU REBOOT.***
- Go back to the main menu and click Reboot > Fastboot.
- Once in fastboot, plug in your phone to your PC.
- Type `fastboot -w` to wipe again.
- Write `fastboot flash system /path/to/your/downloaded/gsi.img` and wait for it to finish flashing.
- Once it finishes, just wait for it to Boot into the OS.

# FAQ
### It Throw Me Back To TWRP From Samsung Logo Screen After Re-Booting From The First Boot. How Can I Fix It?
You don't need to fix it.
It's a good sign that the GSI would work.
It throw you to TWRP because it wants you to **Wipe the Internal Storage** for it to Boot up.
Just wipe the Internal Storage and reboot to system.

### It Bootloops, What Should I Do Now?
Just flash a new GSI.

### I Can't Enter The TWRP and My Phone Bootloops, Now What?
Just force off your phone by holding **all the hardware** buttons at once.
Once it closed, immediately enter the `Download Mode` and re-flash TWRP.
Then enter it with holding **Power Up + Vol+**, don't worry, the system will not overwrite it now since you installed a GSI to the system partition.

### The GSI That I Downloaded Lags A Lot, What Should I Do?
Just try a new one or do some tweakiing in the Treble App Display options.