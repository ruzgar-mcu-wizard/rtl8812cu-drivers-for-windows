[![License](https://img.shields.io/badge/License-View-blue.svg)](./LICENSE)

## Realtek RTL8812CU 802.11ac USB Wi-Fi Driver for Windows

- ⚡ **Single EXE installer** (*9.88 MB*), installs *94.4 MB*
- ⚡ Manual install using **.cat** and **.inf** files
- 💻 **Supports** Windows 7, 8, 8.1, 10, and 11 (x86 & x64)
- 📶 **Works with** *RTL8812CU* 802.11ac USB Wi-Fi adapters
- ✅ **Just works** — plug in, run installer, get Wi-Fi
- ❌ **No maintenance, no updates, no nonsense**
- 📱 **Known Working Devices: RTL8812CU (VID: 0BDA PID: C812)**
- 📡 **Only works with RTL8812CU, don’t plug in random Wi-Fi dongles expecting magic.**
- 🗃 Driver Version: 1030.44.727.2022
- 📆 Release Date: 18.10.2022
- 📥 Source: Realtek OEM Package

## Supported vs Unsupported Dongles (⚠ IMPORTANT)

| Chipset   | Support   | Notes                     |
| --------- | --------- | ------------------------- |
| RTL8812CU | ✅ Yes   | This repo                 |
| RTL8811CU | ❌ No    | Requires different driver |
| RTL8821CU | ❌ No    | Requires different driver |
| RTL8812AU | ❌ No    | Different architecture    |

## Architecture
Do not forget that x64 is for 64-bit Windows installation, x86 is for 32-bit Windows installation.

## Why Does This Exist?
Many RTL8812CU adapters ship without reliable Windows drivers or rely on outdated OEM packages. This repository provides a verified, clean, and easy-to-install driver bundle.

## Installation

If you run the installer you'll see:

![Install](./images/install.png)

If you run the installer again while it’s already installed, you’ll see:  

![Overwrite?](./images/overwrite.PNG)

Choose **Yes** if you want to reinstall.

Choose **No** if you don't want to reinstall.

### Download

[Download Setup](./rtl8812cu.exe)

## How To Check Your Dongle

- **Plug in** the dongle
- Open **Device Manager** (Or **Win+R, devmgmt.msc, enter**)
- **Right click** the device → **Properties** (Or **double left click**)
- Go to **Details** tab
- Select **Hardware IDs**

The ID should be ONLY these:

**USB\VID_0BDA&PID_C812**

**USB\VID_0BDA&PID_C812&REV_0000**

## Antivirus False Positives

Some antivirus engines may flag this installer due to:
- Kernel-mode driver installation
- SYSTEM-level privilege usage
- Self-extracting installer behavior

The driver is **Microsoft Windows Hardware Compatibility Publisher** signed and sandbox analysis (CAPA / Zenbox / VirusTotal Jujubox / CAPE Sandbox / C2AE) shows no malicious behavior.

You can check the Setup here: [VirusTotal](https://www.virustotal.com/gui/file/32d5194252fe20ce4ded077daa05f49340ff367526231e11c7ded7646d0df8f1).

You can check the Driver Source Code here: [VirusTotal](https://www.virustotal.com/gui/file/79ad3b5ce5d5995be1e4fd8844a4b244f6c23aad64c9d5d908250f54139c3a99)

All driver files retain original Microsoft signatures.

## Manual Installation

If you want to install **manually**:

- Go to **Device Manager** (or Win+R, devmgmt.msc, enter),

- **Right click the dongle**

- Go to **Drivers** tab

- **Update Drivers**

- **Browse drivers**

- Open the compatible version for your OS (**Windows 10 driver** for **Windows 11**, **Windows 8 x86 driver** for **Windows 8.1 x86**, dont forget to match **Architecture (x86 / x64)**)

- Click **Finish**, done!

The manual install drivers are [**Here**](./Realtek/WifiAutoInstall/Drivers).

## Setup Hashes

*SHA256*: ```32D5194252FE20CE4DED077DAA05F49340FF367526231E11C7DED7646D0DF8F1```

*SHA512*: ```5CC1B62D2D91E42886D60FF9BB9B9E9A7138987D9B554755C32D77C56517A8AACBEB0DEFC605226A742738D857AE5466A3258A653B54828E523C78F59FB2B834```

*MD5*: ```36F3B7C226FC05E29929BEA264AD0A3A```

## Driver-Source-Code.zip Hashes

*SHA256*: ```79AD3B5CE5D5995BE1E4FD8844A4B244F6C23AAD64C9D5D908250F54139C3A99```

*SHA512*: ```C3724F4EB682F14E21EBE6229DFBFEEB84CE99B5B5FA9461DE6448D80933F4855519FD4BA5ED1FC43CA27EDA138C0F050DAEC5224B310061D8F1A4C5B9825CB9```

*MD5*: ```A4A66356CD983E0A324664899C8C9779```

## RTL8812CU USB Dongle

![Wi-Fi Dongle](./images/wifi_dongle.png "RTL8812CU 802.11ac USB Wi-Fi dongle")

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
  - Go to [**Here**](./Realtek/WifiAutoInstall), run the **unins000.exe**, re-install driver. (Or launch the setup again, click **Yes** to the overwrite message, then click **Install**)
  - If that doesn't work, check the dongle's **VID and PID** (Hardware IDs) from Device Manager, **Network Adapters**, **Find the dongle**, Right click, **Properties**, **Details**, **Property**, choose **Hardware IDs**, make sure its **USB\VID_0BDA&PID_C812** (or close like **USB\VID_0BDA&PID_C812&REV_0000**)

## Contact
Questions, driver issues, or cursed Wi-Fi setups? Reach me at: **ruzgarefecelik67@gmail.com**

Check my [YouTube channel](https://www.youtube.com/channel/UCh0Gprh0Ou6Ah2s-69SvjJQ) or [Custom ROM Vault](https://bit.ly/m/customromvault) for more cursed projects.
