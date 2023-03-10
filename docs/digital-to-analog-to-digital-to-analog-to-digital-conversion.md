# 数模-数模-数模转换

> 原文：<https://hackaday.com/2015/01/03/digital-to-analog-to-digital-to-analog-to-digital-conversion/>

[Andy]有了将混音台变成 MIDI 控制器的想法。乍一看，这个想法似乎非常实用——混音器是在一个便宜、紧凑、坚固的外壳中获得大量拨号盘和推子的好方法。确切地说，如何将混音器转变成 MIDI 设备才是最重要的。[这种建造可能不是最高效的](http://doktor-andy.de/wordpress/?p=1269)，但它有一个有史以来最好的名字:数字到模拟到数字到模拟到数字的转换。

这一过程始于在 Arduino [上产生一个正弦波，并进行一些直接数字合成](http://interface.khm.de/index.php/lab/interfaces-advanced/arduino-dds-sinewave-generator/)。ATTiny85 产生一个 480 Hz 的方波。然后，这两个信号都被馈入 74LS08 与门。根据[Andy]发布的原理图，这些信号进入两个不同的门，门的另一个输入被拉高。该门的输出然后通过一对电阻发送，并组合成“音频输出”信号。[安迪]说这是专业人士的“脊椎爬行”。如果有人知道电路的这一部分*实际上是做什么的，*请在评论中留下注释。

来自与门的信号然后被馈入混频器，并被发送到另一个 Arduino 的模拟输入端。该 Arduino 使用快速哈特利变换将混音器输出的音频转换为频率。有了调音台内部发生的事情的二进制表示，[Andy]就有了可以转换成 MIDI 的东西。

[安迪]放一个这个电路工作的演示。他将 MIDI out 连接到 Abelton，并可以使用混音器修改 MIDI 参数。下面的视频，如果你还在想这个问题的话。

[https://www.youtube.com/embed/u5r6i65eHKk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/u5r6i65eHKk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)