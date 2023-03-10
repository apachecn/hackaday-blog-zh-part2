# 把逆向地理缓存的大脑放在外面

> 原文：<https://hackaday.com/2013/03/20/putting-the-brains-of-a-reverse-geocache-on-the-outside/>

![ioio](img/82be7250f0dde4e9f299f37a2645d4a7.png)

反向地理缓存——一个只在特定地理区域打开的盒子——在 Hackaday 一直很受欢迎。我们看到大量不同的实现，但是大多数时候，构建是相当相似的。当然，将 GPS 接收器专门用于反向地理缓存并不便宜，所以[Eric]提出了一个更好的解决方案。他用一部智能手机作为他的地理缓存的大脑，让他可以把 GPS 和显示器放在锁着的盒子外面。

构建从找到一个旧盒子并修改它开始，这样它就可以用伺服系统锁定。盒子里仅有的其他电子元件是一个 IOIO 板、一个电池组和一个用于存储一些设置的 I2C EEPROM。在手机方面，[Eric] [编写了一个 Android 应用程序](https://play.google.com/store/apps/details?id=com.androchill.reversegeocache),作为他的反向地理缓存的编程接口、UI 和 GPS 硬件。它就像我们见过的所有其他反向地理藏宝车一样，只是这次控制是无线的。

[Eric]放了一个视频演示他的反向地理缓存。休息之后你可以去看看。

[https://www.youtube.com/embed/CGC7AH99Yzk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/CGC7AH99Yzk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)