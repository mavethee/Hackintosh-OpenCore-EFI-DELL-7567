<img src="https://github.com/acidanthera/OpenCorePkg/blob/master/Docs/Logos/OpenCore_with_text_Small.png" width="200" height="48"/>

## Hackintosh-OpenCore-DELL-7567
EFI premade of OpenCore bootloader for DELL-7567 is here!

## Current version - OpenCore 0.9.3 DEBUG
Repository contains full ,,Plug-and-Play" EFI of OpenCore bootloader and
all needed files to install and run macOS on DELL Inspiron 15 7000 Gaming (7567)!

https://github.com/acidanthera/OpenCorePkg/releases/tag/0.9.3

## Sonoma NOTE:

Apple still didn't remove any of kext for Kaby Lake's iGPUs.
So if you wish to run Sonoma, at current state (as of Beta 2), make sure you'll use `MacBookPro15,1`

See `SMBIOS` section below as for working iServices you're required to do so anyways.
Might eventually with time just change it, depending what Apple will do.
And technically thanks to Intel, KBL -> CFL spoof seems to be a thing.

Too early to tell.

P.S. Intel WiFi kexts are dead for now, use Ventura or replace WiFi card if it's a dealbreaker!

See progress here:

https://github.com/OpenIntelWireless/itlwm/issues/883

## Ventura NOTE:

Since it's Kaby Lake machine, it's one of the last machines of Apple's natively supported list hopefully so it probably requires
a few tweaks and you're mostly good to go.
One key difference that after a while seems to be useful is using `MacBookPro15,1` SMBIOS for Hey Siri thing working, now it's macOS Sonoma way to go!
Happy Hackintoshing!! ^^

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
