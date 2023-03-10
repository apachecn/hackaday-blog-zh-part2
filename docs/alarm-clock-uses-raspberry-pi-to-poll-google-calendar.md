# 闹钟使用树莓派来调查谷歌日历

> 原文：<https://hackaday.com/2013/06/06/alarm-clock-uses-raspberry-pi-to-poll-google-calendar/>

![rpi-google-calendar-alarm-clock](img/a1d62f9e811ff0834cfade4566dafd34.png)

我们知道很多人喜欢将他们的智能手机用作床头闹钟。问题是，手机本质上是移动的，最终某天晚上你会忘记把它放在卧室里。这就是为什么我们喜欢[德文·布雷]选择的解决方案。他把他的树莓派设置成一个闹钟，用谷歌日历设置。

他在视频中展示的设置非常简单。树莓派连接到一组电动电脑扬声器。每当谷歌日历上出现一个名为“唤醒”的约会时，它就会播放一首歌。这是通过使用 [Google 数据 APIs Python 客户端库](https://code.google.com/p/gdata-python-client/)来完成的(是不是有点拗口？).

这仅仅触及了可能的表面。有了这个，你就可以很容易地在房间里安装 led 灯来发出日出警报。但是如果你喜欢更简单的硬件方面的东西[，那也是可能的](http://hackaday.com/2012/04/25/automating-household-devices-with-google-calendar/)。

[https://www.youtube.com/embed/SGQ6t0-9W_c?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/SGQ6t0-9W_c?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)