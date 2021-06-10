# Hackintosh-OC-Lenovo-ThinkCentre-M920x

## 平台配置

* 准系统：Lenovo ThinkCentre M920x
* CPU：Intel Core i5-8600T (Coffee Lake)
* iGPU：Intel UHD Graphics 630
* dGPU：AMD Radeon RX560 4GB
* 网卡：Apple BCM94360CS2
* 内存：16GB DDR4 2666MHz

## 特性

* 仿冒机型：iMac19,1（SN已去除，需自行补充）
* 系统版本：Big Sur 11.4
* 核显编解码加速正常，无显示输出，显卡FB：3E920003，VRAM：1536MB
* 独显输出正常，最高支持4屏输出（MiniDPx4）
* 内置扬声器、前置耳机、麦克风输出正常，声卡ID：17
* WiFi正常，免驱
* 蓝牙正常，支持接力，支持随航
* 睡眠正常，支持电能小憩
* USB端口正常，端口属性正确修正
* CPU电源管理正常，支持功率报告
* 支持开机音效
* 电源按钮正常，短按1S睡眠，长按>3S弹出关机对话框
* EC（SuperIO）正常，支持风扇转速报告

## 已知问题

* 无

## BIOS配置（版本：M1UKT65A）

* 恢复出厂设置：`Exit`->`OS Optimized Defaults [Enabled]`->`Load Optimal Defaults`
* 关闭VT-d：`Advanced`->`CPU Setup`->`VT-d [Disabled]`
* 关闭安全启动：`Security`->`Secure Boot`->`Secure Boot [Disabled]`
* 关闭CFG Lock：0x721 0x0

## 更新日志

### 2021-6-11

* 更换机型iMac19,1
* 去除核显输出，变更为纯加速卡

### 2021-6-8

* 更新OpenCore 0.7.0
* 更新AppleALC 1.6.1
* 更新NVMeFix 1.0.8
* 更新VirtualSMC 1.2.4
* 更新Whatevergreen 1.5.0
* 打开看门狗

### 2021-5-7

* 更新SMCSuperIO自编译版本（已合入官方主线，1.2.4发布后再替换官方版本）
* 支持风扇和电压报告

### 2021-5-6

* 更新OpenCore 0.6.9
* 更新AppleALC 1.6.0
* 更新IntelMausi 1.0.6
* 更新Lilu 1.5.3
* 更新NVMeFix 1.0.7
* 更新VirtualSMC 1.2.3

### 2021-4-30

* 去除无用的ACPI表
* 关闭Verbose模式

### 2021-4-24

* 更新OpenCore 0.6.8
* 修复HDMI接口输出
