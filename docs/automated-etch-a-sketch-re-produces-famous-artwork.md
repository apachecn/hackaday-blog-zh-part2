# 自动化蚀刻草图重现著名艺术品

> 原文：<https://hackaday.com/2015/02/02/automated-etch-a-sketch-re-produces-famous-artwork/>

除非你是比战斗机飞行员更灵巧的天才，否则在草图上制作任何东西都很难。所以【埃文】决定[把它机动化，](http://www.evanlong.info/projects/etching/)再骗一点。

她使用 Arduino Uno 来控制两个步进电机，她使用一小段橡胶管和大猩猩胶水将这两个电机绑定到 Etch-a-Sketch 旋钮。她 3D 打印了一些定制的电机支架，允许电机直接放置在旋钮上方，以及一个 ULN2803 来切换步进器所需的 12V。

在她设置好所有硬件之后，她编写了一个简单的 Python 脚本。png 并生成通过 Arduino 发送的矢量艺术。如果你想知道，蚀刻草图大约有 550 x 370 像素，或者大约 500 x 320 的“安全区域”。

由于 Etch-a-Sketch 的局限性，比如它不能停止书写，一些图像在发送到新的 Etch-a-Sketch 打印机之前可能需要一些编辑。

[https://player.vimeo.com/video/114496052](https://player.vimeo.com/video/114496052)

虽然蚀刻素描是许多人童年生活的祸根，但也有不少人进行了报复。蚀刻素描钟？[检查。](http://hackaday.com/2014/03/28/an-etch-a-sketch-to-fetch-the-time/)蚀刻草图 CNC？[检查](http://hackaday.com/2011/03/14/cnc-etch-a-sketch-draws-on-itself/)。自动蚀刻草图？[止。](http://hackaday.com/2012/02/06/robotic-etch-a-sketch-draws-grayscale-images/)