# 为您的家庭影院添加电动百叶窗

> 原文：<https://hackaday.com/2013/02/07/add-motorized-blinds-to-your-home-theater/>

![motorized-blinds](img/d61ec3b0e761fa5e641492465a72990f.png)

[Chipsy]发现自己遇到了一个有趣的问题。为他的家庭影院服务的房间有一面墙镜，在观看时可以反射部分屏幕。在一个黑暗的房间里，这非常分散注意力。他的解决方案是增加一个百叶窗，在观看时盖住镜子，但谁想不断地拉下百叶窗，然后再拉起来呢？由于他正在使用的电动投影屏幕有一个遥控器，他想出了一个办法来[电动化盲人，并将其与屏幕的遥控器](http://www.instructables.com/id/Automatic-blind-hooked-up-to-existing-projector-sc)同步。

屏幕使用机械继电器来切换电机。他用 Arduino 把这些连接起来，检测屏幕是向上还是向下。对盲人使用他自己的继电器和马达是很容易的，但他需要一种方法来停止盲人一旦到位。为了盖住镜子，他简单地设置了一个 18 秒的计时器，但是为了收回百叶窗，他想要精确的对准，所以他增加了一个磁铁，并用簧片开关来感应它的位置。休息后在剪辑中看到同步的屏幕和百叶窗。

[https://www.youtube.com/embed/2kYMXx6eL4o?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/2kYMXx6eL4o?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)