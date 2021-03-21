# Hackintosh-Dell-OptiPlex-9020M

This is the Hackintosh EFI Folder for Dell OptiPlex 9020 Micro. The configuration settings support macOS Big Sur 11.2.3 with resolution up to 3440 x 1440. My CPU is a Mobile i7-4960HQ modified from FCBGA 1364 to LGA 1150
You will have to **generate a new serial and SmUUID** before login to your iCloud account.

## Hardware Specs
* **Barebone Chassis**: [Dell OptiPlex 9020M](https://www.dell.com/aw/business/p/optiplex-9020m-desktop/pd) with 2 DP Ports
* **CPU**: [Intel® Core™ i7-4960HQ](https://ark.intel.com/content/www/us/en/ark/products/76088/intel-core-i7-4960hq-processor-6m-cache-up-to-3-80-ghz.html)
* **iGPU**: Intel® Iris® Pro Graphics 5200
* **RAM**: 16GB DDR3L 1600 Daul Channel 
* **Wi-Fi & Bluetooth**: BCM94360CS2 with NGFF Adapter

## What Works
* CPU Turbo Boost & Thermal Throttling
* Integrated Graphics with acceleration
* monitor output at 3440 x 1440
* Integrated Audio Output/Input
* All USB Ports
* LAN & Wireless Network
* Airdrop & Airplay
* Sleep & Wakeup

## BIOS Settings
- General → Advanced Boot Options: ***uncheck***
- System Configuration → SATA Operation: ***AHCI***
- Secure Boot → Secure Boot Enable: ***Disabled***
- Virtualization Support → VT for Direct I/O: ***uncheck***

## BIOS Settings via GRUB
* Set Pre-Allocated DVMT to 128M: 
***setup_var 0x263 0x04***
* Disable CFG lock: 
***setup_var 0xD9F 0x00***