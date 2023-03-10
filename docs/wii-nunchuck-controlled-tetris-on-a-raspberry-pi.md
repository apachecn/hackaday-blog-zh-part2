# Wii 双截棍控制的俄罗斯方块在树莓皮上

> 原文：<https://hackaday.com/2013/12/14/wii-nunchuck-controlled-tetris-on-a-raspberry-pi/>

[![tetris](img/f8ab756066f5819cd2ccaaebc0ce6902.png)](http://hackaday.com/wp-content/uploads/2013/12/tetris.jpg)

[Vince]在缅因大学教嵌入式系统课，他的一些学生正在为他们的期末考试做视频游戏。他决定[“测试”学生们正在使用的硬件](http://www.deater.net/weave/vmwprod/hardware/pitris/)，将两个 8×8 显示器、一个 4×7 分段显示器和一个 Wii 双节棍放在 I2C 的公交车上。然后他写了一个版本的*俄罗斯方块*，它接受触发器按压和加速度计输入进行控制。从视频来看(休息后嵌入)，树莓派运行游戏没有问题。当然，公共汽车完全有能力处理一切事情。

不幸的是，[文森特]很难控制好。有时掉落一块会导致下一块掉落得太快，加速度计控制似乎有点太敏感了。我们想象使用操纵杆进行旋转，并在游戏中添加一些战略性暂停会有所帮助。他大方地发布了项目的[源代码，所以也许在不久的将来我们会看到一些拥抱和扩展。](https://github.com/deater/vmw-meter/tree/master/nunchuck)

[https://www.youtube.com/embed/LOmpkivQIkM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/LOmpkivQIkM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)