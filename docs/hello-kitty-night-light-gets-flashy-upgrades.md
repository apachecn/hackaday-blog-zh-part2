# 凯蒂猫小夜灯得到华丽的升级

> 原文：<https://hackaday.com/2014/11/20/hello-kitty-night-light-gets-flashy-upgrades/>

看到世界上一些糟糕的事情？作为一个具有黑客能力的人，你会把这种糟糕的事情视为一种挑战，以提出一种改进，在某些情况下，这种改进超出了真正必要的范围，但*只是很酷的*。这就是制造商和父亲(丹·麦克杜格尔)对他女儿的[灯光投影凯蒂猫枕头](http://imgur.com/gallery/lH5Qm)所做的。

作为一个只有一个目的，那就是在晚上在孩子的墙上照出明亮的星星图案的东西，这个枕头悲惨地失败了。[Dan]想知道为什么他女儿的玩具在吸干电池的同时不能达到合理的期望，所以他打开枕头中央的大型粉红色塑料外壳，找到一个相当小的电路板，驱动三个非常暗的 led。那些忽明忽暗产生不同颜色混合的发光二极管甚至也不是红色、绿色和蓝色的。玩具的制造商使用黄色，而不是稍贵的蓝色。没有这些，[丹]用一个 Arduino Pro Mini 取代了这些悲伤的内部零件，他编程驱动一个旧的抢救扬声器和三个从灯带末端借来的明亮的 RGB LEDs。对于不必要但很酷的部分，他使用 Arduino 微控制器的额外引脚在粉红色外壳的外部添加了四个触摸感应按钮。这些由铜带制成的小电容瓦片在被触摸时会激活声音并改变 led 的颜色，使枕头比以前更具反应性。

Arduino Mini 板和添加的组件在焊接完成后非常适合枕头的原始粉红色外壳。他女儿的 Hello Kitty 枕头有三倍高亮度的发光二极管和一个超级频闪模式，现在更像是一个迪斯科球，而不是一个小夜灯……但我们怀疑她会抱怨这些很酷的附加物。要了解枕头的使用情况，了解更多升级信息，请观看下面的[Dan]视频:

[https://www.youtube.com/embed/1gXsgdD21-4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/1gXsgdD21-4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)