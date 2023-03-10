# 射频开关模块可以学习新的遥控器

> 原文：<https://hackaday.com/2013/02/20/rf-switching-module-can-learn-new-remotes/>

![rf-remote-also-learns-by-itself](img/08f3a8c4c3136b0e788a6a42bee5eb56.png)

这个试验电路板是塞尔吉奥无线控制电器的解决方案。具体来说，他希望有一种方法可以从房子里打开和关闭他的泳池泵。因为他手头上有大部分部件，所以他决定自己构建一个解决方案。他最终得到的是一个可以学习从不同远程设备接收命令的射频基站。

主要组件包括图像底部的固态继电器。这使得 ATtiny13 可以切换电源电压设备。微控制器(位于试验板中心的覆铜方块上)与其左侧的绿色射频板接口。右边是一个单叶交换机。这作为输入。快速点击会切换继电器，但三秒钟的按压会将设备置于学习模式。然后,[Sergio]可以按下射频遥控器上的按钮，设备会将接收到的代码存储在 EEPROM 中。正如你在休息后的片段中看到的，他甚至包括了忘记远程代码的方法。

[https://www.youtube.com/embed/EcFoa1AURaI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/EcFoa1AURaI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)