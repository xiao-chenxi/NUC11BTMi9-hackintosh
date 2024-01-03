> NUC11BTMi9-hackintool
For NUC11th generation Beast Canyon-NUC11BTMi7/i9, MacOS sonoma

NUC11BTMi7/i9 OpenCore

## Computer Configuration

- processor：Intel® Core™ i9-11900KB Processor (24M Cache, up to 4.90 GHz)
- network：Intel i225
- Wireless network/Bluetooth：IntelAX210
- Audio：USB Audio
- graphics card：AMD Radeon RX 6900 XT/Other driver-free graphics cards
- Thunderbolt 4
- Memory：Crucial DDR4 16G 3200MHz*2
- harddisk1：KIOXIA RC20
- harddisk2：KIOXIA RC20
  
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

## 安装

## 硬件

- [x] GPU acceleration：内置`Intel UHD Graphics 910`
- [x] GPU acceleration：（`AMD Radeon RX 6900 XT/Other driver-free graphics cards`Ready out of the box）
- [x] Ethernet⚡
- [x] Audio
- [x] USB A port
- [x] SD card slot
- [x] NVMe SSD
- [x] wireless network⚡
- [x] Bluetooth⚡
- [x] CPU power management (tested with Intel Power Gadget)
software

## software

- [x] Installers, app stores, app updates
- [x] Updating MacOS directly from Apple （requires a few steps`not selected：Config-Kernel-BlueToolFixup.kext / IntelBluetoothFirmware.kext / IntelBTPatcher.kext]` ； `Add Config-NVRAM-7C436110-AB2A-4BBB-A880-FE41995C9F82-boot-args-revpatch=sbvmm`）
- [x] APFS, SSD pruning
- [x] iMessage, iCloud, Siri, iTunes, other services
- [x] 金属、GPU 加速应用：**Sapphire Pulse`RX 570`**
- [x] time Machine
- [x] sleep mode
- [x] Shut down/sleep/wake up
- [x] Schedule startup or wakeup

## Hardware not tested

- Audio (microphone, Toslink)
- DP audio
- multiple monitors
- Thunderbolt 4 port
- Secure boot (with high security)
