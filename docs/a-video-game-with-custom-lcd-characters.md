# 带有自定义 LCD 字符的视频游戏

> 原文：<https://hackaday.com/2013/07/23/a-video-game-with-custom-lcd-characters/>

![LCD](img/f9b54a85e1f95b1eb2fed479911be162.png)

[Nakul]想要制作一个视频游戏，随着一些 Arduino 项目经验的积累，他决定最终实现他的目标。他[使用了一个字符液晶显示器](http://nakulrao.wordpress.com/2013/07/23/arduino-video-game/)来制作他的游戏，而不是基于文本的冒险，他用了一个图形侧滚动条。

这个基于空间的侧滚动条的显示不是像 CRT 或图形 LCD 那样的图形显示。相反，[Nakul]正在使用无处不在的日立 HD44780 字符液晶显示器。通常这些用于显示文本，但它们都能够显示自定义的 5x8 像素字符。代码将这些自定义角色——飞船、导弹和障碍物——放入显示器的内存中，并将它们用作视频游戏的精灵。

你可以在[他的 git](https://github.com/nakul13/Arduino-Video-Game) 上下载【Nakul】的代码，或者看看下面的动作视频。【T2

[https://www.youtube.com/embed/JgQqy9P-3mE?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/JgQqy9P-3mE?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent) [https://www.youtube.com/embed/xqOkMi2o0E0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/xqOkMi2o0E0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent) [https://www.youtube.com/embed/c8C7xiSPxM0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/c8C7xiSPxM0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)