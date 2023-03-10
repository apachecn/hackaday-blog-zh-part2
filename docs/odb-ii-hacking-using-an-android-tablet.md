# 使用安卓平板电脑的 ODB-II 黑客攻击

> 原文：<https://hackaday.com/2013/04/28/odb-ii-hacking-using-an-android-tablet/>

在你汽车的数字仪表盘显示屏上读到的信息是多么奇怪啊。这证明[克里斯托佛·史密斯]能够在他的鹰牌大切诺基上控制 ODB-II 总线。

他这样做不仅仅是为了好玩。这源于他的目标:在仪表板上添加一个 Android 平板电脑，这在最近的已经成为一个流行的黑客。这使得[克里斯托弗]的方向盘控制失灵。他们最初操作无线电，所以他开始让他们控制平板电脑。

他曾见过一个 Arduino 用来控制 CAN 总线，但决定走一条不同的路线。他以 25 美元左右的价格抢到了一个 USB CAN 总线接口。第一件事就是用它和他的电脑一起嗅出可用的数据。从那里，他能够解码流量，并找出他需要监控的命令。难题的最后一部分是编写他自己的 Android 代码来监视方向盘按钮并对其做出反应。你可以在[他的仓库](https://github.com/theksmith/Steering-Wheel-Interface)查看代码，休息后再看演示。

[https://www.youtube.com/embed/iYj5OgHyrc0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/iYj5OgHyrc0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[感谢垫]