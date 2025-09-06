---
title: pdf图片互转工具
published: 2025-09-07
description: pdf图片互转
image: ""
tags: [linux]
category: 工具
draft: false
---

## pdf转图片

安装：

```bash
sudo pacman -S imagemagick
```

ImageMagick 需要 `Ghostscript (`gs`) `来渲染 PDF

安装 Ghostscript:

```bash
sudo pacman -S ghostscript
```

```bash
gs --version
```



转换 PDF → PNG：

```bash
magick -density 300 input.pdf -background white -alpha remove output.png

```

`-density 300`: 分辨率

`-background white`: 背景

`-alpha remove`: 去掉透明

`output.png`: 文件格式，会以output-1.png,output-2.png...输出

`input.pdf`: 输入的pdf文件

## 修复pdf

`qpdf` 修复 PDF

```bash
sudo pacman -S qpdf
```

执行修复：

```bash
qpdf --linearize input.pdf fixed.pdf
```

## 图片转pdf

```bash
magick *.png output.pdf
```

