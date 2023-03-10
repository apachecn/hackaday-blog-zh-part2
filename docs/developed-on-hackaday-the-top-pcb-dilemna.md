# 开发于 Hackaday:顶级 PCB 困境

> 原文：<https://hackaday.com/2014/04/12/developed-on-hackaday-the-top-pcb-dilemna/>

[![](img/7c2f20e4c61a7e73f6b61782649efd4c.png)](http://hackaday.com/wp-content/uploads/2014/04/olivier_mockup2.png)

黑客社区[离线密码保管员](https://github.com/limpkin/mooltipass)正在慢慢走到一起。几天前，我们收到了 Olivier 设计的顶级 PCB(如上所示)。如果你看下面的图片，你可能会看到我们打开包装时发现的问题:阻焊膜的颜色不对！考虑到板子应该放在有色丙烯酸面板后面，这是一个相当大的问题…

[![](img/9a669b1e5f5076d58f33a02b8e97d5ee.png)](http://hackaday.com/wp-content/uploads/2014/04/p1050601.jpg)

在使用了一些喷漆之后，我们设法到达了图片左下方所示的点。下一个任务是找到用反向安装 led 照亮输入接口的最佳方式。我们使用数控铣床加工开口(右上 PCB ),但也去除了 PCB 两侧的一些环氧树脂，认为这将提供更好的光漫射。然后，我们编写了部分 Mooltipass PWM 代码，并拍摄了这些图片:

[![](img/441f360a85e3dee13b010ef14806ee25.png) ](http://hackaday.com/wp-content/uploads/2014/04/p1050618.jpg) *使用 FR4 来漫射光线*

[![](img/c733065d98216e20caabc70d2201760a.png) ](http://hackaday.com/wp-content/uploads/2014/04/p1050623.jpg) *凿通开口*

我们希望你同意“FR4 版本”看起来更好。另一个有切口的版本照明不均匀，因为智能卡不在所有发光二极管的下面。这提出了几个问题，我们希望我们亲爱的 Hackaday 读者能够回答:

1.  这种加工可以在标准 PCB 工厂中进行吗？
2.  我们是否应该用白色阻焊膜覆盖 FR4，而不是将裸露的 FR4 留在顶部？
3.  我们是否应该用白色丝网覆盖 FR4，而不是将裸露的 FR4 留在顶部？

请记住，我们只需要加工 PCB 的一面。

另一个问题是顶板。如前所述，我们目前使用的是有色丙烯酸面板，这可能不是防止划痕的最佳解决方案。我们在考虑未来使用玻璃(康宁大猩猩玻璃？)所以我们也可以隐藏显示器活动区域周围的一切。你们有这方面的经验吗？相对少量的话会很贵吗？

正如你所看到的，我们仍然需要找到最好的妥协，我们希望你能帮助我们。请在下面的评论区发布快速消息或联系官方 [Mooltipass Google Group](https://groups.google.com/forum/?hl=en#!forum/mooltipass) 中的团队。