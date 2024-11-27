# Hackintosh Build Guide: Intel i5-10600k & MSI Z490 GAMING EDGE WIFI


![macOS About Screen](https://cdn.discordapp.com/attachments/1213894175221878784/1311277451820662846/Screenshot_2024-11-27_at_2.04.44_AM.png?ex=674845ca&is=6746f44a&hm=45813ea7af47c99c5c0e30143163fd0b375fa0e61d3413f021ba7248b49bae77&)


## Introduction

This document provides a detailed guide for installing macOS **Sequoia (15)** on a Hackintosh system featuring an Intel i5-10600k CPU and an MSI Z490 GAMING EDGE WIFI motherboard. The configuration files provided here are optimized for this specific setup and more than likely only work for Sequoia.

## Compatibility

- **OpenCore Version**: 1.0.2
- **Supported CPUs**: Intel Comet Lake i5/i7/i9 (10th Gen)
- **Motherboard Chipset**: Z490
- **Intel UHD 630 iGPU** with Metal, OpenCL, and OpenGL support
- **Tested macOS Versions**: Sequoia (macOS 15)

### System Configuration

This setup is based on the following components:

| Component            | Description                                             |
|----------------------|---------------------------------------------------------|
| **Motherboard**       | MSI Z490 GAMING EDGE WIFI                               |
| **Processor**         | Intel i5-10600K (Comet Lake)                            |
| **Integrated GPU**    | Intel UHD 630                                           |
| **Dedicated GPU**     | NVIDIA RTX 3060 Ti (disabled in BIOS)                   |
| **RAM**               | 2x Corsair Vengeance DDR4 16GB 3200MHz                  |
| **Audio**             | Realtek ALC1200 (AppleALC.kext, layout-id=11)           |
| **Ethernet**          | Realtek RTL8125B-CG 2.5Gbps                             |
| **Wi-Fi**             | Intel AX201                                             |
| **Storage**           | SAMSUNG EVO 1TB SSD                                     |
| **Display Output**    | 1x HDMI, 1920x1080 Monitor                              |

## Key Features Working

- ✅ **USB Ports**: Fully functional, including front panel and all rear ports
- ✅ **Keyboard**: PS/2 keyboard support works out-of-the-box
- ✅ **Display**: HDMI output is recognized and displays at 1080p
- ✅ **Audio**: Audio is working via AppleALC.kext with layout-id=11
- ✅ **Ethernet**: Realtek 1Gbit RTL8125B-CG Ethernet is functional
- ✅ **Graphics**: Metal, OpenCL, and OpenGL support for Intel UHD 630 iGPU
- ✅ **Sleep/Wake**: Sleep and wake functions work correctly without issues
- ✅ **WiFi**: Working with OCLP patch on Sequoia
- ✅ **Bluetooth**: Working with bluetooth kexts from OpenIntelWireless
  
## Known Issues

- ❌ **Display on Wake**: Sometimes the HDMI monitor doesn’t come back on after sleep; requires a hdmi unplug

## Acknowledgements

I would like to express my gratitude to [ARGAMX](https://github.com/ARGAMX) for their fantastic EFI configuration, which significantly helped resolve issues like GPU compatibility and display refresh rate problems. Their work provided a solid foundation that made my setup process much smoother. You can find their original repository [here](https://github.com/ARGAMX/Hackintosh-Intel-i9-10850k-MSI-Z490-GAMING-EDGE-WIFI).

---

Happy Hackintoshing!
