# Arduino 会在您的手机触摸屏上播放白色磁贴

> 原文：<https://hackaday.com/2014/12/23/arduino-plays-white-tiles-on-your-mobile-touchscreen/>

像许多手机游戏玩家一样，[Daniel]发现自己沉迷于令人上瘾的“白色瓷砖”游戏。虽然[丹尼尔]没有自己玩游戏，但他决定编写自己的自动白棋玩家。虽然这种攻击[以前也曾成功](https://www.youtube.com/watch?v=2TJ7itil1cc)，但从未被很好地记录下来。[Daniel]利用他在 Hackaday 和 Hackaday.io 上收集的知识来实现他的黑客技术。

最基本的问题是感知白色和黑色的瓷砖，并激活 iPad 的电容式触摸屏。在检测方面，[丹尼尔]本可以使用光电晶体管，但事实证明，简单的 CdS 电池或光敏电阻在这种应用中已经足够快了。事实证明，激活屏幕有点困难。[Daniel]最初尝试将铜带绑在晶体管上，但发现它们不能可靠地触发屏幕。他改用继电器，效果非常好。我们猜测，改变导线长度会导致足够大的电容变化，从而使屏幕检测到触摸。

最终的结果是一个巨大的成功，因为(丹尼尔的)Arduino 为基础的球员撕裂通过经典的游戏只有 3.9 秒！干得好[丹尼尔]！

点击休息时间观看[Daniel]的设备工作，并观看他解释其创作的视频。

[https://www.youtube.com/embed/QLNiDpJHrC4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/QLNiDpJHrC4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[https://www.youtube.com/embed/y8ZDLS0f_a8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/y8ZDLS0f_a8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)