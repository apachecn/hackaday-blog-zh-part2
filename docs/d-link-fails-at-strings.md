# D-Link 在字符串处失败

> 原文：<https://hackaday.com/2015/04/14/d-link-fails-at-strings/>

小型办公室和家庭办公室(SOHO)无线路由器的安全性很差。这没什么新鲜的。但有些可悲的是，制造商只是不断重复利用相同的坏固件。:D 林克公司的新型 DIR-890L 就是一个很好的例子，它看起来像一只乌龟。[Craig]查看了奇怪的外壳，并从 D-Link 的网站上获取了该设备的最新固件。然后他[发现了一个严重的漏洞](http://www.devttys0.com/2015/04/hacking-the-d-link-dir-890l/)。

[![D-Link's DIR-890 Router](img/42672e359a6a012cf724f43c8f03cd8c.png)](http://hackaday.com/2015/04/14/d-link-fails-at-strings/dir890/)

通常的过程应用于固件映像。提取它，运行 [binwalk](https://github.com/devttys0/binwalk) 找到固件映像的各种内容，然后提取根文件系统。这包含了运行路由器各种服务的所有代码。

CGI 脚本是发现问题的明显地方。[Colin]分解了处理所有 CGI 请求的单个可执行文件，并开始查看处理[家庭网络管理协议](http://en.wikipedia.org/wiki/Home_Network_Administration_Protocol) (HNAP)请求的代码。第一个发现是，系统命令是使用 HNAP 数据构建的。数据没有被清理，所以需要的只是一种绕过身份验证的方法。

这就是 D-Link 犯下重大错误的地方。他们希望允许一个特定的 URL 不需要认证。看起来很简单，比较字符串 A 和字符串 B，确保它们匹配。但是他们使用了 [strstr](http://man7.org/linux/man-pages/man3/strstr.3.html) 函数。如果字符串 A *包含*字符串 b，这将返回 true。

所以可以绕过认证，可以启动 telnetd，瞧:D-Link 最金字塔形路由器上的一个根 shell。哦，你不能禁用 HNAP。我们可以建议 [OpenWrt](https://openwrt.org/) 或者 [dd-wrt 吗？](http://www.dd-wrt.com/site/index)