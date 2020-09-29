---
title: Nodejs安装指南
date: 2020-09-29 09:55:16
categories: Node
tags: ["nvm","node","详细安装"]
icon: fa-pencil-square-o
keywords: nodejs安装教程,nodejs详细安装,node配置淘宝镜像
---

## 概要
<!-- toc -->


通过node官网提供的.msi文件安装不利于版本控制。本文章讲解一下NVM安装nodejs。
[![0AmTHS.png](https://s1.ax1x.com/2020/09/27/0AmTHS.png)](https:imgchr.com/i/0AmTHS)

**安装注意事项;**
在安装NVM之前，您需要卸载任何现有版本的node.js。同时删除可能保留的任何现有nodejs安装目录（例如，“C：\ Program Files \ nodejs”）。NVM生成的符号链接不会覆盖现有的（甚至是空的）安装目录。

您还应该删除现有的npm安装位置（例如“C：\ Users <user> \ AppData \ Roaming \ npm”）


## nvm下载安装和配置

### 下载nvm

1. 打开GitHub
[![0AmInf.md.png](https://s1.ax1x.com/2020/09/27/0AmInf.md.png)](https://imgchr.com/i/0AmInf)
[![0AmHAg.md.png](https://s1.ax1x.com/2020/09/27/0AmHAg.md.png)](https://imgchr.com/i/0AmHAg)

2. 搜索nvm-windows,并打开该项目。
[![0AmoB8.md.png](https://s1.ax1x.com/2020/09/27/0AmoB8.md.png)](https://imgchr.com/i/0AmoB8)
3. 往下滚动网页，选择Releases 
[![0Am4jP.png](https://s1.ax1x.com/2020/09/27/0Am4jP.png)](https://imgchr.com/i/0Am4jP)
4. 点击nvm-setup.zip下载。
[![0AmbNQ.md.png](https://s1.ax1x.com/2020/09/27/0AmbNQ.md.png)](https://imgchr.com/i/0AmbNQ)

### 安装nvm

1. 解压压缩包。
2. 双击nvm-setup.exe运行安装程序。
[![0Amqhj.png](https://s1.ax1x.com/2020/09/27/0Amqhj.png)](https://imgchr.com/i/0Amqhj)
3. 按以下图片操作。
- 同意协议并下一步
[![0AmO9s.png](https://s1.ax1x.com/2020/09/27/0AmO9s.png)](https://imgchr.com/i/0AmO9s)
- 指定NVM安装路径并下一步
[![0AmX3n.png](https://s1.ax1x.com/2020/09/27/0AmX3n.png)](https://imgchr.com/i/0AmX3n)
- 指定Nodejs安装路径并下一步
[![0Amjcq.png](https://s1.ax1x.com/2020/09/27/0Amjcq.png)](https://imgchr.com/i/0Amjcq)

[![0Amjcq.png](https://s1.ax1x.com/2020/09/27/0Amjcq.png)](https://imgchr.com/i/0Amjcq)

[![0AmzuV.png](https://s1.ax1x.com/2020/09/27/0AmzuV.png)](https://imgchr.com/i/0AmzuV)

[![0AnSBT.png](https://s1.ax1x.com/2020/09/27/0AnSBT.png)](https://imgchr.com/i/0AnSBT)
  

### 验证nvm安装

1. <kbd>Win</kbd>+<kbd>R</kbd> 打开运行。
2. 输入cmd
[![0AnCEF.png](https://s1.ax1x.com/2020/09/27/0AnCEF.png)](https://imgchr.com/i/0AnCEF)
3. 输入`nvm version` 如下图则证明安装成功。
[![0AnPN4.png](https://s1.ax1x.com/2020/09/27/0AnPN4.png)](https://imgchr.com/i/0AnPN4)

### 添加淘宝镜像源

> 添加镜像源提高下载速度。
1. 用文本编辑器打开settings.txt文件(路径`nvm安装路径\settings.txt`)
2. 在文件后添加以下内容。
```
node_mirror:https://npm.taobao.org/mirrors/node/
npm_mirror: https://npm.taobao.org/mirrors/npm/
```
3. 保存settings.txt
[![0AK2h4.png](https://s1.ax1x.com/2020/09/27/0AK2h4.png)](https://imgchr.com/i/0AK2h4)

## nvm使用
### 下载nodejs
0. 打开cmd
1. 列出服务器上所有node版本
```bash
nvm ls available
```
[![0Ani4J.md.png](https://s1.ax1x.com/2020/09/27/0Ani4J.md.png)](https://imgchr.com/i/0Ani4J)
2. 安装指定版本的node。
```bash
nvm install 版本号
# 如安装12.18.4版本
nvm install 12.18.4
```
[![0AnkC9.png](https://s1.ax1x.com/2020/09/27/0AnkC9.png)](https://imgchr.com/i/0AnkC9)
3. 执行`nvm ls`查看已经安装的nodejs版本。
[![0AnA3R.png](https://s1.ax1x.com/2020/09/27/0AnA3R.png)](https://imgchr.com/i/0AnA3R)

### 启用nodejs
1. 启用上步骤安装的nodejs 使用以下命令直接切换到该版本的nodejs即可启用。至于为什么要这样做，答虽然安装了nodejs但是我们并没有告诉NVM要使用那个版本的nodejs。
```bash
nvm use 已安装nodejs版本号 
# 如使用12.18.4
nvm use 12.18.4
```
[![0AnEg1.png](https://s1.ax1x.com/2020/09/27/0AnEg1.png)](https://imgchr.com/i/0AnEg1)
2. 输入`node -v` 查看当前的node版本。
[![0AnVjx.png](https://s1.ax1x.com/2020/09/27/0AnVjx.png)](https://imgchr.com/i/0AnVjx)
3. 输入`npm -v` 查看npm版本。
[![0AnMUe.png](https://s1.ax1x.com/2020/09/27/0AnMUe.png)](https://imgchr.com/i/0AnMUe)
4. 以上命令如果都正确执行则表示nodejs已经成功安装，可以正常使用了。

### 多版本nodejs切换
> 提示；使用nvm install 命令可以安装更多版本node。

1. 查看本地安装的nodejs版本，前面有`*`代表当前使用的node版本。
```bash
nvm ls
```
[![0A1KVP.png](https://s1.ax1x.com/2020/09/27/0A1KVP.png)](https://imgchr.com/i/0A1KVP)

2. 切换到另一个版本node。
```bash
nvm use 版本号
# 如切换到14.12.0
nvm use 14.12.0
```

3. 再次查看版本已经成功切换到了14版本。
[![0AGnbR.png](https://s1.ax1x.com/2020/09/27/0AGnbR.png)](https://imgchr.com/i/0AGnbR)


### 卸载nodejs
```bash
nvm uninstall 版本号。
# 如卸载10.22.1
nvm uninstall 10.22.1
```
[![0AnnHO.png](https://s1.ax1x.com/2020/09/27/0AnnHO.png)](https://imgchr.com/i/0AnnHO)


## npm配置淘宝镜像
> 提高下载速度
1. 查看当前npm源,结果如果是`https://registry.npmjs.org` 证明我们使用的npm内置的源。
```bash
npm get registry
```
[![0Z86F1.png](https://s1.ax1x.com/2020/09/29/0Z86F1.png)](https://imgchr.com/i/0Z86F1)

**临时换源;**
只有当前使用才生效，下次启动npm会自动恢复默认内置源。
```bash
npm --registry https://registry.npm.taobao.org install express
```
**持久换源;**

```bash
npm config set registry https://registry.npm.taobao.org
```
[![0Z8cJx.png](https://s1.ax1x.com/2020/09/29/0Z8cJx.png)](https://imgchr.com/i/0Z8cJx)

配置后可通过下面方式来验证是否成功
```bash
npm get registry
```

[![0Z8gW6.png](https://s1.ax1x.com/2020/09/29/0Z8gW6.png)](https://imgchr.com/i/0Z8gW6)
如果查看发现源改变则证明换源成功，赶紧试试安装一个包吧





## CNPM
> 如果你感觉NPM配置了淘宝镜像还是慢可以尝试以下CNPM

**全局安装cnpm;**

```bash
npm install -g cnpm --registry=https://registry.npm.taobao.org
```
**验证安装；**

```bash
cnpm -v
```
[![0AnKED.md.png](https://s1.ax1x.com/2020/09/27/0AnKED.md.png)](https://imgchr.com/i/0AnKED)

以后再次安装包时，把npm换为cnpm即可。

## 如何卸载nvm
直接向QQ那样到控制面板卸载NVM for Windows

## 附录

### nvm常用命令
```bash
nvm ls # 查看安装的node版本
nvm list # 查看安装的node版本

# node安装
nvm ls available # 列出服务器上所有node版本
nvm install 版本号 [位数] # 选择要安装的版本如是32位系统要后加32，表示下载32位node


# 版本切换 
nvm use version # 要切换的版本
nvm use 8.1 # 切换到8.1系列的最高版本
nvm use node # 切换到最新版本
nvm uninstall 0.0.0 # 卸载指定版本的node

```
### npm常用命令
**参数简写对照**
- `--save`相当于`-s`
- `--global`相当于`-g`
- `--save-dev`相当于`-d`
- `--save-optional`相当于`-o`
- `--save-exact`相当于`-e`
需要注意的是，我们在安装第三方包的时候通常会用到-s、-g、-d后缀，其他的很少用到。

```bash
npm uninstall -g 包名 # 卸载指定的全局包
# 安装第三方包
npm install xxx  # 安装模块如不指定版本号，默认会安装最新的版本，安装但不写入package.json
npm install xxx 0.0.1  # 安装指定版本的模块
npm install --save xxx # 安装并把模块的版本信息保存到dependencies（生产环境依赖）中，即你的package.json文件的dependencies字段中
npm install --global xxx    # 全局安装指定的包。
npm install --save-dev xxx # 安装并把模块版本信息保存到devDependencies（开发环境依赖）中，即你的package.json文件的devDependencies字段中
npm install --save-optional xxx # 安装并把模块安装到optionalDependencies（可选环境依赖）中，即你的package.json文件的optionalDependencies字段中
npm install --save-exact xxx # 精确的安装指定版本的模块，dependencies字段里每个模块版本号前面的^会取消掉
# 其他npm命令行
npm init # 在当前目录生成一个package.json文件，这个文件中会记录一些关于项目的信息，比如：项目的作者，git地址，入口文件、命令设置、项目名称和版本号等等，一般情况下这个文件是必须要有的，方便后续的项目添加和其他开发人员的使用。
npm list 或 npm ll 或 npm la 或 npm ls  # 列出已安装模块， ll 、 ls 、 la 三个命令意思都一样，但是列表的展示方式不一样
npm show xxx  # 显示模块详情
npm update  # 升级当前目录下的项目的所有模块
npm update xxx  # 升级当前目录下的项目的指定模块
npm update -g xxx  # 升级全局安装的指定模块
npm uninstall xxx  # 删除指定的模块
npm list --depth=0 # 仅获取顶层的软件包
npm list minimist # 程序最小依赖
npm view pkg versions    # 列出包的所有版本

```
