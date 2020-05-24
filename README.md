# MSI Z370i Gaming Pro Carbon AC Hackintosh Build - OpenCore

### Hardware Components
- MSI Z370i Gaming Carbon Pro AC
- Intel i3-8100
- 8GB Corsair 2400MHz
- Gigabyte RX460 4GB
- WD Black M.2 SSD 240GB

### What's Working/What's Not

#### Working
- Ethernet
- Audio (including DP/HDMI audio)
- APFS
- Sleep/Wake
- Headless iGPU
- All USB ports (USB2, USB3)
- iMessage
- App Store
- Facetime
- Bluetooth
- Native Power Management

#### Not Working
- Built-in WiFi (Not supported by macOS)
- Built-in Bluetooth (Works but cannot be turned off)

#### Not Tested
- FileVault
- USB-C

### Kexts
This build relies on the following kexts.
- [Lilu](https://github.com/acidanthera/lilu/releases)
- [WhateverGreen](https://github.com/acidanthera/whatevergreen/releases)
- [AppleALC](https://github.com/acidanthera/applealc/releases)
- [VirtualSMC](https://github.com/acidanthera/virtualsmc/releases)
- SMCProcessor - included with VirtualSMC
- SMCSuperIO - included with VirtualSMC
- [IntelMausi](https://github.com/acidanthera/IntelMausi/releases)
- [NVMeFix](https://github.com/acidanthera/NVMeFix/releases) - Only if using an NVMe SSD
- USBPorts - Included in this repo. All ports included except for the internal Bluetooth (HS11). If you wish to use the internal Bluetooth, make sure to include port HS11 in the included USB.plist and generate the kext using [USBMap tool](https://github.com/corpnewt/USBMap)

### SSDTs
This motherboard works OOB with the included SSDTs from OpenCore package. No special config needed.
- SSDT-EC-USBX
- SSDT-PLUG
- SSDT-SBUS-MCHC

#### PlatformInfo
Make sure to generate and fill up your own PlatformInfo


### Guide Used
[Opencore-Vanilla-Desktop-Guide](https://khronokernel.github.io/Opencore-Vanilla-Desktop-Guide/).

### Credits
Special thanks to:
- [OpenCore](https://github.com/acidanthera/OpenCorePkg) team for the bootloader.
- [corpnewt](https://github.com/corpnewt) for the tools used.
- [acidanthera](https://github.com/acidanthera) for the kexts.
- Entire Hackintosh community for the support.
