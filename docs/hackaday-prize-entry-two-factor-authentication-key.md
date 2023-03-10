# 黑客日奖品入口:双因素认证密钥

> 原文：<https://hackaday.com/2015/07/20/hackaday-prize-entry-two-factor-authentication-key/>

因为在选择密码时，人们通常都是白痴——包括应该更了解的人——谷歌创造了谷歌认证器。这是基于共享密钥的所有谷歌登录的双因素验证。很牛逼，大家都要用。

实际上，从手机应用程序中输入代码是相当烦人的，而[Alistair]有一个更好的解决方案:[一个认证器 USB 密钥](https://hackaday.io/project/5886-authenticator-usb-key)。不是每次他需要验证器代码时都打开验证器应用程序，这个 USB key 会通过按下一个按钮将代码发送到谷歌。

Google Authenticator 背后的算法有据可查，而且实际上非常简单；它只是 Unix 时代以来当前 30 秒周期数和一个 80 位密钥的散列。有了密钥的知识，你可以生成认证码，直到时间结束。[在](http://hackaday.com/2013/09/14/using-google-authenticator-with-an-arduino/)之前已经用 Arduino 完成了，但是【Alistair】的项目使这成为一种不接触键盘就能输入代码的极其方便的方式。

目前的计划是使用 ATMega328、实时时钟和 VUSB 来生成认证码并将其发送到计算机。在设备上获取密钥听起来很棘手，但[Alistair]对此有自己的锦囊妙计:他将使用光学传感器和网页上的闪烁图形将密钥发送到设备。这是一个有点笨拙的解决方案，但是考虑到密钥只需要被编程一次，这不一定是一个坏的解决方案。

通过一个插入 USB 集线器的小按钮，[Alistair]为那些对每隔几天打开 Authenticator 应用程序感到恼火的人提供了一个完美的设备。它不是应用程序的替代品，只是让一切变得更容易。

#### 2015 年[黑客日奖](http://hackaday.io/prize)由以下机构赞助:

[![](img/8e6c49d55ea91b307d7d191b75ab18c8.png)](http://hackaday.io/atmel)[![](img/6b53a13e67e0346985e237ef126c1bcc.png)](http://hackaday.io/freescale)[![](img/3fe105965ef22414d89f71032d9babee.png)](http://hackaday.io/microchip)[![](img/ebcbe4e97993de26ebcf849e70523a14.png)](http://hackaday.io/mouser)[![](img/15f4f8aaed16b020832d8be6282e47f5.png)](http://hackaday.io/ti)