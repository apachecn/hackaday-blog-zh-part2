# 咖啡壶的精确温度控制

> 原文：<https://hackaday.com/2013/09/02/precise-temperature-control-of-a-coffee-urn/>

![coffee-urn-temperature-controller](img/71610eead6fbd22d2db267b057cc5372.png)

Hackaday 校友[Nick Schulze]决定帮助一位朋友，他需要一个控制器将水保持在精确的温度。全世界狂饮咖啡的黑客应该感到高兴，因为[Nick]瞄准了一个咖啡壶作为该项目的容器。他想出的是[几块定制板和一个自己卷起来的温度探头](http://hownottoengineer.com/projects/fuzzy-urn.html)，它在调节液体温度方面做得非常好。

由于需要切换加热元件的电源，他立即想到了基于三端双向可控硅开关的交流斩波电路。没有立即想到的是需要检测过零事件。在上图中，你可以看到离骨灰盒最近的高压电板。下面是过零检测器电路。为了获得反馈，他使用 TC1047 温度传感器制作了自己的温度探头。在焊接上一个过滤帽和引线后，他将它浸入 JB 焊缝中以使其防水。如果你用它来煮咖啡，我们建议你寻找一种食品安全探针。

测试成功后，他添加了一个用户界面，并在下面的视频中看到的外壳上扣好。

[https://www.youtube.com/embed/CbBa9eyjocI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/CbBa9eyjocI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

![Fry](img/b653cd5e208a76a4e4f4fefb5587ffe6.png)