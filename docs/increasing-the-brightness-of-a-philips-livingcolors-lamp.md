# 增加飞利浦 LivingColors 灯的亮度

> 原文：<https://hackaday.com/2015/06/12/increasing-the-brightness-of-a-philips-livingcolors-lamp/>

[Martin]最近购买了一盏飞利浦 LivingColors 灯。这是一种商业产品，基本上作为情绪照明，能够改变许多不同的颜色。[Martin]对他的现成灯的亮度感到失望。与其花几百美元去买更多的灯，他决定改装他已经有的那一个。

[Martin]首先拆下他的灯的前盖。他发现里面有四个明亮的发光二极管。两个红色，一个绿色，一个蓝色。[Martin]将一根电线焊接到每个 LED 的驱动器上。这些导线然后连接到一块原型板上的四个不同的 N 沟道 MOSFET 晶体管。

在连接上他的 [RIGOL 示波器](http://hackaday.com/2014/11/12/how-to-get-50-more-zed-from-your-rigol-ds1054z/)后，【Martin】能够看到每个 LED 都是由一个脉宽调制信号驱动的。他所要做的就是将一个简单的不可寻址 RGB LED 灯条和一个电源连接到他的新驱动板上。现在，灯可以控制 LED 灯条和内部 LED。这极大地扩展了灯的亮度，而对商业产品的修改最小。请务必查看下面的视频，了解完整的演练。

[https://www.youtube.com/embed/p4ACGasGaT8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/p4ACGasGaT8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)