# 基于 Gameboy 彩色相机的莫尔斯码收发器

> 原文：<https://hackaday.com/2012/12/10/morse-code-transceiver-based-on-gameboy-color-camera/>

[![Morse Code IR Transceivers](img/364009b8ecd37d32de475d993a30bddd.png)](http://hackaday.com/?attachment_id=91414)

为了他们在微控制器课程中的最终项目，[Trudy]和[Josh]设计了一对[莫尔斯码收发器](http://people.ece.cornell.edu/land/courses/ece4760/FinalProjects/f2012/qs44_twc55/qs44_twc55/morsetransceiver.html "Morse Code Transceivers")。为了传递信息，他们使用了一组红外发光二极管。使用 Gameboy 彩色相机接收消息，该相机负责基本的图像处理。这允许 8 位 ATMega1284p 微控制器处理发送和接收消息。

传输 LED 形成一个正方形图案，其中一个 LED 位于中央。四个外部 LED 用于帮助接收器定位中央 LED，中央 LED 用于传输信息。

Gameboy 彩色相机基于 M64282FP 图像传感器。该传感器使用类似 SPI 的协议，他们在 ATMega 上实现了该协议。它允许他们从相机中抓取帧，并获得特定像素的值。从这些数据中，他们找到中央 LED 并处理信息。

结果一次可以传输 200 个字母的信息，但速度受到相机帧率的限制。如果你有一个 Gameboy 彩色相机，他们的详细介绍可能会提供一些灵感和如何在黑客中使用它的信息。