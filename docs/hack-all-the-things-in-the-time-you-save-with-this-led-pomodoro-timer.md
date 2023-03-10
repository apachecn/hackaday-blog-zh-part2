# 用这款 LED 番茄计时器，在你节省的时间内搞定所有事情

> 原文：<https://hackaday.com/2014/02/09/hack-all-the-things-in-the-time-you-save-with-this-led-pomodoro-timer/>

你想更有效地利用你的时间，但又不喜欢吃西红柿吗？[罗宾]的 [LED 番茄定时器](http://robinscheibler.org/2014/02/04/pomodoro-timer/)可能是你的完美选择。

[番茄工作法](http://pomodorotechnique.com/)是 20 世纪 80 年代末开发的一种时间管理解决方案。基本的想法是花 25 分钟进行一些活动，比如工作或学习，然后休息 5 分钟。它的许多支持者使用一个西红柿形状的厨房定时器来提醒他们在两种状态之间切换，但[Robin]想自己制作一个，并在过程中学习。

首先，他想使用 ATtiny85 并了解它的特性。具体来说，他使用了它的定时器、PWM 和低功耗睡眠模式。[Robin]使用了 [Charlieplexing](https://en.wikipedia.org/wiki/Charlieplexing) 来驱动总共六个 led。当计时器启动时，五个黄色发光二极管被驱动到高电平，以指示每 5 分钟的工作时间。在 5 分钟的休息时间里，一个红色的 LED 灯亮起。

[Robin]还探索了紧凑型 PCB 设计和制造。所有元件都是 SMD，他的板是 4cm 见方。[Robin]正在使用[这个 SMD 蜂鸣器](http://www.mouser.com/ProductDetail/Kobitone/254-PB501-ROX/?qs=%2fha2pyFaduio21Wb3%2fEgDw7Itv2u2RCUk%252bCSGDldQmgXvX6wRiKaqw%3d%3d)进行离散反馈。他包括了一个六引脚 ISP 接头的封装，并用弹簧针对其进行了编程。定时器是完全中断驱动的:一次点击触觉按钮启动工作计数器，当时间到了蜂鸣器响起。第二次点击启动中断计数器。

[Robin]在他的 GitHub repo 中提供了所有可用的东西，并鼓励你使用它。时间在浪费！