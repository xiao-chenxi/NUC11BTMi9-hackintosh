> NUC11BTMi9-hackintool
For NUC11th generation Beast Canyon-NUC11BTMi7/i9, MacOS sonoma

NUC11BTMi7/i9 OpenCore

## Computer Configuration

processor：Intel® Core™ i9-11900KB Processor (24M Cache, up to 4.90 GHz)

network：Intel i225

Wireless network/Bluetooth：IntelAX210

Audio：USB Audio

graphics card：AMD Radeon RX 6900 XT/Other driver-free graphics cards

Thunderbolt 4

Memory：Crucial DDR4 16G 3200MHz*2

harddisk1：KIOXIA RC20

harddisk2：KIOXIA RC20

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
- [x] (Updating MacOS directly from Apple [requires a few steps`not selected：Config-Kernel-BlueToolFixup.kext / IntelBluetoothFirmware.kext / IntelBTPatcher.kext]`；`Add Config-NVRAM-7C436110-AB2A-4BBB-A880-FE41995C9F82-boot-args-revpatch=sbvmm`
- [x] APFS、SSD 修剪
- [x] iMessage、iCloud、Siri、iTunes、其他服务
- [ ] 切换、连续性、通用剪贴板：**内置`Intel AX200`**
- [x] 切换、连续性、通用剪贴板：**Broadcom`BCM94360CS2`**
- [x] Metal、GPU 加速应用程序：**内置`Intel UHD 630`**
- [x] 金属、GPU 加速应用：**Sapphire Pulse`RX 570`**
- [x] 时光机器
- [x] 睡眠模式
- [x] 关机/睡眠/唤醒
- [x] 安排启动或唤醒
- [x] 屏幕共享 (VNC)
- [ ] 屏幕共享唤醒

## 🔧 添加 Broadcom `BCM94360CS2`wifi 卡

这个想法是将 wifi 卡插入 M.2 插槽，并在新卡上使用内置 wifi 卡天线。天线的硬件问题：内置电缆为 MMCX 公头和`BCM94360CS2`MHF4 (IPEX-4) 母头。让它运行的最简单方法是获取天线

### 所需硬件

- 博通无线`BCM94360CS2`网卡
- `BCM94360CS2`至 M.2 Key-M 适配器
- 天线

### BIOS设置

为了防止出现任何问题，您应该禁用内置 wifi：

- Advanced
  - Onboard Devices > `WLAN: uncheck`
  - Onboard Devices > `Bluetooth: uncheck`

## 未测试硬件

- 音频（麦克风、Toslink）
- DP 音频
- 视频编码器/解码器硬件
- 多个显示器
- 雷电3端口
- 安全启动（具有高安全性）
