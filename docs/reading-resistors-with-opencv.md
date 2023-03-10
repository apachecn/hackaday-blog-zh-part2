# 利用 OpenCV 读取电阻

> 原文：<https://hackaday.com/2015/05/14/reading-resistors-with-opencv/>

这是我听过好几次的一个干瘪工程师的建议。如果你正在检查一个有故障的电路，看看电阻颜色代码。有时，如果电阻过热，颜色代码带会改变颜色，从橙色变为棕色，从蓝色变为黑色，等等。如果你知道你喜欢的电阻值，你可能会发现一个电阻值不合适的电阻。这是电路过热的地方，你可能就快发现问题了。

这种技术的问题在于，您必须查看并解码所有电阻。如果自动化和计算机视觉更适合你，[Parth] [开发了一个 Android 应用程序](https://www.youtube.com/watch?v=h_bITwduLPk)，它会通过将摄像头对准电阻来自动告诉你电阻值。

[代码](https://github.com/thegouger/ResistorScanner)使用 OpenCV 扫描屏幕中间的一小行像素。从中提取颜色，电阻值显示在屏幕上。如果你不想学习他们最近教的政治正确的记忆术，它非常适合扫描几百个通孔电阻。

视频，该应用可在 Google Play 商店免费下载[。](https://play.google.com/store/apps/details?id=ca.parth.resistordecoder)

[https://www.youtube.com/embed/h_bITwduLPk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/h_bITwduLPk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)