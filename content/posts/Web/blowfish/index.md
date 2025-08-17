+++
date =2025-06-18
draft = false
categories = ['Web']
tags = ['blowfish']
title = 'Tips about blowfish'
description = '安装 Blowfish 的小 tips '
+++

# Tips about blowfish

## 背景与封面图片

如果想给文章加上封面和背景，然后两张图片分开的话，需要:
在你的文章同一目录下，将背景图片 命名为 `background.png`，封面图片命名为 `feature.png`。

## gtihub action

用 github action 构建 github pages 只需要将 theme/blowfish 下 .github 文件复制出来即可，但是原文件直接上传可能会引起错误，要把文件复制出来后，把 test.yml 和 pages.yml 删除，就不会遇到错误。