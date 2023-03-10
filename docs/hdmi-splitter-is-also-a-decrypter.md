# HDMI 分离器也是一个解密器

> 原文：<https://hackaday.com/2015/03/12/hdmi-splitter-is-also-a-decrypter/>

当社区聚在一起时，它温暖了我们的心。[esar]需要为他的家庭影院系统获取一个解密的 HDMI 流。评论中的一条密报和大量优秀的老式黑客技术使得一个 HDMI 分路器变成了一个全功能的 HDMI 解密器。故事是这样的。

他的[惊人的定制流光溢彩克隆](http://hacks.esar.org.uk/hdmi-light-v2/)在这里得到了简介，有人在评论中问他，当[高带宽数字内容保护(HDCP)](https://en.wikipedia.org/wiki/High-bandwidth_Digital_Content_Protection) 开启时，它是否工作。[esar]感叹没有。 [Hackaday 读者救场。](http://hackaday.com/2014/12/16/fpga-ambilight-clone-packs-a-ton-of-features/comment-page-1/#comment-2254669)【Alan Hightower】和【RoyTheReaper】向【esar】指出，HDMI 分路器需要对信号进行解密和重新加密才能传输，并向他指出了一个破坏板载微控制器的技巧。从那里起飞。

不幸的是，将微型设备从画面中移除会扰乱许多其他 HDMI 功能。所以[esar]开始挖掘 HDMI 分离器芯片的数据手册，寻找与重新加密相关的寄存器。如果他能进入 I2C 总线上的微控制器和分离器芯片之间，使重新加密失效，他就成功了。

如果你对 I2C 黑客或滥用 HDMI 分路器感兴趣，你需要阅读他的帖子，因为他详细描述了所有的磨难和胜利。他首先尝试通过用 0 覆盖 1 位来强制 I2C。这(正确地)向微处理器发出了总线上有冲突的信号，因此它再次重新发送命令。死胡同。

然后他发现了另一个信号，接收器可以用它来表明它没有解密。他试着连续发送这个到分离器，这样它就会停止加密。这种方法奏效了，但有时只适用于一个频道。事实证明，他的代码在他那位摔坏的 I2C 代码中耗时太长。他解决了这个问题，一切都好吗？嗯，90%的路都是这样。

为了降低最后 10%的功能，[esar]购买了几个分离器，试验了另一个与 3D 兼容的分离器芯片组，并焊接了更多的电线来实现音频返回通道。经过大量有据可查的艰苦工作，他最终取得了胜利。