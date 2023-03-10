# 在 Hackaday 上开发:Olivier 的设计纲要

> 原文：<https://hackaday.com/2014/04/15/developed-on-hackaday-oliviers-design-rundown/>

[![](img/9ca2ce62167e0663545e57ecac648a81.png)](http://hackaday.com/wp-content/uploads/2014/04/dev.png)

Hackaday 的作者和读者目前正在携手开发一个离线密码管理器，即 [Mooltipass](https://github.com/limpkin/mooltipass) 。几天前，我们展示了 Olivier 的设计前 PCB，甚至没有展示他创作的其他部分(我们太粗鲁了……)。我们还[向我们的读者](http://hackaday.com/2014/04/12/developed-on-hackaday-the-top-pcb-dilemna/)询问我们应该如何设计前面板。因此，在这篇新文章中，我们将向您展示这第一个(非最终)原型中不同的部分是如何组合在一起的…休息之后，请跟随我们！

[![](img/afced75ded184b5834e72ea16ea50772.png)](http://hackaday.com/wp-content/uploads/2014/04/p1050637.jpg)

这是底部的 PCB，包含主微控制器、Arduino 接头和有机发光二极管屏幕的 FPC 连接器。寻找低轮廓标准. 1”母接头是我们最长的谷歌搜索之一。上面可以看到的是直通连接器，也就是说管脚可以穿过 PCB。

[![](img/701130f25d4b09062c2ccd75b7f22f88.png)](http://hackaday.com/wp-content/uploads/2014/04/p1050644.jpg)

这是数控铣削的原型案例。在底部，您可能会注意到两个深度较小的插槽，位于 Arduino 连接器的正上方。正如我们之前在 Hackaday 文章中提到的[，我们希望给最终用户将他们的安全密码管理器转换成 Arduino 平台的能力。正如你可能已经猜到的那样，转换 Mooltipass 将像切割这层薄塑料层(见图片顶部)一样简单，以访问 Arduino 接头并解锁平台。](http://hackaday.com/tag/developed-on-hackaday/)

[![](img/1268b222bdae9e4ce24a5ea2105db866.png)](http://hackaday.com/wp-content/uploads/2014/04/p1050649.jpg)

这就是底部 PCB 如何装入外壳的方式。4 个螺丝可以用来固定所有东西。较大的凸起塑料区域用作智能卡的平坦表面:

[![](img/bd90f04acc988f9fd1b27a4da0c9207c.png)](http://hackaday.com/wp-content/uploads/2014/04/p1050650.jpg)

有机发光二极管屏幕位于表壳两侧:

[![](img/241bf1e94bba0c7375c0a668b40bd458.png)](http://hackaday.com/wp-content/uploads/2014/04/p10506541.jpg)

屏幕后面留有足够的空间，以便柔性 PCB 舒适地弯曲。最后，将顶板放入剩余的空间中，并将丙烯酸板放在组件的顶部:

[![](img/441f360a85e3dee13b010ef14806ee25.png)](http://hackaday.com/wp-content/uploads/2014/04/p1050618.jpg)

[正如我们上一篇文章所说的](http://hackaday.com/2014/04/12/developed-on-hackaday-the-top-pcb-dilemna/)，我们显然还有一些需要完善的地方。与此同时，我们将手工焊接一些原型，并将它们发送给当前的开发人员。

想要保持消息灵通？你可以加入官方的 [Mooltipass Google Group](https://groups.google.com/forum/?hl=en#!forum/mooltipass) 或者关注我们的[黑客项目](http://hackaday.io/project/86-Mooltipass)。