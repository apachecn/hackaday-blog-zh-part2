# 将 Raspi 变成 AdBlock

> 原文：<https://hackaday.com/2013/09/15/turning-a-raspi-into-adblock/>

![pi](img/845b92b570731fb472562da9aa9e0380.png)

没有什么比看到带宽浪费在平淡无奇的 flash 动画、不相关的广告和动画 gif 上更让人恼火的了。坏消息是这些广告是很多你喜欢的网站的唯一收入来源——包括 Hackaday。好消息是[你可以用树莓派、WiFi 适配器和终端中的一点乐趣来关闭这些广告](http://learn.adafruit.com/raspberry-pi-as-an-ad-blocking-access-point/overview)。

这个构建创建了一个无线接入点，将 WiFi 适配器插入 Raspberry Pi。通过插入以太网电缆，这有效地将 Raspi 变成了无线路由器。

要配置该软件阻止广告，只需从命令行安装 dnsmasq，并确保您最喜爱的网页上的所有广告都超时。这意味着对你的新 DIY 路由器的性能有相当大的影响，但随着 [Pixelserv](http://proxytunnel.sourceforge.net/pixelserv.php) 的安装，你可以托管一个 1 像素的透明 GIF 图像，取代所有的广告，并使它们不可见。

如果你不喜欢在 PS3、XBox、平板电脑或其他非 PC 互联网设备上看广告，这是一个很好的项目。如果人们窃取你的无线连接是一个问题，那么对于那些流氓 WiFi 盗版者来说，将每张图像颠倒或模糊应该不难。