# 巴尔杜伊诺，现在与脸书融合

> 原文：<https://hackaday.com/2014/05/10/barduino-now-with-facebook-integration/>

![Bar](img/e53bebfcb3a7553dba3702ba49963fed.png)

我们见过自动给你倒饮料的机器人，但是有 RFID 的怎么样？一个和脸书融合的怎么样，这样你的朋友就知道你是个酒鬼了？等等。脸书已经告诉他们了。哼。

[安迪]和[丹尼尔]的最新版本紧随许多类似的鸡尾酒机器人之后；一个 Arduino 控制几个连接到 CO2 供应的电磁阀，几瓶酒和混合器，只需按一下按钮就可以分发饮料。这个项目有趣的地方在于它对 RFID 和脸书的使用。

用户界面是为 Windows 7 编写的，带有一个 RFID 标签(表面上是发给每个来宾的)，允许唯一的登录，该登录检查 SQL server 以查看用户拥有什么特权。该应用程序将用户的脸书个人资料照片拉下来，显示在屏幕的角落里，服务器会跟踪他们喝了多少酒(以及什么种类)，如果有适当的权限，应该可以将这些信息发布到他们的墙上。因为我们都知道你昨晚做了什么，即使你不知道。