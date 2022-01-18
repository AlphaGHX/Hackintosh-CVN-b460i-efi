## 更新日志

* 2022/1/19 OC版本改为RELEASE版本，同时解决了睡眠唤醒问题。
* 2022/1/6 更新了部分kext，支持Monterey。
* 2021/11/10 OC更新至0.7.5，更新了部分kext。
* 2021/7/18 OC更新至0.7.0，已经完全定制了USB，现在在macOS11.3+中也能使用USB3的速率。
* 2021/4/6 OC更新至0.6.8，更新了部分kext。
* 2021/3/3 OC更新至0.6.7，更新了部分kext。
* 2021/2/9 修复USB3接口只能用USB2的速率。
* 2021/2/5 OC更新至0.6.6，修复CPU睿频（我的i5 10400最高功率能跑到85W，全核心睿频到4GHZ）。

## 使用前

* 基于opencore 0.7.5
* 支持到macOS Monterey 12.1
* 支持七彩虹CVN-b460i
* 支持Intel 10代CPU，UHD 630 GPU，免驱卡可用。
* 安装完成后，请下载Hackintool，运行并生成序列号等信息，最后在config中更改，重点是下面三个。
![68747470733a2f2f692e6c6f6c692e6e65742f323032312f30372f31382f77686f3242344a71766b694f366e452e706e67.png](https://i.loli.net/2021/07/18/nydmeVr9BMOXFNv.png)
* 黑苹果不稳定，重要文件勤做备份！！！

## BIOS设置

* 开启XMP内存超频（可选）
* 高级模式>电源管理配置>USB键盘鼠标唤醒>开（如果你想使用鼠标键盘唤醒）

## 安装教程
* 下载镜像与烧录镜像[黑果小兵](http://blog.daliansky.net)，对镜像自带EFI没要求，因为EFI本来就有。
* 使用DiskGenius读取烧录好的U盘，替换掉自带的EFI。
* 启动项选U盘。
* 先抹掉磁盘，格式化为APFS，然后安装，不出意外就没问题了。
* 如果出现下图情况，很可能你插的是USB3，请使用USB2接口安装。经测试BigSur和Catalina都能正常安装，如果不行请更换不同版本的固件。
<img src="https://support.apple.com/library/content/dam/edam/applecare/images/en_US/macos/Big-Sur/macos-big-sur-startup-screen-prohibitory-sign.jpg" width="70%">

## 目前正常功能

* WIFI正常（Intel AX200）
* 蓝牙正常
* 有线正常
* HDMI & DP正常（主板上尽量只使用DP，HDMI有些问题，如果有解决方案，欢迎联系我。）
* USB3正常
![截屏2021-07-18 下午1.08.05.png](https://i.loli.net/2021/07/18/dSLTXrFA6nYlWc3.png)
* 核显硬件加速正常
![截屏2021-07-18 上午1.17.58.png](https://i.loli.net/2021/07/18/UpZ2BxgiAmwWIuz.png)
* 睡眠正常

## 目前问题功能

* 隔空投递不正常，可以使用免驱卡解决。

## 附图

![截屏2022-01-06 下午10.46.26.png](https://s2.loli.net/2022/01/06/4dnVRYKHUrXO78B.png)
![截屏2022-01-06 下午10.48.35.png](https://s2.loli.net/2022/01/06/N18klaRgvEQ6xt4.png)

## 排错

* 若出现问题，请开-v截图然后找我[Alpha的Telegram](https://t.me/Alpha_TL)，虽然我也基本玩不明白黑苹果，但是还是会尝试帮你解决。
<img width="979" alt="2FE88917-4440-481F-B19F-3EF17A1B7917" src="https://user-images.githubusercontent.com/61853980/110348750-efa01080-806c-11eb-8151-240bacb02abe.png">

## 感谢

* 最好的入门教程：[OpenCore Install Guide](https://dortania.github.io/OpenCore-Install-Guide/)
* 中文教程：[Xjn的博客](https://blog.xjn819.com/post/opencore-guide.html)
* 中文文档 & kexts集合下载：[OpenCore中文文档](https://oc.skk.moe/)
* 镜像下载 & 中文教程：[黑果小兵](http://blog.daliansky.net)
* 全网的黑苹果前辈
