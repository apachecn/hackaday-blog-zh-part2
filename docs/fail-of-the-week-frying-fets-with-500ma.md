# 本周失败:用 500 毫安油炸羊乳酪

> 原文：<https://hackaday.com/2014/01/09/fail-of-the-week-frying-fets-with-500ma/>

![fotw-mosfet-smoke-at-500ma](img/5e0a7bc7d0ae0fde47c32a350b50e396.png)

当[Simon]仅用 500mA 电流就烧坏了他的 3A 额定 FET 时，他将其归咎于 SOT23 封装在没有散热器的情况下无法散热。在项目的下一次迭代中，他升级到了 12A 额定器件。幸运的是，他决定在将电路板送去 fab 之前再测试一次电路。他拼凑了这个恒流负载测试，这让他发现了自己的失败之处。

这个开关电路是为他的家庭安全系统项目设计的，我们已经看过至少两次了，在 500 毫安的电流下工作正常。但是当他把车开到了门槛以上时，包裹很快就热起来了。它变得如此之热，它实际上回流其焊点！问题与振荡有关，但即使进一步测试，他也无法让 FET 一直可靠地关断。看看他在顶部链接的失败报告，然后让我们知道一些可能的补救措施。

* * *

**[![2013-09-05-Hackaday-Fail-tips-tile](img/4ddcb45ba24697ecb36e5a2da073e8dc.png)](mailto:tips@hackaday.com?Subject=[Fail of the Week]) 每周失败是一个每周三运行的黑客专栏。通过写下你过去的失败和[给我们发送一个故事的链接](mailto:tips@hackaday.com?Subject=[Fail of the Week])，或者发送你在互联网旅行中发现的失败报道的链接，来帮助保持乐趣。**