# WiFi 灯挑战–5 小时极速跑

> 原文：<https://hackaday.com/2014/12/24/wifi-lamp-challenge-5-hour-speedrun/>

“我们希望尽快完成，而不是马上。”

【CNLohr】最喜欢的台灯坏了，于是他给自己一个挑战:5 小时内把灯换成 LED 并[通过 WiFi](http://www.youtube.com/watch?v=oh4ZDkBHFYM) 控制，从零开始。他对整个过程进行了视频录制和叙述，并很好地解释了过程中的棘手部分和失败，让我们快速浏览了慢的部分。

一些零碎的东西简单而明显:挖出旧灯泡，连接一些发光二极管，添加几个功率电阻，为发光二极管添加一个“像显示器或其他东西一样，不要在意”的电源，为逻辑添加一个看起来像 LM2596 可调电源的东西，某种 ATMega，新的 ESP8266 (Wi07C)，拼接电源线等。标准的东西。

对于倾向于从烙铁和螺丝刀开始的读者来说，该视频展示了设计电子项目的更难部分:在软件中创建 PCB(他使用了 [KiCad](http://www.kicad.org) )，通过光刻将电路转移到 PCB，铋焊膏&填充电路板，以及[在 Github](http://github.com/cnlohr/wi07clight) 上编写和记录他的代码。也许最令人放心的是，他还展示了每一个贪婪的捷径的后果以及围绕它们的故障排除过程。

如果你曾经试图遵循烹饪节目的食谱，并注意到当一切都事先经过测量和准备时，这看起来是多么容易——然后当你尝试它时，它是多么的灾难——这里也揭示了同样的情况。总的来说，这是一个非常全面的演示，展示了设计一个项目实际需要什么，而不仅仅是完美的电路和要遵循的完美步骤。

最后，他在最后一刻完成了任务，因为他不会加法，所以晚了一个小时。够近了。

[https://www.youtube.com/embed/oh4ZDkBHFYM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/oh4ZDkBHFYM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

谢谢你的提示。