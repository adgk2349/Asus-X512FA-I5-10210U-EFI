<h1 align="center">Asus-X512FA-I5-10210U-EFI </h1>

<p align="center">
    <a href="https://www.apple.com/">
        <img src="https://img.shields.io/badge/Sequoia-15.0.0-skyblue"/></a>
        <img src="https://img.shields.io/badge/OpenCore-1.0.2-blue"/></a>
</p>

<p align="center">
    <a href="https://paypal.me/run1213">
        <img src="https://img.shields.io/badge/-Buy%20me%20a%20coffee-orange.svg"></a>
</p>

#### I am not responsible for any damages you may cause.

#### If my work here helped you. Please consider donating, it would mean a lot to me.

- Complete EFI packs are available in the releases page.
- I will try my best to keep the repo updated with the latest kexts and OpenCore version.
- Please **do not clone or download** the main branch for daily use: it may include **unstable code** just because it is my repository.
- This EFI is configured with Only Sonoma.

## Update
- Updated to Sequoia EFI Configuration.
- Up to Sequioa 15.1 is supported. (Tested EFI is up to 15.0)
- All of iServices are work as native. (Except some of Wifi related services.)

<details>
<summary><strong> SUMMARY </strong></summary>
<br>

> ### Video and Audio

| Feature                              | Status | Dependency          |
| :----------------------------------- | ------ | ------------------- |
| Full Graphics Accleration (QE/CI)    | ✅   | `WhateverGreen.kext`                                            |
| Audio Recording                      | ✅   | `AppleALC.kext` with Layout ID = 55 and                  |
| Audio Playback                       | ✅   | `AppleALC.kext` with Layout ID = 55 and                  |
| Automatic Headphone Output Switching | ✅   | `AppleALC.kext` with Layout ID = 55 and                  |
| Dock Audio Port                      | ✅   | `AppleALC.kext` with Layout ID = 55 and                  |
| Apple Music                          | ❌   | Some music can play on airpods or bluetooth devices.     |
> ### Power, Charge, Sleep and Hibernation

| Feature                              | Status |
| :----------------------------------- | ------ |
| S3 Sleep/ Hibernation Mode 3         | ✅    | 
| Fan Control                          | ✅    |

> ### Input/ Output

| Feature                              | Status | Dependency          |
| :----------------------------------- | ------ | ------------------- |
| WiFi                                 | ✅   | `itlwm.kext`                                                             |
| Bluetooth                            | ✅   | `IntelBluetoothFirmware.kext` `IntelBTPatcher.kext` `BlueToolFixup.kext` |
| Ethernet                             | ✅   | -                                                                        |
| USB 2.0, USB 3.0                     | ✅   | `USBMap.kext`                                                            |
| USB Power Properties in macOS        | ✅   | `SSDT-PLUG.aml`                                                       |
| ASUS Fn Key                          | ✅   | Works with Brightness and Sound Control                                  |
| Backlight                            | ❌   | I added `AsusSMC.kext` to enable this feature, but it's not working      |
| primitive laptop feature             | ✅   | Many of `Voodoo__.kext` for work properly                                |

> ### macOS Continuity

| Feature                              | Status | Dependency          |
| :----------------------------------- | ------ | ------------------- |
| iCloud                               | ✅     | iMessage, FaceTime needs to change your SMBIOS                         |
| AirDrop                              | ❌     | Physically unable to use on Sequoia in native                          |
| Time Machine                         | ✅     | Native                                                                 |

</details>

<details>
<summary><strong> REFERENCES </strong></summary>
<br>

Read these before you start:

- [dortania's Hackintosh guides]<https://github.com/dortania>.
- [dortania's OpenCore Install Guide]<https://dortania.github.io/OpenCore-Install-Guide/>.
- [dortania's OpenCore Post Install Guide]<https://dortania.github.io/OpenCore-Post-Install/>.
- [dortania/ Getting Started with ACPI]<https://dortania.github.io/Getting-Started-With-ACPI/>.
- [dortania/ opencore `multiboot`]<https://github.com/dortania/OpenCore-Multiboot>.
- [dortania/ `USB map` guide]<https://dortania.github.io/OpenCore-Post-Install/usb/>.
- [ChefKissInc/ Radeon Card Accelerlation Guide]<https://github.com/ChefKissInc/NootRX>.
- `Configuration.pdf` and `Differences.pdf` in each `OpenCore` releases.
- [OpenIntelWireless's HeliPort github]<https://github.com/OpenIntelWireless/HeliPort>.

</details>

<details>
<summary><strong> REQUIREMENTS </strong></summary>
<br>

- A macOS machine(optional): to create the macOS installer.
- Flash drive, 32GB or more, for the above purpose.   
- [ProperTree](https://github.com/corpnewt/ProperTree) if you need to edit plist files on Windows.  
- [MountEFI](https://github.com/corpnewt/MountEFI) to quickly mount EFI partitions.  
- [IORegistryExplorer](https://developer.apple.com/downloads), for diagnosis.  
- [Hackintool](https://www.insanelymac.com/forum/topic/335018-hackintool-v286/), for diagnostic ONLY, Hackintool should not be used for patching, it is outdated.
- Patience and time, especially if this is your first time Hackintosh-ing.

</details>

<details>
<summary><strong> HARDWARE </strong></summary>
<br>

| Category  | Asrock B760M ITX D4 |
| --------- | ------------------------ |
| CPU       | Intel Core i5-10210U                       |
| GPU       | Intel UHD Graphics 620                     |
| SSD       | Western Digital WD MOBILE Blue 5400 500GB  |
| WiFi & BT | Intel(R) Wifi Chip integrated              |


- Refer to Various Companies that making electronics for possible Hackintosh configurations.

</details>

<details>
<summary><strong> GETTING STARTED </strong></summary>
<br>

Before you do anything, please familiarize yourself with basic Hackintosh terminologies and the basic Hackintosh process by throughly reading Dortania guides as linked in `REFERENCES`

- How To Create macOS installer: refer to [Dortania's OpenCore Install Guide](https://dortania.github.io/OpenCore-Install-Guide/installer-guide/)

</details>

<details>
<summary><strong> BENCHMARKS </strong></summary>
</br>

- macOS 14.3.1, EFI OpenCore 0.9.8

| CPU            | Single-Core  | Multi-Core  |
| :------------- | ----------:  | ---------:  |
| Geekbench 6    |         1100 |       3051 |

| GPU            | OpenCL       | Metal         |
| :------------- | ----------:  | ---------:    |
| Geekbench 6    |        -     |        -      |

</details>

# CONTACT

- Email: adgk2349b@gmail.com

# Credits

- [Apple](https://www.apple.com) for macOS and customer support etc.
- [Acidanthera](https://github.com/acidanthera) for all the kexts/utilities that they made.
- [Rehabman](https://github.com/RehabMan) and [Daliansky](https://github.com/daliansky) for the patches and guides and kexts.
- [George Kushnir](https://github.com/n4ru) for modified BIOS.
- [Dortania](https://github.com/dortania) for the OpenCore Install Guide.
