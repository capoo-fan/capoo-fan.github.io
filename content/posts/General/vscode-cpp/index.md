+++
date =2025-08-03
draft = false
categories = ['General','Vscode']
tags = ['Vscode','C/Cpp']
title = 'Vscode配置教程'
description = '配置在Vscode的C/Cpp运行环境'
+++

# Vscode 配置教程

## 下载 vscode 

[vscode官方网址](https://code.visualstudio.com/Download)

![img](img/download.png) 注意这里建议全部勾选，以后会方便很多。

## 插件安装

在左边栏的方块中就是插件市场，直接搜索下载就可以。

- Chinese (Simplified) (简体中文) 
- Tokyo Night
- C/C++ Compile Run
- C/C++
- Better C++ Syntax
- Error Lens

## 配置编译运行调试环境

### mingw-w64下载

[下载网址](https://sourceforge.net/projects/mingw-w64/files/Toolchains%20targetting%20Win64/Personal%20Builds/mingw-builds/8.1.0/threads-posix/seh/)

注意选择下方的 x86_64-8.1.0-release-posix-seh-rt_v6-rev0.7z 链接进行下载

![img](img/mingw.png)
如果下载速度过慢，可以点击页面的 "problem downloading?" 链接，选择不同的链接来更换下载源，速度会有不同。

### 配置环境变量

在下载的目录(可以放到C/D盘)下找到 `mingw64/bin` 目录，复制其路径。

- 在 Windows 搜索框中搜索 “环境变量”，然后选择 “编辑系统环境变量”。

- 在弹出的 “系统属性” 窗口中，点击 “环境变量(N)...” 按钮。

- 在下方的 “系统变量(S)” 区域，找到并双击名为 Path 的变量。

- 在 “编辑环境变量” 窗口中，点击 “新建”，然后将你的编译器路径 ("C:\Users\ *你的用户名* \x86_64-8.1.0-release-posix-seh-rt_v6-rev0\mingw64\bin") 粘贴进去。

- 一路点击 “确定” 保存所有设置。

- 'Win+R' 打开运行窗口，输入 `cmd` 并回车，在输入框输入 `g++ --version` 检查是否安装成功。
- 
- 如果显示版本信息(有一大段输出)，则表示安装成功。

### 编译运行

