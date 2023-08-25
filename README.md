 Build your hackintosh with opencore, Hackintosh EFI information for TUF-GAMING-B660M-PLUS-WIFI-D4 and i5-12490F
 #
 [If you want to use CLOVER, please click here](https://github.com/dawalishi0821/Hackintosh-TUF-GAMING-B660M-PLUS-WIFI-D4-i5-12490F/tree/CLOVER)

[中文版README](https://github.com/dawalishi0821/Hackintosh-TUF-GAMING-B660M-PLUS-WIFI-D4-12490f/blob/main/README-zh-Hans.md)

I am a Chinese student, and my English is not very good, so I may have many grammatical errors when writing English readme. I hope you can forgive my English level

Share a nearly perfect homemade EFI，the project is used to boot Hackintosh

Author's QQ account：3083512851(Green hand in the group/Call me Comrade Vladimir）

#
Configuration

Accessories |  Description | Work or not | Be careful
----|----|----|---
CPU | Intel Core i5-12490F |✅|/
Motherboard | ASUS TUF GAMING B660M-PLUS WIFI D4 |✅|/
GPU | YingTong RX6800XT |✅|/
RAM | KINGBANK 3200MHz 16GB*2 |✅|/
SSD | WD sn770 1TB |✅|/
HDD | Seagate SkyHawk 4TB  |✅|/
Sound Card | RealtekALC897 |✅|/
Ethernet | Realtek8125Ethernet 2.5Gb |✅|/
WNIC | Intel Wi-Fi 6 AX201 With BT 5.2 |✅|❗

![img](https://raw.githubusercontent.com/dawalishi0821/Hackintosh-TUF-GAMING-B660M-PLUS-WIFI-D4-i5-12490F/main/关于本机.png)
#
*  Working Condition

     *  BigSur and Monterey Ventura Sonoma works normally.Catalina  seems to have some small problem
#
Detailed content
*  1.CPU

     *  The CPU works normally on High Sierra+ and has been counterfeited for 8 generations.

     *  [CPU Turbo Boost](https://github.com/acidanthera/CPUFriend)has been customized and [Geekbench5](https://www.geekbench.com)runs normally，If the CPU model is different,[please customize it again](https://www.bilibili.com/video/BV143411F7aJ/?share_source=copy_web&vd_source=89eb3ac3d3a5704fbe370f14fbc338ef)

*  2.Motherboard

     *  Motherboard works normally,USB ports have been customized，Sleep function normal,Support USB wake-up

     *  Use usbport.kext that is closer to native usb,If the usb port does not work properly,please customize it again,[Customize USB tutorial](https://www.bilibili.com/video/BV1m3411b7JP/?share_source=copy_web&vd_source=89eb3ac3d3a5704fbe370f14fbc338ef)

     *  If sleep is abnormal,try to use [ssdttime](https://github.com/corpnewt/SSDTTime)to extract again

*  3.GPU

     *  GPU works normally(The graphics card no-load fan may not work under macOS

     *  [Injection of DP information can solve the problem](https://www.bilibili.com/video/BV1WT411A72F/?share_source=copy_web&vd_source=89eb3ac3d3a5704fbe370f14fbc338ef)

*  4.RAM

     *  Memory works normally,and overclocking works normally

*  5.SSD&HDD

     *  The hard disk perfectly supports Tirm and works normally,Avoid [hard disks not supported by macos](https://hpglw.com/cdc6109c.html)

*  6.Sound Card

     *  [Sound Card](https://github.com/acidanthera/AppleALC) works normally,and the drive has been simplified,Counterfeit layout-id 66 successed（Suspected all IDs can be）

*  7.Ethernet

     *  [Ethernet](https://www.insanelymac.com/forum/files/file/1004-lucyrtl8125ethernet/)works normally,Network speed is normal

*  8.Wi-Fi

     *  Wi-Fi works normally,support 802.11ax(beat),Handoff works normally，in BigSur can work in both directions,Monterey in only one directions,Neither AirDrop nor Sidecar works,AirDrop can only discover devices.

     *  [Airportitlwm driver and itlwm driver warehouse](https://github.com/OpenIntelWireless/itlwm/releases)

     *   Itlwm is recommended with [Heliport](https://github.com/OpenIntelWireless/HeliPort)

*   9.Bluetooth

     *   [Bluetooth](https://github.com/OpenIntelWireless/IntelBluetoothFirmware)works normally,support BT5.2,There is no problem connecting the wireless headset and audio,

     *  Thin drive added,Bluetooth switch has added maximum and minimum kernel number,Switch drive can automatically change loading.

#
Start Hackintosh
*  BIOSsetup Basic operation：

     *  1.Turn off csm

     *  2.change satamode to ahci

*  Other operation：

     *  https://apple.sqlsec.com/3-准备工作/3-1/

     *  This motherboard has no cfglock option. Unlock cfg reference[Tutorials for 乌龙蜜桃来一打](https://www.bilibili.com/video/BV1LV4y1N7jF/?share_source=copy_web&vd_source=89eb3ac3d3a5704fbe370f14fbc338ef)

*   Installation method

     *  https://apple.sqlsec.com
And more tutorials at https://www.bilibili.com

*   More subsequent optimization

     *  https://apple.sqlsec.com/6-实用姿势/6-1/

*  Encountered a problem

     *  1.Can ask the author 

     *  2.You can join the QQ group to communicate  Hackintosh and ask questions to the group friends

     *  3.You can contact enthusiastic bloggers who are active in bilibili

     *  4.Submit issues
#
Thanks for

[Acidanthera](https://github.com/acidanthera) Developed [OpenCore](https://github.com/acidanthera/OpenCorePkg) and [Other drives](https://github.com/orgs/acidanthera/repositories) and [Official Tutorial](https://dortania.github.io/OpenCore-Install-Guide/)

[Apple](https://www.apple.com) Developed [macOS](https://www.apple.com/macos/)

[zxystd](https://github.com/zxystd) Developed [itlwm](https://github.com/OpenIntelWireless/itlwm)

[Bat.bat](https://github.com/williambj1) Developed [IntelBluetoothFirmware](https://github.com/OpenIntelWireless/IntelBluetoothFirmware) and [HeliPort](https://github.com/OpenIntelWireless/HeliPort)

[Mieze](https://www.insanelymac.com/forum/profile/983225-mieze/) Developed [LucyRTL8125Ethernet](https://www.insanelymac.com/forum/files/file/1004-lucyrtl8125ethernet/)

[corpnewt](https://github.com/corpnewt) Developed [SSDTTime](https://github.com/corpnewt/SSDTTime)

[USBToolBox](https://github.com/USBToolBox) Developed [USBToolBox](https://github.com/USBToolBox)

[benbaker76 etc.](https://github.com/benbaker76) Developed [Hackintool](https://github.com/benbaker76/Hackintool)

[ic005k](https://github.com/ic005k) Developed [OCAuxiliaryTools](https://github.com/ic005k/OCAuxiliaryTools)

[国光酱](https://space.bilibili.com/112842166?spm_id_from=333.337.0.0)'s [Hackintosh  Tutorial](https://apple.sqlsec.com)

[乌龙蜜桃来一打](https://space.bilibili.com/244390800?spm_id_from=333.337.0.0)'s  [Cfg unlocking tutorial](https://www.bilibili.com/video/BV1LV4y1N7jF/?spm_id_from=333.999.0.0&vd_source=1b694a12fb9af6d07f612a9c284e1867) and Careful teaching

[老八带你玩黑果](https://space.bilibili.com/504306154?spm_id_from=333.337.search-card.all.click) 的 [CPU Turbo Boost Customization Tutorial](https://www.bilibili.com/video/BV143411F7aJ/?spm_id_from=333.999.0.0&vd_source=1b694a12fb9af6d07f612a9c284e1867) and Careful teaching,accompany

[大头蔡](https://space.bilibili.com/16323318)'s [Usb customization tutorial](https://www.bilibili.com/video/BV1m3411b7JP/?spm_id_from=333.337.search-card.all.click&vd_source=1b694a12fb9af6d07f612a9c284e1867)

[胡杨](https://space.bilibili.com/597075281?spm_id_from=333.337.0.0)'s Careful teaching

[白给大老师](https://space.bilibili.com/1314835603?spm_id_from=333.337.0.0)'s Careful teaching

[win1010525](https://github.com/win1010525)'s Careful teaching

[黄少](https://space.bilibili.com/621086526?spm_id_from=333.337.0.0)'s Careful teaching

[16](https://github.com/shilu0718)‘s accompany

老六大老师's accompany

七 Donated RX5600XT

之一 Donated RX570

lch Donated GT730
