# 神秘博士式的 WiFi

> 原文：<https://hackaday.com/2013/04/01/doctor-who-style-wifi/>

![wifi](img/fd5c2ba0ef1010e14f87a9c92c4c1e1a.png)

#### **剧透，亲爱的……**

如果你没有看《神秘博士》的最新一集，这里有一个情节:随机的人连接到名字奇怪的 WiFi 网络，然后在笨蛋机器人的帮助下将他们的意识上传到互联网。对于非 Whovian 人来说，这没有太多意义，但[Tony Box] [想出了一种方法，用 Linux box 和 USB WiFi 卡复制这种效果](http://blog.tonybox.net/blog/2013/03/31/doctor-who-style-wi-fi-with-sentient-captive-portal/)，正好赶上一个伟大的愚人节玩笑。

对于 SSID，reddit 上的[人决定最好的字符来自](http://www.reddit.com/r/doctorwho/comments/1bb9yy/doctor_who_7x07_the_bells_of_saint_john/c95aqba)[统一加拿大土著音节 Unicode block](http://en.wikipedia.org/wiki/Unified_Canadian_Aboriginal_Syllabics_(Unicode_block)) 。[Tony]然后设置一台带有 USB wifi 卡的笔记本电脑，并使用 hostapd 和 dnsmasq 来更改 SSID 和 DHCP 租约。nginx 提供了一个简单的网页，上面有这一集的一个短片(一个勺子头上传意识)。

真正有趣的是:[Tony]正在使用一个强制门户网站，就像你在咖啡店或酒店登录互联网时出现的网页一样。当这个恶作剧的受害者登录到大智慧的无线网络时，他们会看到一个网页，里面有这个笨蛋的视频。

休息之后你可以看看[托尼]的演示。

[https://www.youtube.com/embed/GlQD9sxTsAw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/GlQD9sxTsAw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)