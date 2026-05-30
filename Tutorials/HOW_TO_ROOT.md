# How To ROOT This Device
You got 1 options here.
- Magisk - User Space

## KernelSU-Next
> [!IMPORTANT]
> Works only 64 bit vendor. I've never tried this.

Here is the [link](https://github.com/ifoodplayer/android_kernel_samsung_sdm450/releases)
## Magisk
### Extracting the AP
- Extract the firmware and take the `AP` file.

### Check
- Firstly, you need to unlock your Bootloader using [this guide](HOW_TO_UNLOCK_BOOTLOADER.md).

### Installing Magisk
- Grab the magisk manager APK file from [this page](https://github.com/topjohnwu/Magisk/releases/tag/v30.6).
- After that, install it.
- Grab the `AP` file that you extracted before and copy it over to your phone.
- Open up magisk manager and select **Install**.
- Select **Patch Method**.
- Select the `AP` file that you copied over from you computer.
- Once the patching finishes, go to you Downloads folder from your phone and grab the `magisk_patchedxxxx.img.tar` file, and copy it to your computer.
- Enter the [download mode](HOW_TO_BOOTLOADER.md#how-to-enter-download-mode) and flash the magisk patched `AP` file with Odin or [brokkr flash tool](https://github.com/Gabriel2392/brokkr-flash). Learn how to install Odin and brokkr on your Linux `(first 3 steps)` 

Odin:
    Enter `odin4 -a /path/to/magisk_patchedxxxx.img.tar` from terminal.
- When it's done, set-up your phone and you should now a Magisk app on your home screen which'll download the magisk manager.
- Once it's downloaded and installed, it'll ask you to do some required stuff to actually set up root. Just accept it.

Brokkr:
    Just open the app and put your `magisk_patchedxxxx.img.tar` into the AP section.
-  When it's done, set-up your phone and you should now a Magisk app on your home screen which'll download the magisk manager.
- Once it's downloaded and installed, it'll ask you to do some required stuff to actually set up root. Just accept it.
# FAQ
### Will The Magisk Get Deleted When I Install A GSI?
No, it'll not. Now it's a part of your phone ;).