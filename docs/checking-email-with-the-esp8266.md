# 使用 ESP8266 检查电子邮件

> 原文：<https://hackaday.com/2014/11/03/checking-email-with-the-esp8266/>

非常缓慢地，每个人最喜欢的 WiFi 适配器正在进入互联网项目。[jimeer01]创造了一种设备，可以从他的收件箱[中读取最新电子邮件的主题和发件人行，并使用 ESP8266 WiFi 芯片](http://www.instructables.com/id/You-Have-Mail-Gets-the-Latest-email-and-displays-t/?ALLSTEPS)将其显示在 LCD 上。

【jimeer】正在使用[by pic](http://www.bypic.co.uk/)写入 LCD 并通过 ESP8266 模块查询收件箱。ByPic 是围绕 BV_Basic 固件构建的板，将 Pic 微控制器填充到 Arduino 外形中，并为其提供基本解释器。因为这个板不像 Arduino 那样“编译和刷新”,所以它非常适合动态更改 WiFi 配置和 IMAP 服务器凭证。

该设备在收件箱中抓取最新的电子邮件，并在显示屏上显示日期、发件人和主题。滚动这些行后，PIC 点击 ESP8266 再次查询服务器，获取最新的电子邮件，并再次重复整个过程，所有这些都不需要将设备连接到计算机。下面视频。

[https://www.youtube.com/embed/fPpyCoBJOzM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/fPpyCoBJOzM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)