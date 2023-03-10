# 围绕 ATmega 芯片构建无刷电机控制器

> 原文：<https://hackaday.com/2013/09/21/building-a-brushless-motor-controller-around-an-atmega-chip/>

你知道，当你看到这样的东西时，它会很棒，我们不会对第一印象失望。[Davide Gironi] [使用 ATmega8 作为大脑，从头开始构建无刷电机控制器](http://davidegironi.blogspot.it/2013/09/a-simple-brushless-sensored-motor.html)。如果你想理解一门学科的方方面面，这就是如何做到的。幸运的是，他解释了原型的每个部分的功能。

无刷电机里面没有电刷(咄)。但是这到底意味着什么呢？为了旋转电机，一个精心制作的信号通过固定部分(称为定子)的电机线圈发送，产生一个磁场，推动转子中的永磁体。制作这种信号的一个重要部分是知道转子的位置。这通常通过霍尔效应传感器来实现，但也可以在没有霍尔效应传感器的情况下，通过测量当前未被驱动的线圈中的反电动势来实现。[Davide]组装的 AVR-GCC 兼容库可以进行调整以适应任何一种设置。

休息之后好好看看这个系统。

[https://www.youtube.com/embed/QTgIheFb8zk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/QTgIheFb8zk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[via [危险原型](http://dangerousprototypes.com/2013/09/20/a-simple-brushless-sensored-motor-driver-for-avr-atmega/)