# 自动寻找闪亮的口袋妖怪

> 原文：<https://hackaday.com/2013/11/05/finding-shiny-pokemon-automatically/>

如果你不熟悉口袋妖怪的世界，这个游戏中几乎每个物种都有一个“闪亮”的品种——每个口袋妖怪都有不同颜色的精灵。就游戏性而言，它们和不发光的同类完全一样，但发光的品种非常罕见，没有多少玩家见过它们。Youtube 上的[dekuNukem]想出了一个很好的方法来自动找到这些闪亮的口袋妖怪,使用 Hackaday 读者最喜欢的工具——一个 Arduino 和 Sparkfun 的一些部件。

这个版本的关键在于，每当玩家在野外遇到闪亮的口袋妖怪时，它们都会有一个简短的动画。这种设置使用鱼竿，因此 Arduino Micro 首先按下 Y 按钮来投掷鱼竿，而' duinos ADC 则监听音频信号，直到指示有鱼上钩。

3DS 底部屏幕上贴着一个光传感器，然后测量屏幕熄灭的时间。每一个闪亮的口袋妖怪的额外动画意味着这个黑暗期大约延长了半秒钟。如果 Arduino 没有看到亮晶晶的东西，它就会“逃跑”，但如果检测到亮晶晶的东西，蜂鸣器就会响起，告诉极其懒惰的口袋妖怪训练员他们的线上有亮晶晶的东西。

从视频来看，找到一个闪亮的口袋妖怪需要大约 36 分钟，在三个小时的测试中大约有 8 个闪亮的口袋妖怪。

[https://www.youtube.com/embed/moBGHUfw-Ho?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/moBGHUfw-Ho?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)