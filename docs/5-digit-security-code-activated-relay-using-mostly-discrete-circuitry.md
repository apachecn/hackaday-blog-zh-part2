# 5 位安全代码激活继电器，主要使用分立电路

> 原文：<https://hackaday.com/2013/10/01/5-digit-security-code-activated-relay-using-mostly-discrete-circuitry/>

[![alarm keypad](img/2538ecdd601c4e708d4111b56d3cd07d.png)](http://hackaday.com/wp-content/uploads/2013/09/alarm-keypad2.jpg)

让我们用[myvideoisonutube 的] [闹钟激活控制电路，使用矩阵风格的电话键盘](http://www.youtube.com/watch?v=laG_pGUpCKs)，让业余爱好电子日历倒退几十年。该电路是相当古老的使用 CMOS 4081 与 4 '和'门硬连线访问代码。[myvideisonutube]references[Ron ' s]"[增强型 5 位报警键盘](http://www.zen22142.zen.co.uk/ronj/k5.html)"此构建的示意图将推荐的键盘更改为触摸板电话中更常见的矩阵风格键盘。这些类型的矩阵键盘不能直接用于输入，所以他切断了一些线路并添加了连接线，将其转换成一个具有公共端子和独立连接按键的键盘。我们喜欢看到这样的黑客捐赠硬件，即使它需要大量的修改。[罗恩的] [源电路](http://www.zen22142.zen.co.uk/ronj/k5.html)包括一个简单到足以建立战术按钮键盘，如果你不能找到一个合适的捐赠手机。

学习如何使用大部分分立元件[而不是微控制器](http://hackaday.com/2013/09/05/custom-car-keypad-entry/)将是构建该电路的核心目标，而不需要键码接入点或其他安全的 12 V 继电器激活器件。这种装置非常安全，需要 4 个数字的“开”代码和 5 个数字的“关”代码。你也不能拔下键盘和热线或者短接什么东西来进入。“功能”上的 4 位数确实大大降低了安全性。然而，所有不在访问码中的键都连接到同一点，因此您可以使用带有更多键的 pad 来提高安全性。

在[Ron 的]网站上，您将找到一份详细的施工指南，包括 veroboard 上所有组件的俯视图和仰视图。休息之后加入我们观看[myvideoisonutube]演示他的版本。

[https://www.youtube.com/embed/laG_pGUpCKs?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/laG_pGUpCKs?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)