# CLOVER-B660-12490F-RX6800XT
一个B660-12490F-RX6800XT的CLOVER引导
分享一个近乎完美的自制CLOVER EFI，项目用于引导Hackintosh

 ![img](https://raw.githubusercontent.com/dawalishi0821/Hackintosh-TUF-GAMING-B660M-PLUS-WIFI-D4-i5-12490F/main/关于本机.png)
#
支持HighSierra～Sonoma
---
作者qq：3083512851（群菜鸡/叫我，弗拉基米尔同志）

配置

配件 | 描述 | 是否工作 | 注意
----|----|----|---
CPU | Intel Core i5-12490F |✅|/
主板 | 华硕TUF GAMING B660M-PLUS WIFI D4 |✅|/
显卡 | 盈通花嫁RX6800XT |✅|/
内存 | 金百达普条3200 16GB*2 |✅|/
硬盘1 | 西数sn770 1TB |✅|/
硬盘2 | 希捷酷鹰4TB  |✅|/
声卡 | 板载RealtekALC897 |✅|/
网卡1 | 板载Realtek8125Ethernet的2.5Gb网卡 |✅|/
网卡2 | AX201 支持Wi-Fi6和蓝牙5.2 |✅|❗

#
详细内容
*  1.CPU

     *  CPU工作正常，已经仿冒8代。

     *  [CPU睿频](https://github.com/acidanthera/CPUFriend)已经定制[geekbench5](https://www.geekbench.com)跑分正常，如果cpu型号不同请重新定制，[定制cpu睿频教程](https://www.bilibili.com/video/BV143411F7aJ/?share_source=copy_web&vd_source=89eb3ac3d3a5704fbe370f14fbc338ef)

*  2.主板

     *  主板工作正常，usb端口均已经定制，睡眠正常，支持usb唤醒

     *  使用更接近原生usb的usbport.kext如果usb端口工作不正常请重新定制，[定制USB教程](https://www.bilibili.com/video/BV1m3411b7JP/?share_source=copy_web&vd_source=89eb3ac3d3a5704fbe370f14fbc338ef)

     *  如果睡眠等不正常尝试用[ssdttime](https://github.com/corpnewt/SSDTTime)重新提取

*  3.显卡

     *  显卡工作正常（macOS下可能遇到显卡风扇无负载不转，

     *  [注入dp信息可以解决](https://www.bilibili.com/video/BV1WT411A72F/?share_source=copy_web&vd_source=89eb3ac3d3a5704fbe370f14fbc338ef)

*  4.内存

     *  内存工作正常，超频工作正常

*  5.硬盘

     *  硬盘完美tirm，工作正常，避免[macos不支持的硬盘](https://hpglw.com/cdc6109c.html)

*  6.声卡

     *  [声卡](https://github.com/acidanthera/AppleALC)工作正常，驱动已经精简，仿冒layout-id 66成功（疑似所有id均可）

*   7.以太网

     *  [以太网](https://www.insanelymac.com/forum/files/file/1004-lucyrtl8125ethernet/)工作正常，网速正常

*   8.无线网卡Wi-Fi

     *  无线网卡Wi-Fi工作正常，支持802.11ax(beat)，接力投屏正常，macos11可以双向，macos12以上单向，隔空投送随航均不能工作.

     *  [Airportitlwm驱动和itlwm驱动仓库](https://github.com/OpenIntelWireless/itlwm/releases)

     *  itlwm建议搭配[Heliport](https://github.com/OpenIntelWireless/HeliPort)

*  9.无线网卡蓝牙

     *  [无线网卡蓝牙](https://github.com/OpenIntelWireless/IntelBluetoothFirmware)工作正常，支持蓝牙5.2，连无线耳机和音响没有问题.

#
开始Hackintosh
*  bios设置最基本：
     *  1.关掉csm

     *  2.satamode改成ahci即可

*  深入：

     *  https://apple.sqlsec.com/3-准备工作/3-1/

     *  这个主板没有cfglock选项，解锁cfg参考[乌龙蜜桃来一打教程](https://www.bilibili.com/video/BV1LV4y1N7jF/?share_source=copy_web&vd_source=89eb3ac3d3a5704fbe370f14fbc338ef)

*   安装方法

     * https://apple.sqlsec.com

     *  以及更多b站教程

*   更多后续优化

     *  https://apple.sqlsec.com/6-实用姿势/6-1/

*   遇到了问题

     *  1.可以联系作者

     *  2.可以加入黑苹果交流的QQ群，向群友提问

     *  3.可以联系B站上热心up

     *  4.提issues

#
鸣谢

[CloverHackyColor](https://github.com/CloverHackyColor)开发的[CloverBootloader](https://github.com/CloverHackyColor/CloverBootloader)

[Acidanthera](https://github.com/acidanthera) 开发的 [常用驱动](https://github.com/orgs/acidanthera/repositories)

[Apple](https://www.apple.com) 开发的 [macOS](https://www.apple.com/macos/)

[zxystd](https://github.com/zxystd) 开发的 [itlwm](https://github.com/OpenIntelWireless/itlwm)

[Bat.bat](https://github.com/williambj1) 开发的 [IntelBluetoothFirmware](https://github.com/OpenIntelWireless/IntelBluetoothFirmware) 和 [HeliPort](https://github.com/OpenIntelWireless/HeliPort)

[Mieze](https://www.insanelymac.com/forum/profile/983225-mieze/) 开发的 [LucyRTL8125Ethernet](https://www.insanelymac.com/forum/files/file/1004-lucyrtl8125ethernet/)

[corpnewt](https://github.com/corpnewt) 开发的 [SSDTTime](https://github.com/corpnewt/SSDTTime)

[USBToolBox](https://github.com/USBToolBox) 开发的 [USBToolBox](https://github.com/USBToolBox)

[benbaker76等人](https://github.com/benbaker76) 开发的 [Hackintool](https://github.com/benbaker76/Hackintool)

[老八带你玩黑果](https://space.bilibili.com/504306154?spm_id_from=333.337.search-card.all.click) 的 [cpu睿频定制教程](https://www.bilibili.com/video/BV143411F7aJ/?spm_id_from=333.999.0.0&vd_source=1b694a12fb9af6d07f612a9c284e1867) 和 细心教导陪伴

[大头蔡](https://space.bilibili.com/16323318) 的 [usb定制教程](https://www.bilibili.com/video/BV1m3411b7JP/?spm_id_from=333.337.search-card.all.click&vd_source=1b694a12fb9af6d07f612a9c284e1867)

[黄少](https://space.bilibili.com/621086526?spm_id_from=333.337.0.0) 的 细心教导
