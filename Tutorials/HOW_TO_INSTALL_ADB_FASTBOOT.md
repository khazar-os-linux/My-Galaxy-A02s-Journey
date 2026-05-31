# How To Install ADB & Fastboot?
## Linux
### Official Distro Packages
- Search for terms like `android-tools`, `adb`, `fastboot` with your package manager.
- Find the appropriate ones, and install them.
### From Google
- Here's a quick command for you:
  ```bash
  curl -L https://dl.google.com/android/repository/platform-tools-latest-linux.zip -o pt.zip && unzip -j pt.zip "platform-tools/adb" "platform-tools/fastboot" && sudo mv adb fastboot /usr/bin/ && rm pt.zip
  ```
  It'll gonna download `platform-tools-latest-linux.zip` as `pt.zip`, extract it, put the `adb` and `fastboot` to `/bin` with sudo, and remove the `pt.zip` later.

Done! You've successfully installed ADB & Fastboot!
