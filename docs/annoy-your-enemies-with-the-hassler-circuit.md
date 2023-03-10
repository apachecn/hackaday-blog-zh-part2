# 用哈斯勒电路骚扰你的敌人

> 原文：<https://hackaday.com/2015/01/29/annoy-your-enemies-with-the-hassler-circuit/>

[克雷格]最近为自己建造了一个版本的[“哈斯勒”赛道](http://www.analogzoo.com/2015/01/building-the-widlar-hassler/ "Hassler circuit")，作为对鲍勃·威德拉的一种敬意。如果你没听说过 Bob Widlar，他是模拟 IC 实现的关键人物。我们在过去的中已经深入报道过这个话题[。哈斯勒电路是一个简单而巧妙的办公室恶作剧。这个想法是，电路发出一个非常高的频率音调，但只有当房间里的噪音水平达到一定的阈值。如果你的同事变得太吵，他们会突然注意到耳鸣。当他们停止说话以确定来源时，噪音就消失了。想要的结果是让你的同事闭嘴。](http://hackaday.com/2014/04/08/heroes-of-hardware-revolution-bob-widlar/ "Bob Widlar")

[Craig]找不到任何公布的原始电路原理图，但他设法用分立元件和 IC 构建了自己的版本。声音首先通过一个小型驻极体麦克风进入电路。然后，信号被放大、半波整流，并通过低通滤波器。麦克风的增益可通过调整电位计进行配置。电容器将输出转换成平坦的 DC 电压。

该信号然后被传递到一个张弛振荡器电路。该电路产生一个信号，其输出占空比取决于输入电压。输入电压越高，占空比越长，频率越低。产生的信号被送到一个小扬声器输出。扬声器也由施密特触发器控制。这可以防止扬声器在电压达到某个阈值之前通电，从而节省能源。整个电路是焊接在一起死臭虫风格，并安装到覆铜板。

房间安静时，输入电压较低。输出频率足够高，超出了人的听觉范围。随着房间慢慢变大，电压增加，输出频率降低。最终，它达到了人类听觉的极限，房间里的人都注意到了。下面的视频一步一步地介绍了电路。

[https://www.youtube.com/embed/b0A_5H801rk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/b0A_5H801rk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)