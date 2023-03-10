# 非偏光薄膜电容走哪条路？有一个答案。

> 原文：<https://hackaday.com/2012/12/19/which-way-do-non-polarized-film-capacitors-go-there-is-an-answer/>

![orienting-non-polarized-film-caps](img/7b0ad652e939f45f6bea08e2c6f98190.png)

如果你和我们一样，认为电容方向只对电解电容等极化品种有影响，那么你应该通读这篇文章。[Bruce Trump]研究了[为什么一些薄膜电容的一端印有条纹，以及为什么它们的方向很重要](http://e2e.ti.com/blogs_/b/thesignal/archive/2012/12/10/pcb-layout-tricks-striped-capacitors-and-more.aspx)。

他的帖子中有一张图片，显示了轴向和浸入式电容，封装的一端印有一条黑色条纹。这是组件内部情况的指示器。线路末端有一个导电箔层作为屏蔽层。不过，如果你能更好地设计电容，这种屏蔽似乎能更好地发挥作用。

上图显示了两个运算放大器电路，都使用了一个无极性电容，如果电路受到外部干扰，该电容会对电路产生影响。[Bruce]讨论了这一现象的各个方面，提到虽然这些精心布局可以在您的设计中进行测试，以证明哪一个更有好处，但模拟应用程序(使用 SPICE)的性能完全相同。