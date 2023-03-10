# 升级旧灯笼

> 原文：<https://hackaday.com/2015/07/07/upgrading-an-old-lantern/>

[冲击波]偶然发现一些旧煤油灯，并决定他也偶然发现他的下一个项目。他决定不使用煤油，取而代之的是使用一些 RGB 发光二极管来让灯笼复活。这是相当大的升级。考虑到燃烧的煤油只会发出几种颜色的光，精明的读者会意识到 RGB 阵列有能力发出超过 1600 万种颜色的光。

经过一些初步测试后，他选定了一个由 ATtiny85 供电的 24 LED 圆形阵列。FastLED 库帮助他将代码保持在严格的内存要求内。[shock war]不习惯使用这么少的内存，但经过一番摆弄，他终于能够使用 8126 字节的内存了。

来源可以在他的 [github](https://github.com/shockwaver/lantern) 页面找到。一定要看看下面的视频，看看 RGB 灯的作用。

[https://www.youtube.com/embed/Njs6zNSPdB0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/Njs6zNSPdB0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)