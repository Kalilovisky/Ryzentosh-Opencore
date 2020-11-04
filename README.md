# OpenCore EFI for AMD Ryzen Hackintosh

**macOS version**: 10.15.7

**OpenCore version**: 0.6.3

## Hardware
| **Component** | **Model** |
| ------------- | --------- |
| CPU | AMD Ryzen 5 2600 @ 3.4GHz |
| Motherboard | ASUS Prime B450M-Gaming/BR |
| RAM | 16GB (2 x 8GB) @ 2133MHz (from AliExpress) |
| Audio Chipset | ALC-887 |
| GPU | ASRock RX 560 4GB |
| WiFi & Bluetooth | Fenvi FV-HB1200 (from AliExpress) |
| OS Disk (SSD) | Samsung 860 Evo 500GB (from AliExpress) |

## Compatible macOS versions
 - High Sierra (10.13.x)
 - Mojave (10.14.x)
 - Catalina (10.15.x)
 - Big Sur (???)
 
 ## Issues
 - 3.5mm jack microphone (only USB/Bluetooth microphones)
 - Sidecar
 
 ## How to use
  1. Make your USB installer with [**this guide**](https://dortania.github.io/OpenCore-Install-Guide/installer-guide/)
  2. Clone the repository and paste "BOOT" and "OC" directories into your's pendrive "EFI" folder
  3. Download [**GenSMBIOS**](https://github.com/corpnewt/GenSMBIOS) to generate unique SMBIOS information. Run it and select **Generate SMBIOS**, as the model select **iMacPro1,1**.
  4. Open config.plist with [**ProperTree**](https://github.com/corpnewt/ProperTree) and go to PlatformInfo > Generic. Set MLB (Board Serial), SystemSerialNumber (Serial) and SystemUUID (SmUUID) to generated values. Change ROM to your network card's MAC address without the `:` character. [**How to get MAC Address?**](https://www.wikihow.com/Find-the-MAC-Address-of-Your-Computer)
  5. Boot it! 
  
  ## Cedits and links:
  * [AMD OS X](https://forum.amd-osx.com/)
  * [OpenCore Desktop Guide](https://github.com/dortania/OpenCore-Desktop-Guide)
