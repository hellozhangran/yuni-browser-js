# 与你浏览器脚本

这是「与你科技」在开发的聊天新软件「与你 App」，我们有一个面向前端技术达人的「与你浏览器」功能，能实现一键保存网络资源，包括微博，抖音，快手，Instagram等，然后在电脑访问，或直接发给微信QQ上的朋友。

这是一个强大的功能，通过强大的JavaScript实现，在「与你浏览器」中打开的网址可以注入开发者脚本，这些脚本可以优化页面阅读，也可以获取页面背后真实的原图和视频，一键保存到「与你相册」。「与你相册」是一个跨设备跨平台的原图相册，里面的图片视频可以调用系统分享到任意App，也可以在电脑上访问「https://photos.uneed.com」访问下载。

使用示例：<br>
1）打开微博正文，然后选「更多……」「复制链接」。<br>
2）打开「与你」，自动弹出「是否使用与你浏览器」，点确定。<br>
3）点底部「批量保存到与你」，将会保存原图（不是缩略图）到「与你相册」。<br>
4）保存到「与你相册」后，可以通过网页版访问下载，或分享到其它App。<br>

![介绍](intro.png)

## 目的

在`与你App`中使用`与你浏览器`打开网页，通过注入相应的css和js，达到优化网页的排版和样式，提供下载资源到`与你相册`的功能。

## 原理

在`与你App`中使用`与你浏览器`打开任意网址时，客户端程序会自动向页面注入一个脚本（即`sites/inject.js`），这个脚本作用如下：

1. 分析域名，如：uneed.com
2. 注入css: cdn.uneed.com/browser/uneed.com/style.css
3. 注入 js: cdn.uneed.com/browser/uneed.com/script.js

## 如何参与开发

[参与开发](contributing.md)


## 相关下载

* 与你App：https://uneed.com



