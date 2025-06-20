# ASUS VivoBook 15 X507UAR OpenCore EFI
![Spec](https://github.com/user-attachments/assets/beb898e7-81b0-4f6c-ba03-ac8be70e784b)
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
- Configured using KabyLake (7th-gen) using Dortania OpenCore Guide, OpCore-Simplify, ProperTree and OC Sanity Check [see config results here](https://sanitychecker.ocutils.me/results/ens9hhr8bcn6w506).
- **Audio**: Fully functional internal+combojack I/O `layout-id=66`.
- **Battery**: Proper battery detection.
- **Display**: May experience color-banding due to the panel (TN) itself. 
- **WiFi/Bluetooth**: Intel AC8265 supported (Apple Magic Devices compatible).
- **HDMI**: HDMI output works.
- **Boot Chime**: Plays the macOS boot chime.

### Apple-Specific Features
- SMBIOS: `MacBookPro15,2` (13-inch, 2018, Four Thunderbolt 3 Ports).
- **iServices**: Fully working (iCloud, Facetime, Messages, Mail and more).

### Note
- **Microphone**: ~~Functionality is not yet tested.~~ Now working `layout-id=66`
- Before using this EFI, run [GenSMBIOS](https://github.com/corpnewt/GenSMBIOS) to generate unique serials installed at config.plist.  
  The `Generic` section in the config is left blank to avoid serial number conflicts.
- Check [here](https://www.asus.com/laptops/for-home/everyday-use/asus-x507/helpdesk_download?model2Name=ASUS-Laptop-X507UA "ASUS X507UAR Drivers and BIOS") for complete drivers for proper ACPI detection.
- When checking `config.plist` at [OC Sanity Checker](https://sanitychecker.ocutils.me)make sure to select '(7th) Kaby Lake' and the OpenCore version (in this case - v1.0.3). Since this is a Refresh CPU despite Intel marketing this as 8th-Gen processor, the CPU remains configured as KabyLake. 
- May need to use AIRPORT on SEQUOIA 

---
**Disclaimer**: This EFI is tailored specifically for the ASUS VivoBook 15 X507UAR. Compatibility with other models is not guaranteed (such as -UB/-MA/-LA/-UF/F507LA models), EFI may subject to change according to your specifications.
