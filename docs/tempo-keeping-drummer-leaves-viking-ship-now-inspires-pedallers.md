# 节奏保持鼓手离开维京船，现在激励踏板

> 原文：<https://hackaday.com/2014/06/13/tempo-keeping-drummer-leaves-viking-ship-now-inspires-pedallers/>

![Bike Controlled Drum Machine](img/cca06e6785a1e9c0b619f37291b27ff2.png)

[Serdef]来信告诉我们他最近创建的一个项目。这是一个[鼓声发生器](http://hackaday.io/project/1449)，它会根据你蹬自行车的速度来改变节奏。这直接与使用音乐来保持你的踏板时间一致和速度相违背。

这个项目从[Serdef]之前制作的一个[tap-tempo 鼓节奏踏板](https://www.youtube.com/watch?v=MGlay8fV_nU)开始。该设备将产生与两个输入信号之间的时间相对应的鼓声。这种类型的设备允许某人，比如说吉他手，快速而容易地指定他们正在演奏的鼓点的速度。

这个项目的主要部分已经想好了，接下来的部分是让自行车的速度触发鼓点的节奏。对于信号输入，车轮每转一圈，安装在车轮上的磁铁触发安装在自行车叉上的簧片开关一次。这与自行车速度计/里程表使用的信息收集方法相同。

这个项目的业务部分包括一个 Arduino，它通过磁性开关测量轮子的速度，调整鼓点的速度，然后通过 MIDI 协议将鼓点发送到合成器。合成器将 MIDI 信号转换为鼓的声音，通过电动扬声器放大，骑手可以听到。整个系统由 9v 电池供电，安装在绑在自行车车把上的项目箱中。

所有的设计文件和 Arduino 代码都可以通过[Serdef 的] excellent write up on hackaday.io 获得，如果你有兴趣为自己制作一个的话。

[https://www.youtube.com/embed/zrgR8VLM19I?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/zrgR8VLM19I?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)