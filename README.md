# ASUS VivoBook 15 X507UAR OpenCore EFI
![Spec](https://github.com/user-attachments/assets/beb898e7-81b0-4f6c-ba03-ac8be70e784b)

## Specifications

| Component | Details |
|---------|--------|
| **Model** | ASUS VivoBook 15 – X507UA-BR385T (X507UAR) |
| **Processor** | Intel Core i3-8130U (Kaby Lake-R) |
| **Graphics** | Intel UHD Graphics 630 |
| **Display** | CMN15E6 (N156BGA-E3, 1366×768) |
| **Audio** | Realtek ALC256 |
| **WiFi / Bluetooth** | Intel Dual-Band Wireless AC 8265 |
| **BIOS** | Latest version: 305 |

---

## Features
- OpenCore version: **1.0.3**
- Configured using KabyLake (7th-gen) following the Dortania OpenCore Guide, OpCore-Simplify, ProperTree, and OC Sanity Check  
  → [View config results](https://sanitychecker.ocutils.me/results/ens9hhr8bcn6w506)
- **Audio**: Fully functional internal + combo jack I/O (`layout-id=66`)
- **Battery**: Proper battery detection
- **Display**: May experience color banding due to TN panel limitations
- **WiFi / Bluetooth**: Intel AC8265 supported (Apple Magic Devices compatible)
- **HDMI**: HDMI output works
- **Boot Chime**: macOS boot chime enabled

### Apple-Specific Features
- **SMBIOS**: `MacBookPro15,2` (13-inch, 2018, Four Thunderbolt 3 Ports)
- **iServices**: Fully working (iCloud, FaceTime, Messages, Mail, etc.)

### Notes
- **Microphone**: ~~Not tested~~ → Now working (`layout-id=66`)
- Before using this EFI, run [GenSMBIOS](https://github.com/corpnewt/GenSMBIOS) to generate unique serial numbers  
  - `PlatformInfo → Generic` is left blank intentionally
- Download official drivers & BIOS from ASUS:  
  [ASUS X507UAR Support Page](https://www.asus.com/laptops/for-home/everyday-use/asus-x507/helpdesk_download?model2Name=ASUS-Laptop-X507UA)
- When using [OC Sanity Checker](https://sanitychecker.ocutils.me), select:
  - **CPU**: (7th Gen) Kaby Lake  
  - **OpenCore version**: v1.0.3  
  > Although marketed as 8th-Gen, the i3-8130U is Kaby Lake-R and must be configured as Kaby Lake
- May require **Airport** workaround on **macOS Sequoia**

---

## Disclaimer
This EFI is tailored specifically for the **ASUS VivoBook 15 X507UAR**.  
Compatibility with other variants (UB / MA / LA / UF / F507LA) is **not guaranteed**.  
EFI contents may change depending on hardware revisions.

⚠️ **Warning**  
Use of **OpenCore Simplify** and **OpenCore Legacy Patcher (OCLP)** must be done **with caution**.  
Improper use or applying configurations without fine-tuning for your specific hardware **may result in boot failure, system instability, or data loss**.  

Always review, adjust, and validate settings based on your **own system configuration**.  
**You have been warned.**

---

**Codename:** ONYX COPPER II
