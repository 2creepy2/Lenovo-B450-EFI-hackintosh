# Lenovo-B450-EFI-hackintosh

Old Lenovo Laptop B450 works well with Mac OS X El Capitan 10.11.6, dualboot with Windows 10 using GUID partition table (GPT) on harddrive.


| Specifications | Detail                                                  |
| ------------------- | ------------------------------------------- |
| Computer model | Lenovo B450 (20029) |
| Processor | Intel Pentium Dual-Core T4400 |
| Memory | 2x2Gb DDR2 667MHz |
| Hard Disk | Hitachi HTS545025B9A300 250Gb |
| Integrated Graphics | Nvidia Geforce G105M 256Mb |
| Monitor | Chi Mei N140B6-L02 1366x768 (14 inch) |
| Sound Card | Conexant Cx20561 ICH9 audio |
| Integrated LAN | Atheros AR8132 |
| Wireless Card | Atheros AR5006X |
| Trackpad | Synaptics SMBus Touchpad |
| SD Card Reader | Realtek USB 2.0 Cardreader (RTS5159 0x0bda0159) |

Cause of limitations of CPU - only SSE3 instructions supported in Pentium Dual-Core T4400, El Capitan is maximum level of Mac OS available on this hardware.

**Used Opencore bootloader 0.8.9.**

Be sure to make legacy bootable flashdrive, because it has only Legacy BIOS, with instruction on Dortania web-site - https://dortania.github.io/OpenCore-Install-Guide/installer-guide/

Works well: everything, except of: 1) internal wi-fi (can be fixed with replacing the card), 2) brightness level keys, 3) hibernation, 4) second display via VGA.

**Please, be sure to change SMBIOS section with yours.**

### To be done in the future: 
- replace CPU to Core 2 Duo T9400; - Done! Works as it should. (Now it's possible to install Mac OS 10.13.6, but this EFI isn't suitable for this).
- flash modified BIOS with whitelist unlock; - Done!
- replace internal wifi with BCM94322MC mini PCI-E card. - Done! Works out of the box. Look BIOS Update folder for modified BIOS.
