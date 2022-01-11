<img src="https://github.com/acidanthera/OpenCorePkg/blob/master/Docs/Logos/OpenCore_with_text_Small.png" width="200" height="48"/>

## Hackintosh-OpenCore-DELL-7567
EFI premade of OpenCore bootloader for DELL-7567 is here!

## Current version - OpenCore 0.7.7 (11th January 2022!)
Repository contains full ,,Plug-and-Play" EFI of OpenCore bootloader and
all needed files to install and run macOS on DELL Inspiron 15 7000 Gaming (7567)!

https://github.com/acidanthera/OpenCorePkg/releases/tag/0.6.5

## Description:
<img src="https://zapodaj.net/images/f0d340d9df0c2.png" width="574" height="376"/>

### CPU: i5-7300HQ 4c4t 2,50-3,50GHz
### GPU: GTX 1050 GDDR5 4GB / i630
### RAM: 16GB DDR4 Dual-Channel 2400MHz SODIMM (2 x Micron 8ATF1G64HZ-2G3H1)
### SSD: ADATA SX8200PNP 256GB (PCI-E 3.0 x4)

## Important note:
My main DELL-7567 fried so won't be able keep up to date this repo anymore,
planning to get ThinkPad x240 and continue Hackintosh repos soon.

### Please note:
Since OC 0.6.5, I decided to switch to RELEASE version, if you expierience any issues, switch to debug using Dortania's Guide:

https://dortania.github.io/OpenCore-Install-Guide/troubleshooting/debug.html

### SMBIOS:
Present in repo SMBIOS is not purchased Apple's device but for own sake, I don't advice you to use it.
...for own sake ;)

To generate SMBIOS you can use:
* GenSMBIOS:
https://github.com/corpnewt/GenSMBIOS
* OpenCore Auxiliary Tools:
https://github.com/ic005k/QtOpenCoreConfig

Tool doesn't matter really, you just need not valid or unused SMBIOS to copy-paste needed info.
...if you wish to use iServices of course :)

### If you use Intel:
Delete all Brcm kexts from EFI/OC/Kexts, 
Depending on macOS version, you're planning to use:
* Airportitlwm for macOS 12 Monterey and delete rest.
* Airportitlwm_Big_Sur for macOS 11 Big Sur,
* Airportitlwm_Catalina for macOS 10.15 Catalina,
* Airportitlwm_Mojave for macOS 10.14 Mojave,
* Airportitlwm_High_Sierra for macOS 10.13 High Sierra.
After that rename chosen Airportitlwm kext to Airportitlwm.kext


## Credits:

### Airportitlwm:
https://github.com/OpenIntelWireless/itlwm
### AppleALC:
https://github.com/acidanthera/AppleALC
### HibernationFixup:
https://github.com/acidanthera/HibernationFixup/
### IntelBluetoothFirmware:
https://github.com/OpenIntelWireless/IntelBluetoothFirmware
### Lilu:
https://github.com/acidanthera/Lilu/
### NVMeFix:
https://github.com/acidanthera/NVMeFix
### RealtekRTL8111:
https://github.com/Mieze/RTL8111_driver_for_OS_X
### USBInjectAll:
https://bitbucket.org/RehabMan/os-x-usb-inject-all/downloads
### VirtualSMC:
https://github.com/acidanthera/VirtualSMC
### VoodooInput:
https://github.com/acidanthera/VoodooInput
### VoodooPS2:
https://github.com/acidanthera/VoodooPS2
### WhateverGreen:
https://github.com/acidanthera/WhateverGreen
### OpenCanopy's resources:
https://github.com/acidanthera/OcBinaryData
