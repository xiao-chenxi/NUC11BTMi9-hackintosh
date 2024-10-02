> NUC11BTMi9-hackintosh
## For NUC11th generation -NUC11BTMi7/i9,Support installation MacOS Sequoia


## Computer Configuration

- processor：Intel® Core™ i9-11900KB Processor (24M Cache, up to 4.90 GHz)
- network：Intel® Ethernet Controller i225-LM
- Wireless network/Bluetooth：Intel® Wi-Fi 6E AX210
- Audio：USB Audio
- graphics card：AMD Radeon RX 6900 XT
- Thunderbolt：2x Thunderbolt™ 4
- Memory：Crucial DDR4 16G 3200MHz*2
- harddisk1：BIWIN NV7400 2T
- harddisk2：WD SN550 2T
- harddisk3：KIOXIA RC20 1T
- harddisk4：KIOXIA RC20 1T
  
## Change log

- 10-2-2024
  - Third submission
  - renew `OpenCore` `v1.0.1`
  - support `Sequoia 15.0` Install and use
  - Supports Sequoia 15.0 WI-FI and Bluetooth, the driver has been added, you only need to use OpenCore-Legacy-Patcher to patch the network card。https://github.com/dortania/OpenCore-Legacy-Patcher
  - `Sonama 14.4-14.X` please download the `NUC11BTMi9-hackintosh-Sonama-V1.2.zip`
  - `sonoma 14.4-14.X` will no longer be maintained

- 3-20-2024
  - Second submission
  - renew `OpenCore` `v0.9.9`
  - Added XHCI-unsupported.kext for USB support for sonoma 14.4：`Kelnel > Add > XHCI-unsupported.kext ：true`
  - Updated AirportItlwm.kext for WI-FI support for sonoma 14.4
  - Only Sonama 14.4 or later versions are supported



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
  - Advanced > Video > `Internal Graphics: Auto`
- Security
  - Security Features > `Intel VT for Directed I/O(VT-d)：Disabled`
- Boot
  - Secure Boot > `Secure Boot: Disabled`
  - boot Priority > `Fast Boot: Unchecked`

## hardware

- ❌  GPU acceleration：`Intel UHD Graphics 750`Unable to drive⚠️（Disable it in BIOS）
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
- ✅ Updating MacOS directly from Apple
- ✅ APFS, SSD pruning
- ✅ iMessage, iCloud, Siri, iTunes, other services
- ✅ Metal, GPU accelerated applications：**AMD Radeon RX 6900 XT**
- ✅ time Machine
- ✅ sleep mode
- ✅ Shut down/sleep/wake up

## Known issues⚠️
- The processor model of the About This Machine page cannot be changed and cannot be processed at the moment.
- boot-args > wegnoigpu does not currently work,UHD750 needs to be turned off, otherwise the display will not light up when waking up from sleep.(Advanced > Video > `Primary Display: PEG Slot / Internal Graphics: Auto`)

## Hardware not tested⚠️

- Thunderbolt 4 port
- Secure boot (with high security)

## Display of results
![截屏2024-10-02 21 21 22](https://github.com/user-attachments/assets/e4ff67f8-270f-421c-a645-8e535332bd3d)
![截屏2024-10-02 21 23 03](https://github.com/user-attachments/assets/62a03929-965c-4065-9c10-a4cef145d5d6)
![xx3](https://github.com/xiao-chenxi/NUC11BTMi9-hackintosh/assets/63736726/799cfacb-788d-439b-9e5e-b6121bd0fa14)
![xx4](https://github.com/xiao-chenxi/NUC11BTMi9-hackintosh/assets/63736726/854a959f-b337-44d7-bae5-2feb61cf616c)
![xx5](https://github.com/xiao-chenxi/NUC11BTMi9-hackintosh/assets/63736726/fb5ac0c0-bc91-48cd-871d-4d628f77e8bf)
