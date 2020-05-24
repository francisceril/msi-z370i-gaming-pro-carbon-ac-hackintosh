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
- Lilu
- WhateverGreen
- AppleALC
- VirtualSMC
- SMCProcessor
- SMCSuperIO
- IntelMausi
- NVMeFix - Only if using an NVMe SSD
- USBPorts - Included in this repo. All ports included except for the internal Bluetooth (HS11). If you wish to use the internal Bluetooth, make sure to include port HS11 in the included USB.plist and generate the kext.

### SSDTs
This motherboard works OOB with the included SSDTs from OpenCore package. No special config needed.
- SSDT-EC-USBX
- SSDT-PLUG
- SSDT-SBUS-MCHC

#### PlatformInfo
Make sure to generate and fill up your own PlatformInfo


### Guide Used
[Opencore-Vanilla-Desktop-Guide](https://khronokernel.github.io/Opencore-Vanilla-Desktop-Guide/).
