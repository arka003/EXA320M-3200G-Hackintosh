# EXA320M-3200G Hackintosh (OC v1.0.0)

This repository contains the EFI folder and configuration files needed to set up a Hackintosh on a system with an ASUS EX-A320M GAMING motherboard and a Ryzen 3 3200G APU.

## System Specifications

- **Motherboard**: ASUS EX-A320M GAMING
- **Processor**: AMD Ryzen 3 3200G
- **Graphics**: AMD Radeon Vega 8
- **RAM**: 16GB 2666Mhz
- **Storage**: Crucial SSD
- **Bluetooth**: TP-Link UB400
- **Ethernet**: Realtek RTL8111
- **Keyboard & Mouse**: Microsoft Wired Keyboard 500 & Dell MS116 USB Optical Mouse

## Current Status

1. **What works?**
   - Bluetooth
   - Sleep
   - Audio
   - iServices (refer https://dortania.github.io/OpenCore-Post-Install/universal/iservices.html#fixing-imessage-and-other-services-with-opencore)
   - iGPU Acceleration (thanks to NootedRed)
   
2. **What doesn't work?**
   - DRM
   - Advanced OpenGL apps may cause graphical glitches and/or GPU hangs
   - One USB3.2 port at the back of the motherboard (I've disabled it due to macOS's 15 port USB limit)

**NOTE:** Remove NootedRed from Kexts and update `config.plist` for the first boot until completely installed, add it after successful installation for GPU acceleration.

**It is recommended to map USB ports again using USBMap from corpnewt even if you're using a slightly different build**
