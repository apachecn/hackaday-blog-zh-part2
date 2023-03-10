# 终极示波器黑客——实时震动

> 原文：<https://hackaday.com/2014/12/29/ultimate-oscilloscope-hack-quake-in-realtime/>

[Pekka]给自己设置了一个相当大的挑战——[使用示波器屏幕实时显示地震](http://www.lofibucket.com/articles/oscilloscope_quake.html)——这可能实现吗？旧的模拟示波器屏幕只是单色的 CRT，但它们是为绘制波形而设计的，而不是绘制图形。

多年来，Hackaday 已经跟踪了显示范围黑客的演变: [Pong](http://hackaday.com/2011/08/01/want-to-play-pong-on-your-oscilloscope/) 、[俄罗斯方块](http://hackaday.com/2014/04/26/playing-tetris-on-an-oscilloscope/)、[矢量显示](http://hackaday.com/2014/02/19/vector-display-output-on-an-oscilliscope/)和[预渲染视频](http://hackaday.com/2014/12/13/tripping-on-oscilloshrooms-with-an-analog-scope/)。没有什么能像这样突破界限。

[Pekka]的解决方案与许多其他解决方案一样，将示波器置于 X-Y 模式并拼接您的耳机线——很容易。然后，他必须想出一些办法来创建一个音频信号，对应于期望的图像。著名的“ [Youscope](http://www.youtube.com/watch?v=s1eNjUgaB-g) ”示例演示了这一点，但该演示是预先呈现的。[Pekka]希望在示波器上实时播放地震，而不仅仅是观看录音。

由于声卡的带宽有限，[Pekka]认为他一次最多可以在屏幕上画一千条线。第一个令人头疼的问题是，他所有的声卡上都有低通滤波器。没办法，他相应地调整了他的上限。ASIO 和 [PortAudio](http://www.portaudio.com/) 是他选择的工具，用来从给定的 XY 线队列中即时创建音频。

为了告诉他的音频引擎要画什么线，他征求了开源的雷神之锤渲染引擎 [Darkplaces](http://icculus.org/twilight/darkplaces/) ，并让它将多边形最小化。然后，他不得不拿出数码树篱修剪机，继续修剪。这篇文章确实不能公正地对待所有巧妙的技巧，这些技巧被用来通过耳机插孔传输最有用的数据。如果你对这种事情感兴趣，那就帮自己一个忙[去看看他的图文并茂的项目日志](http://www.lofibucket.com/articles/oscilloscope_quake.html)。

最终[佩卡]对结果并不完全满意。结果是可玩的，但只是勉强。笔记本电脑努力保持足够简单，声卡努力增加足够的细节，示波器努力足够快地显示所有内容。至少，它为那些希望用这种方法胜过他的人设置了极高的门槛。从岩石中能挤出的水是有限的。

看下面【Pekka】玩雷神之锤第一关的视频。

[https://www.youtube.com/embed/aMli33ornEU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/aMli33ornEU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

感谢:Jay 先生]，[james]，[gudenau]，[AltMarcs]，[Alogus]，[Daniel]以及最后但并非最不重要的[ProfFartSparkles]，他们都非常希望我们报道这个黑客事件并提交了一个提示。