---
title: 如何使用 ClashX 向手机提供代理 -- 写给杜总
date: 2023-02-2 22:50:00 -500
category: [proxy]
tags: [clashX]

---

## 在电脑端进行的操作

打开clash，选择设置

![dashboard](/image/dashboard.png)

1、选择允许来自局域网的连接 （allow connect from lan）
   记住混合端口 ，这里是7890

2、获取电脑的IP地址

- 在mac 系统下，option+click dock栏里的Wi-Fi按钮
- 在windows 下， 点击允许局域网连接 附近的信息按钮，也可获得 IP地址

![ipAddress](/image/ipAddress.png)

## 在手机端进行的操作

![WifiSetting](/image/IMG_1334.PNG)

- 打开 Wi-Fi， 点击所使用Wi-Fi的，这里为 Tp-Link BA3A，的i按钮，

![HttpsProxy](/image/IMG_1335.PNG)

- 滑倒底部，选择构建代理

![ProxyConfiguration](/image/IMG_1336.PNG)

- 按照在电脑端记下的信息填写。
- 注意： 电脑需要和手机连接同一个Wi-Fi

## 原理

- 手机上传下载的 https相关数据会经过 电脑的clash作为中转进行加密，从而达到代理的目的。

- 在Wi-Fi配置中，使用的是 https代理，而有的 app，例如 youtube，需要 udp。
