# NUC11BTMi9-hackintool
For NUC11th generation Beast Canyon-NUC11BTMi7/i9, MacOS sonoma

NUC11BTMi7/i9 OpenCore

电脑配置

processor：Intel® Core™ i9-11900KB Processor (24M Cache, up to 4.90 GHz)

network：Intel i225

Wireless network/Bluetooth：IntelAX210

Audio：USB Audio

graphics card：AMD Radeon RX 6900 XT/Other driver-free graphics cards

Thunderbolt 4：Not tested

Memory：Crucial DDR4 16G 3200MHz*2

harddisk1：KIOXIA RC20

harddisk2：KIOXIA RC20



Change log

1-3-2024

first submission

bios settings

BIOS Version：DBTGL579

Restore BIOS settings：F9 - Optimal Defaults

Configuration

Advanced

PCIE Resizable BAR Support: Disabled（Very important）

Video > Primary Display: PEG Slot

Security

Security Features > Intel VT for Directed I/O(VT-d)

Boot

Secure Boot > Secure Boot: Disabled

boot Priority > Fast Boot: Unchecked


安装
硬件
 GPU加速：内置Intel UHD 630
 GPU 加速：（RX 570开箱即用）
 以太网⚡
 音频（前面板耳机）
 音频（后面板耳机）
 USB A 端口
 SD卡插槽
 NVMe固态硬盘
 无线网络⚡
 蓝牙⚡
 USB C 端口
 Airpods Pro（电池电量/降噪模式开关）
 CPU 电源管理（使用 Intel Power Gadget 测试）
软件
 安装程序、应用程序商店、应用程序更新
 直接从 Apple 更新 MacOS
 APFS、SSD 修剪
 iMessage、iCloud、Siri、iTunes、其他服务
 切换、连续性、通用剪贴板：内置Intel AX200
 切换、连续性、通用剪贴板：BroadcomBCM94360CS2
 Metal、GPU 加速应用程序：内置Intel UHD 630
 金属、GPU 加速应用：Sapphire PulseRX 570
 时光机器
 睡眠模式
 关机/睡眠/唤醒
 安排启动或唤醒
 屏幕共享 (VNC)
 屏幕共享唤醒
🔧 添加 Broadcom BCM94360CS2wifi 卡
这个想法是将 wifi 卡插入 M.2 插槽，并在新卡上使用内置 wifi 卡天线。天线的硬件问题：内置电缆为 MMCX 公头和BCM94360CS2MHF4 (IPEX-4) 母头。让它运行的最简单方法是获取天线

所需硬件
博通无线BCM94360CS2网卡
BCM94360CS2至 M.2 Key-M 适配器
天线
BIOS设置
为了防止出现任何问题，您应该禁用内置 wifi：

Advanced
Onboard Devices > WLAN: uncheck
Onboard Devices > Bluetooth: uncheck
未测试硬件
音频（麦克风、Toslink）
DP 音频
视频编码器/解码器硬件
多个显示器
雷电3端口
安全启动（具有高安全性）
