# 微控制器语音合成让你的项目被听到

> 原文：<https://hackaday.com/2014/03/02/microcontroller-speech-synthesis-lets-your-project-be-heard/>

![](img/43052ac9f7945b8cb7381e6599309153.png)【Aditya】有一个项目需要口语输出。他承认他本可以构建一个基于 PC 的解决方案，但他发现通过使用微控制器来添加语音[不仅是一个便宜和便携的替代方案，而且是一个有趣和容易的构建。](http://skinnysatan.wordpress.com/2014/01/30/adding-speech-to-your-embedded-project/)

他的设计使用了 ATMega128。许多微控制器都可以工作，但他的主要需求是 PWM 产生和大量存储文件的内存。输出经过简单的低通滤波器净化后，进入 8ω扬声器。

[Aditya]以 WAV 格式播放他的曲目，然后压缩到 8 位/8kHz。他发现了一个 C++函数，可以将轨迹数据转换成一个巨大的数组，然后将其数字化。他使用两个定时器，一个用来产生波形，另一个用来计时方波。[Aditya]在他的网站上有一个样本 zip，可以读出数字 0-9。