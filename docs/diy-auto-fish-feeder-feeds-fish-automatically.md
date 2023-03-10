# DIY 自动喂鱼器自动喂鱼

> 原文：<https://hackaday.com/2014/10/14/diy-auto-fish-feeder-feeds-fish-automatically/>

[Brian]有一个相当大的 400 升的水族馆，他喜欢以它为家的鱼。不幸的是，有时生活会妨碍定期给这些鱼喂食。市场上有自动喂鱼器，布莱恩试了一试。虽然它工作正常，但它一次扔进一大块食物(而不是洒进去)，食物漏斗只能容纳非常少量的食物，并且该装置在不到一周的时间内耗尽了一组新电池。花了 50 欧元买了那个自动喂食器，最终它并不比喂鱼更方便。

面临着是否购买另一种他可能不满意的产品的艰难决定，[布莱恩]决定用任何人都能在家里找到的零件制作自己的自动喂鱼系统。主外壳是一个小的特百惠垃圾桶，里面的 3 片塑料被粘在一起，形成一个 v 形的漏斗。鱼食被装入料斗，当它落到底部时，会遇到一个像螺旋钻一样的反向旋转钻头，将食物推出容器。钻头由一个小型步进电机驱动，该电机通过一个由硅酮密封帽制成的简易联轴器连接到钻头上！

控制系统是一个 Arduino 和一个步进电机驱动芯片。通过反复试验,[Brian]发现 100，000 个半步的马达可以将大量的食物倒入水箱。钻头输送方法甚至可以很好地喷洒食物，让鱼尽情享受。为了保持食物定期流动，交流计时器单元控制 Arduino 通电的频率，并随后喂鱼。

[https://www.youtube.com/embed/eHGbhNHhfpI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&start=51&wmode=transparent](https://www.youtube.com/embed/eHGbhNHhfpI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&start=51&wmode=transparent)