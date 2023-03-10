# 起来，站起来。在正念手环的帮助下

> 原文：<https://hackaday.com/2015/06/16/get-up-stand-up-with-a-little-help-from-the-mindfulness-bracelet/>

[Becky Stern]创造了[正念手环](https://learn.adafruit.com/buzzing-mindfulness-bracelet)，这是一款看起来很棒的可穿戴设备，有着重要的用途。手环每小时都会发出嗡嗡声，提醒你站起来，从工作、焊接、游戏或任何你可能正在做的事情中休息一下。这款手镯由皮革制成的 8 字形相互连接而成，不过[贝基]说自行车内胎的橡胶也很好用。最终的形状让我们想起有时在车床或其他工业设备上发现的链带。这些链接的大小非常适合放入 Arduino Gemma，以及电池和振动电机。NPN 晶体管、二极管和电阻构成了该设计的整个材料清单。这款手环比激发它的 Apple watch 功能便宜多了！

代码中的时间间隔设置为 1 小时，用户可以调整。虽然时间以毫秒为单位存储，但该设计确实使用了 ATtiny85 的看门狗定时器(WDT)来省电。这意味着时间可以漂移到每小时 30 秒，这在这个应用中是没问题的。

点击突破，看看手镯的行动！

[https://www.youtube.com/embed/DJfGhETxWlw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/DJfGhETxWlw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)