> NUC11BTMi9-hackintool
## For NUC11th generation -NUC11BTMi7/i9,Support installation MacOS sonoma
![xx1](https://github.com/xl120022/NUC11BTMi9-hackintool/assets/63736726/1ab9d1cf-0850-468a-b0de-d1c3641e7951)
![xx2](https://github.com/xl120022/NUC11BTMi9-hackintool/assets/63736726/2d3c095c-36dc-46d8-beae-49cb2b816aed)


## Computer Configuration

- processor：Intel® Core™ i9-11900KB Processor (24M Cache, up to 4.90 GHz)
- network：Intel® Ethernet Controller i225-LM
- Wireless network/Bluetooth：Intel® Wi-Fi 6E AX210
- Audio：USB Audio
- graphics card：AMD Radeon RX 6900 XT
- Thunderbolt：2x Thunderbolt™ 4
- Memory：Crucial DDR4 16G 3200MHz*2
- harddisk1：KIOXIA RC20 1T
- harddisk2：KIOXIA RC20 1T
  
## Change log

- 1-3-2024
  - first submission
  - renew `OpenCore` `v0.9.7`
  - support `Sonama` Install and use

## bios settings

- BIOS Version：`DBTGL579`
- Restore BIOS settings：`F9 - Optimal Defaults`

### Configuration

- Advanced
  - Advanced > `PCIE Resizable BAR Support: Disabled（Very important）`
  - Advanced > Video > `Primary Display: PEG Slot`
- Security
  - Security Features > `Intel VT for Directed I/O(VT-d)：Disabled`
- Boot
  - Secure Boot > `Secure Boot: Disabled`
  - boot Priority > `Fast Boot: Unchecked`

## hardware

- ❌  GPU acceleration：`Intel UHD Graphics 910`Unable to drive⚠️
- ✅ GPU acceleration：（`AMD Radeon RX 6900 XT/Other driver-free graphics cards`Ready out of the box）
- ✅ Ethernet
- ✅ USB Audio
- ✅ USB A port
- ✅ NVMe SSD
- ✅ wireless network
- ✅ Bluetooth
software

## software

- ✅ Installers, app stores, app updates
- ✅ Updating MacOS directly from Apple （Incremental package upgrade requires setting the following two options，Otherwise you will not be able to receive the new version，Wait for the update to complete before restoring settings）⚠️

      `not selected：Config > Kernel - BlueToolFixup.kext / IntelBluetoothFirmware.kext / IntelBTPatcher.kext`

      `Add：Config > NVRAM-7C436110-AB2A-4BBB-A880-FE41995C9F82 > boot-args - revpatch=sbvmm`
- ✅ APFS, SSD pruning
- ✅ iMessage, iCloud, Siri, iTunes, other services
- ✅ Metal, GPU accelerated applications：**AMD Radeon RX 6900 XT`**
- ✅ time Machine
- ✅ sleep mode
- ✅ Shut down/sleep/wake up

## Hardware not tested⚠️

- SD card slot
- Thunderbolt 4 port
- Secure boot (with high security)
