# 你口袋里的是调谐器吗？

> 原文：<https://hackaday.com/2015/01/29/is-that-a-tuner-in-your-pocket/>

作为一名音乐家，很少能用肉眼识别出一件乐器是否合拍。市场上有很多电子设备可以帮助你做到这一点，然而，如果你要即兴表演给朋友留下深刻印象，使用一个就像睡前戴上牙套一样温和。当调整是必要的时候，为什么不用一种不会束缚你风格的方式呢？

为了帮助他的音乐专业朋友在日常工作中加入邦德式的闪光元素，[dbtayl]设计了一个伪装成怀表的[半音阶调音器，昵称为“pokey”。定制外壳的形式是在 OpenSCAD 中设计的，并在](http://hackaday.io/project/2312-pokey-watch)[自制的数控铣床](http://hackaday.com/2013/08/16/101459/)上从铝原料上切割下来。在其低音谱号装饰的盖子下是 PCB，它是用 KiCad 设计的，以适应手表的圆形空腔，然后从一块覆铜板铣削而成。该板包含恩智浦 Cortex M3，它充当调谐器的大脑，运行 FFT(快速傅立叶变换),使用麦克风将其听到的主音高与最近的音符匹配。侧面的五个蓝色表面贴装 led 指示音符的尖锐或平坦程度，中心为真。

在与机械功能紧密相关的事物中，电路的并置是对我们熟悉度的巧妙利用。你可以在下面看到这个小饰品的测试视频:

[https://www.youtube.com/embed/N0xrQXRuOJQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/N0xrQXRuOJQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)