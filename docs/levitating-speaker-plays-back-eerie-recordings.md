# 悬浮扬声器播放怪异的录音

> 原文：<https://hackaday.com/2014/09/04/levitating-speaker-plays-back-eerie-recordings/>

让我们面对现实吧，悬浮任何东西都是非常迷人的——尤其是当你认为应该有电线的时候。这个项目通过使用 PID 控制器使一个播放音乐的扬声器悬浮起来，为磁悬浮注入了新的活力！

它使用[标准悬浮装置](http://hackaday.com/2013/12/05/avr-atmega-based-pid-magnetic-levitator/)——一个电磁铁、一个永久磁铁和一个霍尔效应传感器。微控制器实现 PID 系统，改变供应给电磁铁的电流，以保持扬声器漂浮在正确的高度。音乐是通过蓝牙无线传输到音箱的，可惜音箱的功率不是。它配备了一个小型锂离子电池，在必须手动充电之前，它的运行时间约为 5 小时。

正如你将在下面的视频中注意到的，有一个浮动扬声器有一个非常有趣的效果——特别是当它开始旋转的时候。

[https://player.vimeo.com/video/104450435](https://player.vimeo.com/video/104450435)

无线传输电力也是可能的，就像我们不久前看到的这个[浮动 LED 项目](http://hackaday.com/2013/12/01/levitating-wireless-led-ring/)——但不管怎样，这都很酷。