# TUF-GAMING-B660M-PLUS-WIFI-D4-12490f
TUF GAMING B660M-PLUS WIFI D4+12490f
分享一个近乎完美的自制efi
作者qq：3083512851（群菜鸡/叫我，弗拉基米尔同志）

配置：
==
cpu inteli5-12490f

主板 华硕TUF GAMING B660M-PLUS WIFI D4

显卡 蓝宝石rx5600xt

内存 英睿达普条3200 8GB*2

硬盘 西数sn770 1TB｜希捷酷鹰4TB
    
声卡 板载ALC897

网卡 板载Realtek8125Ethernet的2.5Gb网卡｜板载AX201 支持Wi-Fi6和蓝牙5.0

状态：
=
Macos11+均正常工作，暂不推荐使用Ventura，macos10.15疑似有小问题


1.Cpu
---
Cpu在10.15+工作正常，已经仿冒10代，如果安装10.13请仿冒8代（未测试是否正常工作，仿冒参数见官方教程

https://dortania.github.io/OpenCore-Install-Guide/

Cpu睿频已经定制geekbench5跑分正常，如果cpu型号不同请重新定制，教程

【黑苹果下CPU睿频，让黑苹果更加完美黑苹果CPU变频睿频日志，一招解决CPU频率不正确，无法变频-CPU黑苹果睿频解决卡顿现象黑果CPU变频日志睿频教程】

https://www.bilibili.com/video/BV143411F7aJ/?share_source=copy_web&vd_source=89eb3ac3d3a5704fbe370f14fbc338ef

2.主板
---
主板工作正常，usb端口均已经定制，睡眠正常，支持usb唤醒

本efi使用更接近原生usb的usbport.kext如果usb端口工作不正常请重新定制

【【黑苹果】全新的定制USB教程】 https://www.bilibili.com/video/BV1m3411b7JP/?share_source=copy_web&vd_source=89eb3ac3d3a5704fbe370f14fbc338ef

如果睡眠等不正常尝试用ssdttime重新提取

https://github.com/corpnewt/SSDTTime


3.显卡
---
显卡工作正常（macOS下可能遇到显卡风扇无负载不转，

注入dp信息可以解决，

教程【高温夏天 显卡风扇不转怎么办？双系统（windows+macOS）下给显卡降降温】 

https://www.bilibili.com/video/BV1WT411A72F/?share_source=copy_web&vd_source=89eb3ac3d3a5704fbe370f14fbc338ef


4.内存
---
内存工作正常，超频工作正常


5.硬盘
---
硬盘完美tirm，工作正常，避免macos不支持的硬盘

https://hpglw.com/cdc6109c.html


6.声卡
---
声卡工作正常，驱动已经精简，仿冒layout-id 66成功（疑似所有id均可），无
工作正常，接力正常，macos11可以双向，macos12以上单向，隔空投送随航均不能工作

https://github.com/OpenIntelWireless/itlwm/releases

https://github.com/OpenIntelWireless/HeliPort


7.无线网卡蓝牙
---
无线网卡蓝牙工作正常，已添加精简驱动，蓝牙开关已添加最大最小内核，开关驱动可以自动更换加载


bios设置
=
最基本：关掉csm，satamode改成ahci即可
深入：https://apple.sqlsec.com/3-准备工作/3-1/
这个主板没有cfglock选项，解锁cfg参考乌龙蜜桃来一打教程
【【黑苹果】无法解锁的CFG LOCK | 新技能get !】 https://www.bilibili.com/video/BV1LV4y1N7jF/?share_source=copy_web&vd_source=89eb3ac3d3a5704fbe370f14fbc338ef

安装方法
=
https://apple.sqlsec.com
以及更多b站教程

更多后续优化：
=
https://apple.sqlsec.com/6-实用姿势/6-1/

遇到了问题：
=
可以联系作者
Qq上也有很多黑苹果的群可以进行交流
B站上也有很多热心up

鸣谢
=
[Acidanthera](https://github.com/acidanthera) 开发的 [OpenCore](https://github.com/acidanthera/OpenCorePkg) 和 [其他驱动](https://github.com/orgs/acidanthera/repositories) 以及 [官方教程](https://dortania.github.io/OpenCore-Install-Guide/)

[Apple](https://www.apple.com) 开发的 [macOS](https://www.apple.com/macos/)

[zxystd](https://github.com/zxystd) 开发的 [itlwm](https://github.com/OpenIntelWireless/itlwm)

[Bat.bat](https://github.com/williambj1) 开发的 [IntelBluetoothFirmware](https://github.com/OpenIntelWireless/IntelBluetoothFirmware) 和 [HeliPort](https://github.com/OpenIntelWireless/HeliPort)

[corpnewt](https://github.com/corpnewt) 开发的 [SSDTTime](https://github.com/corpnewt/SSDTTime)

[USBToolBox](https://github.com/USBToolBox) 开发的 [USBToolBox](https://github.com/USBToolBox)

[ic005k](https://github.com/ic005k) 开发的 [OCAuxiliaryTools](https://github.com/ic005k/OCAuxiliaryTools)

[国光酱](https://space.bilibili.com/112842166?spm_id_from=333.337.0.0) 的 [黑苹果教程](https://apple.sqlsec.com)

[乌龙蜜桃来一打](https://space.bilibili.com/244390800?spm_id_from=333.337.0.0)  的  [cfg解锁教程](https://www.bilibili.com/video/BV1LV4y1N7jF/?spm_id_from=333.999.0.0&vd_source=1b694a12fb9af6d07f612a9c284e1867) 和 细心教导

[老八带你玩黑果](https://space.bilibili.com/504306154?spm_id_from=333.337.search-card.all.click) 的 [cpu睿频定制教程](https://www.bilibili.com/video/BV143411F7aJ/?spm_id_from=333.999.0.0&vd_source=1b694a12fb9af6d07f612a9c284e1867) 和 细心教导陪伴

[小明和他的女朋友](https://space.bilibili.com/591453294?spm_id_from=333.337.0.0) 的 [显卡PP_PhmSoftPowerPlayTable注入修改显卡bios设置教程](https://www.bilibili.com/video/BV1WT411A72F/?spm_id_from=333.999.0.0&vd_source=1b694a12fb9af6d07f612a9c284e1867) 和 [EFI](https://github.com/Xmingbai/ASUS-TUF-GAMING-B660M-PLUS-Wi-Fi-D4-Hackintosh)（后面我自己重做了）

[大头蔡](https://space.bilibili.com/16323318) 的 [usb定制教程](https://www.bilibili.com/video/BV1m3411b7JP/?spm_id_from=333.337.search-card.all.click&vd_source=1b694a12fb9af6d07f612a9c284e1867)

[胡杨](https://space.bilibili.com/597075281?spm_id_from=333.337.0.0) 的 细心教导

[白给大老师](https://space.bilibili.com/1314835603?spm_id_from=333.337.0.0) 的 细心教导

[黄少](https://space.bilibili.com/621086526?spm_id_from=333.337.0.0) 的 细心教导

[16](https://github.com/shilu0718) 的 陪伴

老六大老师 的 陪伴

七 的 RX5600XT

之一 的 RX570
