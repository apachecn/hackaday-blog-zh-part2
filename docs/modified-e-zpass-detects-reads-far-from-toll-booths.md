# 改进的 E-ZPass 可以检测远离收费站的读数

> 原文：<https://hackaday.com/2013/09/16/modified-e-zpass-detects-reads-far-from-toll-booths/>

Def Con speaker [pukingmonkey]花了相当多的时间研究政府和执法部门用来跟踪路上私人车辆的方法。一种主要的追踪方法是 E-ZPass，这是一种在全国几个州使用的电子收费系统。【pukingmonkey】破解了他的 E-ZPass 标签，找到了一个相对基本的电路。在他的 DEF CON 演示文稿中，他指出你不应该对你自己的标签这样做，因为标签在法律上不是用户的财产。

该标签使用 3.6 伏长寿命电池工作。空闲时，标签仅消耗 8 微安。读取期间，电流消耗跃升至 0.3 mA。有了这些信息，添加一个在标签读取时输出脉冲的电流检测电路就相对简单了。然后，脉冲被输入一个玩具牛，每次读取时，玩具牛就会发光并“哞哞”叫。

随着赛道的完成，是时候在纽约市兜风了。在泰晤士广场和麦迪逊广场花园之间令人痛苦的车程中(这条路不收费)，奶牛被分 6 次挤奶。纽约交通部早就声明这些读数仅用于跟踪交通拥堵情况。即便如此，我们还是建议在不接近收费站时，将您的标签放在防静电袋(法拉第笼)中。

[https://www.youtube.com/embed/JCwWVxGtYgE?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/JCwWVxGtYgE?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[via [Boing Boing](http://boingboing.net/2013/09/13/hardware-hacker-learns-his-e-z.html)