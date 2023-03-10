# 拾放机的简陋开端

> 原文：<https://hackaday.com/2014/03/23/humble-beginnings-of-a-pick-and-place-machine/>

![beginnings](img/d44041046731ccbb4af80f47b11dcd24.png)

[Pete's]发明了一种称为空中接线电缆的产品，旨在与飞机的内部通信系统连接，并希望自己制造和组装它们——不幸的是，电路板很小，SMD 组件并不容易安装。所以他决定制造一台[拾取和放置机器来替他做这件事！](http://petemills.blogspot.ca/2014/03/diy-pick-and-place-machine-part-1.html)

它还没有完成，但是[Pete]已经达到了一个重要的里程碑——他已经完成了基本的 CNC 机器部分。他选择了一个主要机械部件的套件，shape oko 2——这是一个可靠的设计，如果你决定从头开始制作一些东西，可能会花费更多时间。

从那时起，他开始单独选择他的电子产品。他选择了 Sparkfun 的大而简单的驱动程序来控制他的步进电机，它支持最大尺寸的 NEMA 17 步进机，所以他也买了五个。为了控制这一切，他使用了 [LinuxCNC](http://www.linuxcnc.org/) 这是一个很好的选择——如果你对 Linux 不疯狂，你实际上可以下载 [Ubuntu 10.04，预装了 Linux CNC](http://www.linuxcnc.org/index.php/english/download)让你变得超级简单——你只需要一台旧的专用 PC 就可以使用。

一旦一切就绪，他编写了一个快速程序来控制他未来的拾取和放置机器——他将一支笔绑在 Z 轴上，它划掉了第一个单词:“Gangsta”。因为你知道，g 代码。对吗？是啊。无论如何，我们非常期待看到这一进展。

[https://www.youtube.com/embed/oH2QoTdPOCY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/oH2QoTdPOCY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

要查看已经运行的拾取和放置机器，请查看这个[漂亮的作品！](http://hackaday.com/2012/10/29/diy-pick-and-place-builds-boards-is-awesome/)