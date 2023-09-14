<img src="https://github.com/acidanthera/OpenCorePkg/blob/master/Docs/Logos/OpenCore_with_text_Small.png" width="200" height="48"/>

# Hackintosh-OpenCore-DELL-7567

Welcome to the Hackintosh-OpenCore-DELL-7567 repository! Here, you'll find a pre-made EFI setup for the OpenCore bootloader tailored to work with the DELL Inspiron 15 7000 Gaming (7567) laptop.

## Current Version - OpenCore 0.9.5 DEBUG

This repository contains a "Plug-and-Play" EFI configuration for the OpenCore bootloader, along with all the necessary files to install and run macOS on your DELL Inspiron 15 7000 Gaming (7567). For the most up-to-date version, please visit the [OpenCore 0.9.5 release](https://github.com/acidanthera/OpenCorePkg/releases/tag/0.9.5).

## Sonoma Note:

Please note that Apple has not yet removed any of the kexts for Kaby Lake's iGPUs. Therefore, if you intend to run Sonoma, you should currently use the `MacBookPro15,1` SMBIOS as described in the "SMBIOS" section below. This is necessary for easier booting and certain iServices to work correctly. Keep an eye on updates from Apple as this may change in the future and require spoofing like in Skylake case. Thanks to Intel, Kaby Lake to Coffee Lake spoofing appears to be an option, but it's still early days.

**P.S.**: Intel WiFi kexts are not functioning at the moment. Consider using Ventura or replacing your WiFi card if this is critical. Check the progress [here](https://github.com/OpenIntelWireless/itlwm/issues/883). You can also use HeliPort with itlwm as an alternative for now.

## Ventura Note:

Since your machine is Kaby Lake-based, it's one of the last machines natively supported by Apple's list. Therefore, it may require a few tweaks, but you should be good to go. One notable difference is that using the `MacBookPro15,1` SMBIOS seems to be useful for enabling Hey Siri functionality, which is now the way to go in macOS Sonoma. SMBIOS ofc, not Hey Siri xD. Happy Hackintoshing! ^^

### SMBIOS:

The included SMBIOS in this repository is not a purchased Apple device, so it's not recommended for use.

To generate your own SMBIOS, you can use the following tool:
- [GenSMBIOS](https://github.com/corpnewt/GenSMBIOS)

**REMEMBER:** You need a unvalid or unused SMBIOS to copy-paste the required info if you wish to use Apple iServices.

To ensure you generated right one, visit [Apple's Check Coverage page](https://checkcoverage.apple.com/).

## Credits:

- [Airportitlwm](https://github.com/OpenIntelWireless/itlwm)
- [AppleALC](https://github.com/acidanthera/AppleALC)
- [HibernationFixup](https://github.com/acidanthera/HibernationFixup/)
- [IntelBluetoothFirmware](https://github.com/OpenIntelWireless/IntelBluetoothFirmware)
- [Lilu](https://github.com/acidanthera/Lilu/)
- [NVMeFix](https://github.com/acidanthera/NVMeFix)
- [RealtekRTL8111](https://github.com/Mieze/RTL8111_driver_for_OS_X)
- [USBInjectAll](https://bitbucket.org/RehabMan/os-x-usb-inject-all/downloads)
- [VirtualSMC](https://github.com/acidanthera/VirtualSMC)
- [VoodooInput](https://github.com/acidanthera/VoodooInput)
- [VoodooPS2](https://github.com/acidanthera/VoodooPS2)
- [WhateverGreen](https://github.com/acidanthera/WhateverGreen)
- [OpenCanopy's resources](https://github.com/acidanthera/OcBinaryData)
