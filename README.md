# Lenovo-B450-EFI-hackintosh

Old Lenovo Laptop B450 works well with Mac OS X El Capitan 10.11.6, dualboot with Windows 10 using GUID partition table (GPT) on harddrive.

Specs: Pentium Dual-Core T4400, Intel GM45 chipset, 2x2Gb DDR2, nVidia Geforce G105M, Atheros AR8132 LAN, Atheros AR5006X WiFi, Conexant Cx20561 ICH9 audio.

Cause of limitations of CPU - only SSE3 instructions supported in Pentium Dual-Core T4400, El Capitan is maximum level of Mac OS available on this hardware.

** Used Opencore bootloader 0.8.9.

Be sure to make legacy bootable flashdrive, because it has only Legacy BIOS, with instruction on Dortania web-site - https://dortania.github.io/OpenCore-Install-Guide/installer-guide/

Works well: everything, except of internal wi-fi, brightness level keys, hibernation.

## Please, be sure to change SMBIOS section with yours.

To be done in the future: 
- replace CPU to Core 2 Duo T9400;
- flash modified BIOS with whitelist unlock;
-  replace internal wifi with BCM94322MC mini PCI-E card.
