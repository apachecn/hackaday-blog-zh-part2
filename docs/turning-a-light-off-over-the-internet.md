# 通过互联网关灯

> 原文：<https://hackaday.com/2012/05/03/turning-a-light-off-over-the-internet/>

![](img/84484f4db5dd04b487d379b357bf8feb.png "switch")

因为伸出几英尺去关掉一个开关对布鲁斯来说太难以忍受了，他把他的台灯连接到了互联网上。这是一个非常酷的构建，是将任何东西连接到互联网的完美教程。

对于他的构建，[Bruce]使用了一个 Arduino，一个继电器连接到一个输出引脚。当 Arduino 在其串行端口上接收到信号时，一个微小的电压被施加到继电器上，从而打开灯。

这本来可以用 Arduino 以太网来完成，但是[Bruce]使用的 PHP 脚本更加通用。每当有人调出[这个数码灯开关网页](http://84.196.121.49:8080/example.php)，他们就可以打开和关闭【布鲁斯】的台灯。

对于将基本项目连接到互联网的介绍，我们真的很喜欢[Bruce]的构建。不要疯狂地使用那个链接，把失败测试留给专业人士。休息之后你可以看看演示视频。

[https://www.youtube.com/embed/ULmMASScJvo?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/ULmMASScJvo?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)