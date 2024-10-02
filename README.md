> NUC11BTMi9-hackintosh
## For NUC11th generation -NUC11BTMi7/i9,Support installation MacOS sonoma


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
  
- 3-20-2024
  - Second submission
  - renew `OpenCore` `v0.9.9`
  - Added XHCI-unsupported.kext for USB support for sonoma 14.4：`Kelnel > Add > XHCI-unsupported.kext ：true`
  - Updated AirportItlwm.kext for WI-FI support for sonoma 14.4
  - Only Sonama 14.4 or later versions are supported
  - 
- 10-2-2024
  - Third submission
  - renew `OpenCore` `v1.0.1`
  - support `Sequoia 15.0` Install and use
  - `Sonama 14.4-14.X` please download the V1.1 version，The final upgrade has been done, sonoma 14.4-14.X will no longer be maintained
  
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
- ✅ Updating MacOS directly from Apple
- ✅ APFS, SSD pruning
- ✅ iMessage, iCloud, Siri, iTunes, other services
- ✅ Metal, GPU accelerated applications：**AMD Radeon RX 6900 XT**
- ✅ time Machine
- ✅ sleep mode
- ✅ Shut down/sleep/wake up

## Known issues⚠️
- The processor model of the About This Machine page cannot be changed and cannot be processed at the moment.
- boot-args > wegnoigpu does not currently work,UHD750 needs to be turned off, otherwise the display will not light up when waking up from sleep.

## Hardware not tested⚠️

- SD card slot
- Thunderbolt 4 port
- Secure boot (with high security)

## Display of results
![xx1](https://github.com/xl120022/NUC11BTMi9-hackintool/assets/63736726/1ab9d1cf-0850-468a-b0de-d1c3641e7951)
![xx2](https://github.com/xl120022/NUC11BTMi9-hackintool/assets/63736726/2d3c095c-36dc-46d8-beae-49cb2b816aed)
![xx3](https://github.com/xiao-chenxi/NUC11BTMi9-hackintosh/assets/63736726/799cfacb-788d-439b-9e5e-b6121bd0fa14)
![xx4](https://github.com/xiao-chenxi/NUC11BTMi9-hackintosh/assets/63736726/854a959f-b337-44d7-bae5-2feb61cf616c)
![xx5](https://github.com/xiao-chenxi/NUC11BTMi9-hackintosh/assets/63736726/fb5ac0c0-bc91-48cd-871d-4d628f77e8bf)
