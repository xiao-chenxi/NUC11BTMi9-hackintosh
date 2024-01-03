> ⚠️一台近乎完美黑果

# sperhmjj NUC9I7QNX OpenCore

> 我喜欢 Mac 操作系统，并且愿意为其折腾数月……

## 电脑配置

- 处理器：Intel® Core™ i7-9750H 处理器（6 核，12 MB 高速缓存，2.6 GHz 至 4.50 GHz）
- 网络： 内置Intel `i210`（下） 内置Intel `i219-LM`（上）
- 无线网络/蓝牙：Broadcom `BCM94360CS2`🔧 + 内置 Intel`AX200`
- 音频：内置`Realtek ALC256`
- 显卡：蓝宝石脉冲`RX 6600`4GB ITX + 内置 Intel `UHD Graphics 630`2048 MB
- 霹雳口：内置英特尔`JHL7540`
- 内存：
- 主硬盘：
- 第二硬盘：

## 更新日志

- 11-2-2023
  - 更新 `OpenCore` `v0.9.5`
  - 支持 `Sonama` 安装使用
  - 适配 `BCM94360CS2`
- 11-1-2023
  - 第一次提交

## bios设置

- BIOS 版本：`QXCFL579`
- 首先，恢复默认BIOS配置：`F9 - Optimal Defaults`

### 配置

- Advanced
  - USB > `Legacy USB Support: Enabled`
- Security
  - Security Features > `Intel Platform Trust Technology: Unchecked`
  - Security Features > `Intel Software Guard Extension (SGX): Disabled`
  - Security Features > `Thunderbold Security Level: Legacy mode`
- Boot
  - Secure Boot > `Secure Boot: Disabled`
  - boot Priority > `Fast Boot: Unchecked`
  - boot Priority > `Network Boot: Disabled`
  - boot Priority > `Ethernet1 Boot: Unchecked`
  - boot Priority > `Ethernet2 Boot: Unchecked`

## 安装

## 硬件

- [x] GPU加速：内置`Intel UHD 630`
- [x] GPU 加速：（`RX 570`开箱即用）
- [x] 以太网⚡
- [x] 音频（前面板耳机）
- [x] 音频（后面板耳机）
- [x] USB A 端口
- [x] SD卡插槽
- [x] NVMe固态硬盘
- [x] 无线网络⚡
- [x] 蓝牙⚡
- [x] USB C 端口
- [x] Airpods Pro（电池电量/降噪模式开关）
- [x] CPU 电源管理（使用 Intel Power Gadget 测试）

## 软件

- [x] 安装程序、应用程序商店、应用程序更新
- [x] 直接从 Apple 更新 MacOS
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
