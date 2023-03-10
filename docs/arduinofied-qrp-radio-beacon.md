# 阿杜伊加密 QRP 无线电信标

> 原文：<https://hackaday.com/2013/02/24/arduinofied-qrp-radio-beacon/>

![moxpd](img/84b3d33385b1e181549d35f3ab38a782.png)

不久前，[m0xpd]从 ebay 上买到了便宜得令人难以忍受的 AD9850 DDS 模块。他把它变成了一个 Raspberry Pi 供电的无线电信标，但像许多美化我们页面的构建一样，trolls 不喜欢为这样一个简单的设备使用如此强大的计算机。为了让这些巨魔安静下来，[m0xpd]又回来了，这一次使用 [AD9850 DDS 模块作为带有 Arduino 的无线电信标](http://m0xpd.blogspot.co.uk/2013/02/arduino-beacon.html)。

这个版本的前代使用了树莓 Pi，因此需要一个电平转换器。这被视为[m0xpd]自己的 Arduino 克隆产品，[WOTDUINO](http://m0xpd.blogspot.co.uk/2013/02/what-do-i-know.html)——发音为“我知道什么”——能够处理 AD9850 的 5v IO。

除了为 DDS 模块制造屏蔽外，[m0xpd]还建造了一个发射机屏蔽来放大信号，并允许' duino '键出一些简单的信息。这是一个相当有能力的设备——[ m0xpd]的一条信息从快乐的古老英格兰传到了亚利桑那州，这是他向西最远的一次。