# 火英雄:树莓派控制烟火

> 原文：<https://hackaday.com/2012/12/22/firehero-raspberry-pi-controlled-pyrotechnics/>

[![Fire Hero 3](img/b3a664ed4ea825dfffc695edf622f30a.png)
](http://hackaday.com/2012/12/22/firehero-raspberry-pi-controlled-pyrotechnics/firehero/)

为了在音乐节上进行现场烟火表演，[克里斯]建造了 [FireHero 3](http://www.chrismarion.net/index.php?option=com_content&view=article&id=170:firehero-3&catid=43:pyrotechnics&Itemid=226 "FireHero 3") 。结果是远程控制的火焰喷射到 100 英尺高的空中。

该系统由树莓 Pi 和 Arduino 控制。服务器在 Pi 上运行，并允许远程计算机控制系统。Pi 通过串行向 Arduino 发送命令，Arduino 切换固态继电器来驱动阀门。

还有一些内置的安全功能:除非你有正确的钥匙和 RFID 标签，否则系统不会启动，还有压力传感器和温度传感器来确保系统安全运行。紧急情况下，CO2 驱动阀可以快速停止燃油流动。

汽化的丙烷产生了火球。蒸汽是通过在热水浴中加热供应罐产生的。一个储罐储存蒸汽，定制的歧管将蒸汽分配给各种火焰炮。在每门加农炮上，一旦阀门打开，氮化硅热表面点火器(HSI)用于点燃火焰。

休息之后，看一段视频，关于消防英雄制造火焰。

[https://www.youtube.com/embed/05zCLWFPDZw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/05zCLWFPDZw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)