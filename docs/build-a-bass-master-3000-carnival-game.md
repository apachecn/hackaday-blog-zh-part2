# 建立一个低音大师 3000 嘉年华游戏

> 原文：<https://hackaday.com/2014/06/28/build-a-bass-master-3000-carnival-game/>

![Bass Master 3000](img/f7d32781a82a44c2142ff2d78480dc3b.png)

我们都经历过。当你在狂欢节上漫步时，你正玩得开心，突然发现自己走过了狂欢节游戏。在摊位工作的人在嘲弄你，试图让你玩他们的游戏。不过，你知道真相。那些游戏被操纵了。你不知道他们是怎么做到的。你只知道他们会…不知何故。

现在你可以放下你的忧虑，建立自己的嘉年华游戏！[约翰]建立了他自己的"[贝斯大师 3000](http://manganlabs.com/build-bassmaster-carnival-game/774/ "Bass Master 3000") "风格的嘉年华游戏，并发布了一个[指令](http://www.instructables.com/id/Bass-Master-3000/?ALLSTEPS "Instructables")，所以你也可以做一个。

这个游戏非常简单。你有一个张开大嘴的巨大鱼形靶子。你拿着一个末端有橡皮球的小渔线轮。你的目标是把球扔出去，击中鱼的大嘴。如果你打嘴，你会听到一个响亮的蜂鸣声，并看到一些闪烁的灯光。该系统还使用网络摄像头偷拍获胜者的照片。电脑屏幕显示了当天所有的获胜者。

这个系统的大脑是一个 Arduino Yún。Yún 类似于 Uno，但它也有一些额外的功能。一些很好的例子是以太网端口、无线适配器和 SD 卡插槽。嘴部传感器只是两个压电元件。每个传感器都通过一个小的微调电位计连接到 Arduino。这允许您调整每个传感器的灵敏度。灯和蜂鸣器通过继电器控制，由 Arduino 上的 5V 数字引脚触发。

Yún 实际上有一个小型的板载 Linux 计算机，您可以在 Arduino 环境中与之通信。这使得[John]可以使用 Yún 直接从网络摄像头拍摄照片，将照片存储在本地 SD 卡上，并在本地网络服务器上显示。web 服务器运行一个简单的脚本，显示存储在卡上的所有照片的幻灯片。

游戏的最后一部分是物理目标本身。目标是用丙烯颜料画在一块小油布上的。然后将防水布贴在由 PVC 管制成的方形框架上。鱼的嘴是从防水布上切下来的。然后将一大块毛毡放在附有压电传感器的孔后面。一小段铜管有助于压住毛毡底部，并使其固定不动。重要的是确保毛毡没有碰到防水布。如果它接触到，它可能会过于敏感，甚至在玩家错过时触发。

现在你知道如何建立自己的低音大师 3000 嘉年华游戏。你是否操纵游戏取决于你自己。此外，请务必查看下面的系统工作视频。

[https://www.youtube.com/embed/u2QFSoBNwnk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/u2QFSoBNwnk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)