# Thinkpad 701c:逆向工程的复古处理器升级

> 原文：<https://hackaday.com/2014/10/21/thinkpad-701c-reverse-engineering-a-retro-processor-upgrade/>

[Noq2]给了他的蝴蝶新翅膀一个升级的 CPU。很少有笔记本电脑像 IBM Thinkpad 701 系列及其[“蝴蝶”轨迹键盘](http://en.wikipedia.org/wiki/IBM_ThinkPad_Butterfly_keyboard)一样具有标志性。事实上，它如此具有标志性，以至于 701c 成为了纽约现代艺术博物馆的[永久收藏的一部分。](http://www.moma.org/collection/object.php?object_id=2168)

作为一款 1995 年的老式笔记本电脑，[noq 2]701 c 以今天的标准来看并不是速度恶魔，这是可以理解的。最快的工厂配置是运行在 75 MHz 的 Intel 486-DX4。然而，长期以来一直有传言和网上拍卖涉及一个定制模型的修改，以运行 133 MHz 的 AMD AM-5×86。这些改装是由德国的汉茨+合作伙伴这样的商店完成的。考虑到这一点，[Noq2]开始对改装进行逆向工程，并为他的 701c 配备了新的处理器。

![thinkpad-brainsurgery](img/4bc405449d129bd897835589b5459bb9.png)第一步是确定使用哪种 AMD 处理器。事实证明，只有少数型号的 AMD 芯片与 701c 主板上的 208 引脚小型四方扁平封装(SQFP)引脚兼容。[Noq2]能够从每个人都喜欢的拍卖网站上的旧 Evergreen 486 升级模块中获得一个。他小心翼翼地将 AM-5×86 从模块上拆下，将 Intel DX4 从 701c 上拆下。稍加焊接之后，大脑移植就完成了。

一些详细的数据手册研究帮助[noq2]找到了如何提高他的 5×86 芯片的总线时钟，并启用回写高速缓存。他所要做的就是移动几个无源元件，短接处理器上的几个引脚。

最终的结果是一个精心设计的 IBM 701c Thinkpad 运行 AMD 5×86 处理器，频率为 133 MHz。对今天的软件来说还是太慢了——但绝对是我们很久以来见过的最酷的复古模式。