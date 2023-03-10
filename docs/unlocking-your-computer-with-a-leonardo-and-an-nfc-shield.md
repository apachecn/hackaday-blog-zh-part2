# 用达芬奇和 NFC 盾牌解锁你的电脑

> 原文：<https://hackaday.com/2014/04/01/unlocking-your-computer-with-a-leonardo-and-an-nfc-shield/>

[![](img/11491ae2264970d64570293bb93c8010.png)](http://hackaday.com/wp-content/uploads/2014/04/fsqiuvyhtddvy2t-large.jpg)

每次你需要在电脑上登录时手动输入你的登录密码会很烦人，尤其是当密码又长又复杂的时候。为了解决这个问题，[Lewis]通过使用 Arduino Leonardo 和 NFC 盾牌组装了一个[NFC 电脑解锁器](http://www.instructables.com/id/NFC-Computer-Unlocker/?ALLSTEPS)。由于后者没有焊接接头，所以需要做一些简单的工作。

印刷了定制的外壳，以便将两块板放在一起，并将其单独安装在桌子下，以便于使用。幸运的是，由于[Lewis]使用了 Adafruit NFC 库，所以只需要很少的代码。主程序基本上扫描附近的 NFC 卡，将它们的(大字节序的)uid 与存储的 uid 进行比较，并在匹配时输入存储的密码。我们认为这是新一代业余爱好者的第一个好项目。这与我们在 9 月份看到的项目是一脉相承的。

(你会注意到我写这篇文章时没有提到那个你知道的项目！)