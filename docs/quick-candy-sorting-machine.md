# 糖果快速分拣机

> 原文：<https://hackaday.com/2013/12/21/quick-candy-sorting-machine/>

强迫症。有时候事情会影响到你，就像那些讨厌的随机包装的糖果。[Torsten]决定建造一台分选机[，能够以每分钟 80 件左右的速度将彩虹糖或 M & Ms](http://beta.ivc.no/wiki/index.php/Skittles_M&M%27s_Sorting_Machine) 按颜色分拣到不同的杯子中。这是一个很好的实现，使用 Arduino Duo。他根据[有限状态机](http://en.wikipedia.org/wiki/Finite-state_machine)的原理编写代码，目的是让它尽可能快。

它的工作原理和你预期的一样:当一个糖果被装入时，颜色是由一个 RGB 传感器决定的。一个 360 度的伺服系统用于将滑槽移动到合适的位置，有趣的是，为了最大化速度，系统在滑槽到位之前先发制人地释放糖果。如果你仔细观察，可以在视频中看到这种行为(插播在休息之后)。

[Torsten]包括一份完整的材料清单，如果您想亲自尝试的话。他还列出了可能的改进。

[https://www.youtube.com/embed/H7HTQai7Wwg?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/H7HTQai7Wwg?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)