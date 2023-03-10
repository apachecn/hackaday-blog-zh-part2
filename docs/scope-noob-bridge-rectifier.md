# 经营范围:桥式整流器

> 原文：<https://hackaday.com/2014/12/03/scope-noob-bridge-rectifier/>

欢迎回到本周的部分，在这里我将分享我学习使用我的第一台示波器的经历。上周[我开始用 AC-AC 壁式电源适配器测量电源频率](http://hackaday.com/2014/11/26/scope-noob-probing-alternating-current/)。对于那些跟随的人来说，家庭作业是建造一个桥式整流器，并探测其中的信号。让我们来看看。

[https://www.youtube.com/embed/7Q0W-IHu1UM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/7Q0W-IHu1UM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

## 桥式或全波整流

[![bridge-rectifier-shunt-before](img/647e60e870030d09aadac4f78597213f.png)](https://hackaday.com/wp-content/uploads/2014/12/bridge-rectifier-shunt-before.png) 左边是一个全波整流器的示意图。同样，需要注意的重要一点是，我使用的是一个 2 脚“壁式电源”AC-AC 适配器，它可以将 120V 线电压转换为 12V。因此，我使用 1N4001 二极管来制作桥式整流器。

桥式整流器也被称为全波整流器，因为它们接受交流电，并使用波形的两部分来产生直流电。完整的解释并不是本专栏的目的，所以请查看顶部的[本教程等资源(链接已失效，请尝试](http://www.electronics-tutorials.ws/diode/diode_6.html)[互联网档案](https://web.archive.org/web/20141101074850/http://www.electronics-tutorials.ws/diode/diode_6.html))了解这一概念背后的理论和数学。

[![DS1Z_QuickPrint4](img/da8a2ec535568f3899865921748807c5.png)](https://hackaday.com/wp-content/uploads/2014/12/ds1z_quickprint4.png) 我做了一个这些测量的视频，嵌在上面。我首先再次探测输入的交流波形，以确保我有一个已知的起点。这一次我使用“AC”作为触发源，通过按下示波器触发部分的菜单按钮可以找到它。这使用电源信号供电的范围来触发测量，这是非常方便的这个特定的练习。

但当我去探测整流波形时，我遇到了一个惊喜。我的全波整流信号在示波器上只显示为半波整流。右边的截图显示了一个向上的曲线，后面是一个平坦的区域，这里应该有连续的弧线。

## 你不能一次探测所有的东西

 [![bridge-rectifier-shunt-after](img/b4f9bc96e22140bd4def12fe828e881b.png "bridge-rectifier-shunt-after")](https://hackaday.com/2014/12/03/scope-noob-bridge-rectifier/bridge-rectifier-shunt-after/)  [![DS1Z_QuickPrint5](img/ffefb7e1b03b6c3914b5aa13435bbdb5.png "DS1Z_QuickPrint5")](https://hackaday.com/2014/12/03/scope-noob-bridge-rectifier/ds1z_quickprint5/) 

我只花了几分钟的时间就想出了这个问题。连接两个探针(通道 1 和 2)的基准电压夹后，我实际上是在其中一个二极管周围分流，有效地将电桥变回半波整流器。这是因为，正如我上周所说的，示波器上所有通道的参考夹相互连接，并连接到示波器电源线上的接地引脚。

将通道 1 从交流测量中断开会产生我所期望的全波整流信号。但有一个问题我需要帮助回答:为什么每隔一个波形转换有点错位？我原以为每一次转换都会有一致的波形。

## 平滑和调节

[![DS1Z_QuickPrint7](img/844ef79cd68a06f305a599840ab8e084.png)](https://hackaday.com/wp-content/uploads/2014/12/ds1z_quickprint7.png)

为了完成这组测试，我在 DC 连接处增加了一个电解电容来平滑输出。该电容同时低于和高于规格，为 3300uF，但仅为 10V。这是我从一个旧主板上取下的一个盖子，和我的一些跳线一样松散地漂浮在同一个容器中。

上图显示了通道 1 上的稳压电源轨(黄色)和通道 2 上的平滑 DC 轨(蓝色)。根据这些测量，7805 输出 5.79 伏。当我制作视频时，我感到困惑，因为我认为平滑后的信号比没有电容时的电压高。现在看截图，我意识到事实并非如此。我认为这也是重要的一课。在对电路进行故障诊断时，拍摄屏幕截图，以便您可以再次检查您认为已经记住的值！

## 家庭作业

[![erroneous trigger](img/f43653b0f5a9e29df7d034344ff93c54.png)](https://hackaday.com/wp-content/uploads/2014/12/erroneous-trigger.png) 我已经为下周的专栏做了一些工作，我非常兴奋地分享我学到的所有东西。这里有一点好东西的味道。我应该在示波器上只看到一个正弦波，但我得到了两个。我也很高兴在信号中找到一个小问题，并使用它在我的代码中找到原因。

本周你自己也来试试吧。我使用微控制器驱动 R/2R 梯形电阻，从而实现直接数字合成。[Bil Herd]对主题的深入解释启发了我。如果你像我一样使用微控制器，我建议你将 8 路数字输出分配到微控制器的两个端口，看看会发生什么。我将在下周讨论这个和更多的内容！

我还需要关于未来 *Scope Noob* 主题的建议，所以请在下面留下评论，让我知道你认为我应该尝试什么。