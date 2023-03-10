# MSP430 的低功耗方向跟踪器和优化的数学库

> 原文：<https://hackaday.com/2014/04/18/low-power-orientation-tracker-and-an-optimized-math-library-for-the-msp430/>

![MSP430 Orientation Tracker](img/da707688db4340663cbba7b7a0ad5e4d.png)

方位追踪器可以用于许多不同的应用:追踪误处理的包裹、贵重物品失窃通知和导航只是几个例子！德州仪器(ti)最近的一篇博客文章讨论了如何利用 MSP430 构建一个[低成本、低功耗的方位跟踪器](http://e2e.ti.com/blogs_/b/msp430blog/archive/2014/03/25/low-power-orientation-tracker-enabled-by-iqmathlib.aspx)。

基于 [MSP430 发射台](http://www.ti.com/ww/en/launchpad/launchpad.html)和 [CircuitCo 的教育助推器包](http://www.boosterpackdepot.com/educationalboosterpack.html)，方位追踪器组装起来非常简单。它也可以通过使用任何带有[油箱助推器](http://www.ti.com/tool/boostxl-battpack)的[无线助推器](http://www.ti.com/ww/en/launchpad/boosterpacks.html)，或者通过使用带有内置锂电池电路的 [BLE 助推器](http://store.hardwarebreakout.com/index.php?route=product/product&product_id=65)来实现无线。TI 在其参考应用程序中提供了所有必要的代码和设计文件,用于启动和运行您的方位跟踪器。休息之后，请务必观看设备的运行情况！该项目不仅涉及构建低功耗方向跟踪器，还展示了 MSP430 上的优化定点数学函数库 [IQmathLib](http://www.ti.com/tool/msp430-iqmathlib) 。使用 MSP430 或 Arduino 等小型 MCU 的一个更具挑战性的方面是内置数学库的效率有多低。查看 IQmathLib，它大大改进了 MSP430 的内置数学函数。

看到这个项目被修改成一个 DIY 计步器或者用在自平衡机器人上会很有趣。将 IQmathLib 移植到其他微处理器上也会很有趣，比如 Arduino。看看如何在自己的项目中使用这种参考设计！

[https://www.youtube.com/embed/awptY1q7fvI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/awptY1q7fvI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)