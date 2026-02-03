[![License](https://img.shields.io/badge/License-View-blue.svg)](./LICENSE)

## Realtek RTL8212CU 802.11ac USB Wi-Fi Driver for Windows

- ⚡ **Single EXE installer** (*9.88 MB*), installs *82.06 MB*
- ⚡ Manual install using **.cat** and **.inf** files
- 💻 **Supports** Windows 7, 8, 8.1, 10, and 11 (x86 & x64)
- 📶 **Works with** *RTL8212CU* 802.11ac USB Wi-Fi adapters
- ✅ **Just works** — plug in, run installer, get Wi-Fi
- ❌ **No maintenance, no updates, no nonsense**
- 📱 **Known Working Devices: RTL8212CU (VID: 0BDA PID: C812)**
- 📡 **Only works with RTL8212CU, don’t plug in random Wi-Fi dongles expecting magic.**

## Installation

If you run the installer you'll see:

![Install](./images/install.png)

If you run the installer again while it’s already installed, you’ll see:  

![Overwrite?](./images/overwrite.PNG)

Choose **Yes** if you want to reinstall.

Choose **No** if you don't want to reinstall.

[Download EXE](./rtl8212cu.exe)

If you are paranoid you can check it in [VirusTotal](https://www.virustotal.com/gui/file-analysis/MjQyODY5ZWE5MTdiOTc1NWYwMTBiNDM0ZmNjYjJlZTU6MTc3MDAyOTg2Nw==).

Digital Driver Signer is **Microsoft Windows Hardware Compatibility Publisher**.

## Manual Installation

If you want to install **manually**, go to **Device Manager** (or Win+R, devmgmt.msc, enter), **right click the dongle**, go to **Drivers** tab, **Update Drivers**, **Browse drivers**, open the compatible version (**Windows 10 driver** for **Windows 11**, **Windows 8 x86 driver** for **Windows 8.1 x86**), click **Finish**, done!

The manual install drivers are inside [**Here**](./Realtek/WifiAutoInstall).

## Hashes

*SHA256*: ```091FF20ECC58A964339FC3FE158076D4FF82151261291EB37A8CBB2773368CD3```

*SHA512*: ```CDF0E2352E84A39BD2AE1F015125765D564F86D40F9365DBC648320E0EFA1B2D1F08B3CB02F6EDC7F408936DB43F5C7EF631668AB17119E3969E60ECF03BAC41```

*MD5*: ```603BF3F021228A732D8DE75F70ED0B2```

## RTL8212CU USB Dongle

![Wi-Fi Dongle](./images/wifi_dongle.png "RTL8212CU 802.11ac USB Wi-Fi dongle")

*For reference only*

## Troubleshooting
1. Device Not Detected
  - Try **rebooting** your PC,
  - Try a **different USB** port,
  - Do **not** use hubs or extension cables,
  - Open **Device Manager**, check under **Network Adapters** and **Universal Serial Bus Controllers**

2. Wi-Fi Not Working
  - Try **rebooting** your PC,
  - Use the **Rear USB** ports (if you were using front USB ports and rear is available),
  - Try a **powered hub** (if you have one),

3. Random Disconnects
  - Try **rebooting** your PC,
  - Go to **Device Manager** (or Win+R, devmgmt.msc, enter), Go to **Network Adapters**, **Find the dongle**, Right click, **Properties**, **Power Management** tab, **Uncheck Allow Windows to turn off this device to save power**, Reboot

4. Still Broken?
  - Go to [**Here**](./Realtek/WifiAutoInstall), run the **unins000.exe**, re-install driver.
  - If that doesn't work, check the dongle's **VID and PID** (Hardware IDs) from Device Manager, **Network Adapters**, **Find the dongle**, Right click, **Properties**, **Details**, **Feature**, choose **Hardware IDs**, make sure its **USB\VID_0BDA&PID_C812** (or close like **USB\VID_0BDA&PID_C812&REV_0000**)

## Contact
Questions, driver issues, or cursed Wi-Fi setups? Reach me at: **ruzgarefecelik67@gmail.com**

Check my [YouTube channel](https://www.youtube.com/channel/UCh0Gprh0Ou6Ah2s-69SvjJQ) or [Custom ROM Vault](https://bit.ly/m/customromvault) for more cursed projects.
