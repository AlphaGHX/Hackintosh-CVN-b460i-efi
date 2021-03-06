## 更新日志

* 2021/3/3 OC更新至0.6.7，更新了部分kext
* 2021/2/9 修复USB3接口只能用USB2的速率
* 2021/2/5 OC更新至0.6.6，修复CPU睿频（我的i5 10400最高功率能跑到85W，全核心睿频到4GHZ）

## 使用前

* 基于opencore 0.6.7
* 支持macOS BigSur 11.2.2
* 支持七彩虹CVN-b460i
* 支持Intel10代CPU，UHD 630 GPU，独显未做支持！
* 安装完成后，请下载Hackintool，运行并生成序列号等信息，最后在config中更改。

## BIOS设置

* 开启XMP内存超频
* 高级模式->高级->CSM设置->关闭CMS
* 高级模式->引导->关闭BIOS写保护
* 值得注意的是：在安装的时侯，可能出现下图所示的禁止图标，如果出现，请等待5分钟左右。本人第一次安装的时侯也出现了此问题，等了一段时间（具体忘记了）就成功进入安装界面了，之后也不会出现此问题。
<img src="https://support.apple.com/library/content/dam/edam/applecare/images/en_US/macos/Big-Sur/macos-big-sur-startup-screen-prohibitory-sign.jpg" width="70%">

## 目前正常功能

* WIFI正常（Intel AX200）
* 蓝牙正常
* 有线正常
* HDMI & DP正常
* USB3正常

## 目前问题功能

* 睡眠唤醒后系统某些应用卡死，请在设置里设置只关闭屏幕，因为是台式机，对电源管理没那么敏感，暂时不做修复，听说是关于主板ME设置的事情，如果有大佬知道问题所在欢迎提issues，感谢～
* 隔空投递不正常，这个可能要等AirportItlwm的更新，我们现在能不用免驱卡正常上网已经是不容易了！

## 附图

![截屏2021-02-06 上午11.57.46.png](https://i.loli.net/2021/02/06/k1BS3OVqmHDbg4z.png)
![截屏2021-02-06 下午12.15.25.png](https://i.loli.net/2021/02/06/aKJEW3IYgU6btQu.png)

## 感谢

* 最好的入门教程：[OpenCore Install Guide](https://dortania.github.io/OpenCore-Install-Guide/)
* 中文教程：[Xjn的博客](https://blog.xjn819.com/post/opencore-guide.html)
* 中文文档 & kexts集合下载：[OpenCore中文文档](https://oc.skk.moe/)
* 镜像下载 & 中文教程：[黑果小兵](http://blog.daliansky.net)
* 全网的黑苹果前辈
