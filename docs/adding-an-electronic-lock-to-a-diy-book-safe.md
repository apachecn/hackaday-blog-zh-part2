# 为 DIY 图书保险箱添加电子锁

> 原文：<https://hackaday.com/2012/04/11/adding-an-electronic-lock-to-a-diy-book-safe/>

![electronic-book-safe](img/05d5c456c5f6c4d3f59fe9125234979b.png "electronic-book-safe")

DIY 图书保险箱很好，但是如果你给某人足够的时间来细读你的藏书，3 英寸厚的“关于 14 世纪畜牧业技术的案例研究”可能会在你收集的手工装订的“暮光之城”同人小说中脱颖而出。为了教他的朋友一点关于微控制器和电路的知识，[Jonathan]花了一些时间为你的笔记本保险箱增加一点安全性。

这两个人开始时是耗时的将书页粘在一起，并为存储和电子设备创造足够的中空空间。这样一来，他们在空腔内安装了一个闩锁和伺服电机，后者由带有 Arduino 引导加载程序的 Atmega328p 控制。为了拿到藏在里面的东西，乔纳森挂上一个 PS/2 小键盘，输入密码。这会触发伺服电机，打开锁闩。

虽然闩锁可能只是给图书保险箱增加了一点点安全性，但这是一个足够有趣的学习练习，值得花时间来组装它。

继续阅读，观看[乔纳森的]电子锁存书安全运行的短片。

[https://www.youtube.com/embed/cUY-xZqdRK8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/cUY-xZqdRK8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)