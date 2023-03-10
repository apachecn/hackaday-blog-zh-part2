# 提高有效负载

> 原文：<https://hackaday.com/2015/05/03/improving-active-loads/>

[Texane]的工作需要在一组负载下测试几块电路板，尽管工作中的实验室有一些专业工具，但这似乎是一个尝试 Re:load 2 的好机会。这是一个小巧的有源负载，当然可以通过注入焊料和硅来改善。

虽然 Re:load 2 是一个漂亮、简单的设备，可以将高达 12 瓦的功率直接转化为热能，但它是不可编程的。创建和保存负载曲线的能力将是一个方便的功能，所以[Texane]采用了 Teensy 3.1 微控制器，并在 Re:load 的放大器前安装了电阻分压器。一个运行在计算机上的简单脚本允许[Texane]设置当前倾倒的数量，并自动斜坡和计时器。

Re:load 还有一个更基本的问题；可能流入散热器的最低电流为 90mA。[Texane]用零漂移放大器替换放大器，将 90mA 数字降至 7mA。

当然，Re:load 和 Teensy 3.1 在 Hackaday 商店出售[，但是如果你正在寻找一个现成的计算机控制的主动负载解决方案，你可以随时查看](http://store.hackaday.com/) [Re:load Pro](http://store.hackaday.com/collections/products-tools/products/re-load-pro) ，这是一个有液晶显示器的精美模型。专业版价格更高，而[Texane]只是告诉你如何用我们正在销售的较便宜的型号获得相同的功能，尽管…