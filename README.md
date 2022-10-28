## 更新日志

* 2022/10/28 OC 更新至 0.8.5，更新了 kext，定制了主板显示接口，支持 Ventura。（注：本次更新时隔较长，内容较多，更新时请先使用U盘引导，确认没问题后，在移动到硬盘。同时，因为精力有限，此更新不再支持主板自带的 AX200 网卡，如果需要，请自行安装，需要 [AirportItlwm](https://github.com/OpenIntelWireless/itlwm) 和 [IntelBluetoothFirmware](https://github.com/OpenIntelWireless/IntelBluetoothFirmware)，以及移除 EFI 自带的与 Brcm 有关的 kext）
* 2022/1/19 OC 版本改为 RELEASE 版本，同时解决了[睡眠问题](#睡眠问题)。
* 2022/1/6 更新了部分 kext，支持 Monterey。
* 2021/11/10 OC 更新至 0.7.5，更新了部分 kext。
* 2021/7/18 OC 更新至 0.7.0，已经完全定制了 USB，现在在 macOS11.3+ 中也能使用 USB3 的速率。
* 2021/4/6 OC 更新至 0.6.8，更新了部分 kext。
* 2021/3/3 OC 更新至 0.6.7，更新了部分 kext。
* 2021/2/9 解决 USB3 接口只能用 USB2 的速率。
* 2021/2/5 OC 更新至 0.6.6 ，解决 CPU 睿频问题。

## 使用前

* 基于 opencore 0.8.5
* 支持 macOS Ventura
* 支持七彩虹 CVN-b460i
* 支持 Intel 10 代 CPU，UHD 630 GPU，免驱卡可用。
* 安装完成后，请下载 [OCAT](https://github.com/ic005k/OCAuxiliaryTools) 并且生成红框中的信息，并保存。
[![x4hpS1.png](https://s1.ax1x.com/2022/10/28/x4hpS1.png)](https://imgse.com/i/x4hpS1)
* 已经基本可以满足日常使用，如果不出现 macOS 或 OC 的重大更新，此 EFI 将不会更新，如果需要更新 OC 版本，可自行使用 [OCAT](https://github.com/ic005k/OCAuxiliaryTools) 进行更新。
* 黑苹果不稳定，重要文件勤做备份！！！

## BIOS 设置

* 开启XMP内存超频（可选）
* 高级模式>电源管理配置> USB 键盘鼠标唤醒>开（如果你想使用鼠标键盘唤醒）

## 安装教程
* 下载镜像与烧录镜像 [点击此处](#感谢)。
* 下载 [Releases](https://github.com/AlphaGHX/Hackintosh-CVN-b460i-efi/releases)。
* 复制到指定分区。
* 启动项选U盘。
* 抹掉磁盘，格式化为 APFS ，安装。
* 如果出现下图情况，请使用 USB2 重试。
<img src="https://support.apple.com/library/content/dam/edam/applecare/images/en_US/macos/Big-Sur/macos-big-sur-startup-screen-prohibitory-sign.jpg" width="70%">

## 功能

* WIFI正常（博通免驱卡）
* 蓝牙正常
* 有线正常
* HDMI & DP 正常（部分显示器或者线材可能导致双屏的一些问题，比较玄学。）
* 睡眠正常
* USB3 正常
![截屏2021-07-18 下午1.08.05.png](https://i.loli.net/2021/07/18/dSLTXrFA6nYlWc3.png)
* 核显硬件加速正常
![截屏2021-07-18 上午1.17.58.png](https://i.loli.net/2021/07/18/UpZ2BxgiAmwWIuz.png)

## 睡眠问题

* 可以不更新EFI，但需要更新到最新的BIOS，同时在BIOS里开启BIOS写保护。你也可以更新到最新BIOS后恢复BIOS出厂设置，默认是开启BIOS写保护的。

## 附图

[![x4hPOK.png](https://s1.ax1x.com/2022/10/28/x4hPOK.png)](https://imgse.com/i/x4hPOK)

## 排错

* 若出现问题，请开 -v 截图然后找我 [Alpha的Telegram](https://t.me/Alpha_TL)，虽然我也基本玩不明白黑苹果，但是还是会尝试帮你解决。
[![x4hkwD.png](https://s1.ax1x.com/2022/10/28/x4hkwD.png)](https://imgse.com/i/x4hkwD)

## 感谢

* 最好的入门教程：[OpenCore Install Guide](https://dortania.github.io/OpenCore-Install-Guide/)
* 中文教程：[Xjn的博客](https://blog.xjn819.com/post/opencore-guide.html)
* 中文文档 & kexts集合下载：[OpenCore中文文档](https://oc.skk.moe/)
* 镜像下载 & 中文教程：[黑果小兵](http://blog.daliansky.net)
* 镜像下载(英文)；[Dortania's Creating the USB](https://dortania.github.io/OpenCore-Install-Guide/installer-guide/)
* 全网的黑苹果前辈
