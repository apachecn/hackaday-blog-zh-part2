# 黑客超越 Wifi SD 卡

> 原文：<https://hackaday.com/2013/08/12/hacking-transcend-wifi-sd-cards/>

[Pablo]最近自豪地拥有了一张 Transcend WiFi SD 卡。它可以让他在几秒钟内将照片传输到任何支持 WiFi 的设备上。

由于他怀疑上面运行着某种 Linux，他开始尝试是否能在上面获得根访问权限……[并成功了](http://haxit.blogspot.ch/2013/08/hacking-transcend-wifi-sd-cards.html)。

他清晰而详细的文章从解释一个简单的技巧如何让他浏览卡的文件系统开始，这个文件系统(他猜对了)正在运行 busybox。从那里，他能够看到任何写得很差的 Perl 脚本是否有安全漏洞…并且得到了比他期望的更多的东西。

他首先认为他已经找到了一种方法，通过发出一个特殊的 HTTP POST 请求，使嵌入式 Linux 启动用户提供的脚本并执行命令…由于一个小的技术问题，这个方法失败了。他的第二次尝试成功了:[Pablo]发现用户设置的密码是直接在 Linux shell 命令中输入的。因此，密码“adminecho haxx > /tmp/hi.txt # "可以创建一个 hi.txt 文本文件。

从那以后，事情变得容易了。他只需让该卡下载另一个 busybox，就可以使用该卡的 Linux 中原本禁用的所有命令。最后，他拿到了一张卡，可以把 bash 连接到他的电脑上，这样他就可以发出任何他想要的命令。

因为这还不够，[Pablo]甚至发现了一个简单的方法来找到卡的当前密码。谈论安全性…