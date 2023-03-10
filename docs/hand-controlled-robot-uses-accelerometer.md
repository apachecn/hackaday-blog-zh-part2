# 手控机器人使用加速度计

> 原文：<https://hackaday.com/2015/08/16/hand-controlled-robot-uses-accelerometer/>

管弦乐队指挥、巫师和 Leap 控制器用户有什么共同点？他们都是通过挥手来控制事物的。[萨达姆]一定想要同样的效果，所以他创造了一个机器人，他用手势无线控制这个机器人。

加速度计读取手部动作，并通过射频模块将其发送到 Arduino。这是一个小技巧，因为这个设备产生一个模拟值，萨达姆使用一些比较器来数字化射频发射机的信号。发射端没有 Arduino 或其他 CPU(除了射频模块中的任何东西)。

从视频来看，这似乎是一种控制机器人的自然方式，只要你不介意用管道将发射器绑在手上。当然，如果你是一个真正的黑客极客，你甚至可以认为这是一个优势，因为你可以假装你正在努力成为一个电子人。

[Saddam]花了一些时间谈论加速度计的内部工作原理，如果你感兴趣的话，我们之前已经讨论过了。事实证明，这些设备并不像我们通常认为的那样是电子的，而是机械的。

[https://www.youtube.com/embed/IEVK3PpQTho?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/IEVK3PpQTho?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)