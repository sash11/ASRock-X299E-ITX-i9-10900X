# ASRock X299E-ITX/AC with Opencore 0.9.5
<p align="center">
  <img src="Docs/AboutThisMac.png" align=center">
 </p>
 <p align="center">
  <img src="Docs/PCI.jpg" align=center">
 </p>
 <p align="center">
  <img src="Docs/USB.jpg" align=center">
 </p>
 <p align="center">
  <img src="Docs/Peripherals.jpg" align=center">
 </p>

## Specs
| **Component** | **Model** |
| ------------- | --------- |
| CPU | i9-10900X 10 cores and 20 threads @3.7GHz |
| RAM | 3x16GB 266MHz DDR4 SO-DIMM Crucial CT16G4SFRA266 |
| Audio Chipset | Realtek ALC S1220. Works with Layout-id 7 |
| dGPU | Sapphire AMD Radeon RX6900XT. Works OOB |
| WiFi & Bluetooth | Fenvi BCM94360NG. Works OOB |
| OS Disk | 2TB WD SN850X |
| macOS | Ventura 13.5.2/OpenCore 0.9.5

## BIOS
- Press F2 or Del to enter the BIOS. Use latest available bios for the system 2.20B
- Multi Core Envancement Disabled
- SATA Mode AHCI
- XHCI Hand-Off Enabled
- For more detailed settings download folder BIOS-Screenshots

## Installation instructions
- Copy both EFI and NVRAM folders onto the bootable USB stick and later onto the HDD once system is up and running.
- Adjust your config according to your GPU. I am using a "natively" supported GPU with no WEG kext.
- Generate your own SMBIOS obviously. The one in the config now is just a sample for installation purposes only. Do not use it in your system.
- Follow instruction to emulate NVRAM by running a command Launchd.command from OpenCore release Utilities folder and LogoutHook subfolder https://dortania.github.io/OpenCore-Post-Install/misc/nvram.html