---
title: OBS简单入门
date: 2018-07-30 17:05:24
categories: 常用工具
tags: ["OBS","电脑录屏软件","开源软件","免费"]
keywords: obs屏幕录制,免费无水印电脑录屏软件
---


## 概要
<!-- toc -->

----

## 录制屏幕
#### 录制整个屏幕
1. 运行OBS右击——>添加【添加场景】

![添加场景](https://res.cloudinary.com/miku52/image/upload/v1532939413/OBS/01.gif "添加场景")

2. 添加源右击——>添加——>选则【显示器获取】

![获取来源](https://res.cloudinary.com/miku52/image/upload/v1532939414/OBS/02.gif "获取整个屏幕")

3. 点击【预览串流】，看能否获取到屏幕如果可以点击【开始录制视频】，录制的视频默认保存在`C:\用户\当前用户\视频文件夹下\`

![开始录制](https://res.cloudinary.com/miku52/image/upload/v1532939414/OBS/03.gif "开始录制")

#### 录制指定区域
1. 右击添加——>选择【显示器获取】——>「区域」——>勾选区域——>选择区域——>拖动到要录制的区域并调节到适合的大小调节好后按回车——>确认，把整个屏幕项去掉勾选，预览一下串流确认能看到画面后开始录制。

![指定区域录制](https://res.cloudinary.com/miku52/image/upload/v1532939414/OBS/04.gif "指定区域录制")

精确控制选择指定区域，在区域菜单项中可以更改一下参数实现精确控制大小和位置。

![选区参数控制](https://res.cloudinary.com/miku52/image/upload/v1532939414/OBS/05.png "选区参数控制")

## 录制视频参数配置
### 存储路径&视频格式
- 设定——>设定——>广播设定——>档案路径——>浏览（新的存储路径）——>保存类型两种格式可选（默认flv/mp4）——>文件名`[$T]`是一个参数表示文件名按时间来命名,其它这种参数如下图——>选择——>确认。

![路径&格式](https://res.cloudinary.com/miku52/image/upload/v1532939414/OBS/06.gif "路径&格式")

![文件命名参数](https://res.cloudinary.com/miku52/image/upload/v1532939414/OBS/07.png "文件命名参数")

### 视频帧数配置/FPS

- 设定——>设定——>影像——>FPS（取值范围1~60）——>确定。

![FPS](https://res.cloudinary.com/miku52/image/upload/v1532939414/OBS/08.gif "FPS")
## 快捷键的使用

打开设定面板【快捷键】项，我们可以从这里设置开始录制和暂停录制的热键。

![快捷面板](https://res.cloudinary.com/miku52/image/upload/v1532939414/OBS/09.png "快捷面板")

---
## 共享资源

最后分享一下我正在使用的OBS官方绿色版内置一些常用插件64bit

[获取OBS64bit](https://www.lanzous.com/i1izyoh
 "获取资源")