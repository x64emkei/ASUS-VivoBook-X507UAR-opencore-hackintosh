# ASUS VivoBook 15 X507UAR OpenCore EFI

## Specifications
- **Model**: ASUS VivoBook 15 – X507UA-BR385T (X507UAR)
- **Processor**: Intel Core i3-8130U (KabyLake-R)
- **Graphics**: Intel UHD Graphics 630
- **Display**: CMN15E6 (N156BGA-E3 1366x768)
- **Audio**: Realtek ALC256
- **WiFi/Bluetooth**: Intel Dual-Band Wireless AC8265
- **BIOS**: Latest version: 305

## Features
- OpenCore version: **1.0.3**
- Configured using KabyLake (7th-gen) using OpCore-Simplify, ProperTree and OC Sanity Check.
- **Audio**: 3.5mm combo jack working (layout-id=56).
- **Battery**: Proper battery detection.
- **Display**: May experience color-banding due to the panel (TN) itself. 
- **WiFi/Bluetooth**: Intel AC8265 supported (Magic Devices compatible).
- **HDMI**: HDMI output works.
- **Boot Chime**: Plays the macOS boot chime.

### Apple-Specific Features
- SMBIOS: **MacBookPro15,2** (13-inch, 2018, Four Thunderbolt 3 Ports).
- **iServices**: Fully working.

### Note
- **Microphone**: Functionality is not yet tested.
- Before using this EFI, run [GenSMBIOS](https://github.com/corpnewt/GenSMBIOS) to generate unique serials.  
  The `Generic` section in the config is left blank to avoid serial number conflicts.

---
**Disclaimer**: This EFI is tailored specifically for the ASUS VivoBook 15 X507UAR. Compatibility with other models is not guaranteed.
