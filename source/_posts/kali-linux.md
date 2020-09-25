---
title: Windows引导kali Linux实现双系统（U盘安装）
date: 2018-07-28
categories: 操作系统
tags: ["kali Linux","Linux","双系统"]
icon: fa-linux
keywords: windows kill 双系统,linu win 双系统
---

### 概要
<!-- toc -->

----


<iframe class="if_video" frameborder="0" width="100%" height="640"  src="https://v.qq.com/iframe/player.html?vid=k0564u9t6e9&tiny=0&auto=0" allowfullscreen style=""></iframe>

### 先看我
1. 安装前建议看一下图文教程,up主也看了此教程才出的视频。
2. 适用于传统的BIOS引导MBR分区表，不支持UEFI引导GPT分区表。
<strong style="color:red">注意：</strong>


1. 想安装Linux你必须能够熟练安装windows各版本，如果不能那么就不要折腾了，免得到时候电脑GG了。装机有风险，请备份好你的数据。
2. 教程更正内容安装kali前Windows下操作 `桌面——>右击此电脑——>属性——>高级系统设置——>高级——启动和故障恢复——>设置` 按图中所示操作，完成确认。
![kali_01](https://s1.ax1x.com/2018/07/29/PaweVe.png "01")
---
### 工具
- 8gb U盘（自行购买）
- kali linux镜像
	https://www.kali.org/downloads/
- Universal USB Installer（linux镜像刻录U盘工具）
	https://universal-usb-installer.en.softonic.com/
- 分区助手（选择性下载）
	http://www.disktool.cn/
- 分区神器（DiskGenius）
	http://www.diskgenius.cn/
- 引导工具（EasyBCD）
	http://neosmart.net/EasyBCD/
---
### 视频详情
> 图文教程引用

  http://blog.sina.com.cn/s/blog_8c8d4e710102wggl.html
<strong style="color:red">图文教程内容更正</strong>
1. 不要使用软碟通制作，无法启动
2. 引导写入最后高级设置驱动器设置里先设置为boot看能否启动如果不能可以设置为c\
---
### 卸载方法


直接用分区神器删除Linux分区，重新分区可以格式为其它分区格式然后用引导工具删除Linux引导

---
### BGM
> BGM引用

- 与你最后的夏天
	http://music.163.com/#/m/song?id=315061&userid=446083135
- なんでもないや 没什么大不了的（Cover：Radwimps） 
	http://music.163.com/#/m/song?id=450795499&userid=446083135



