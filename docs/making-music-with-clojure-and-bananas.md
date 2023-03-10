# 用 Clojure 和香蕉做音乐

> 原文：<https://hackaday.com/2015/04/27/making-music-with-clojure-and-bananas/>

在这一点上，香蕉钢琴是一个非常经典的黑客。香蕉变成了一个便宜的彩色触摸传感器，看起来有点像钢琴键。Arduino 将引脚设置为低电平输出，然后用上拉电阻将引脚设置为输入。引脚从 0 翻转到 1 所需的时间决定了传感器是否被触摸。

[Stian]对香蕉钢琴采取了一种新的方法，将它与 Clojure 和 Overtone 联系起来。 [Clojure](http://en.wikipedia.org/wiki/Clojure) 是运行在 Java 虚拟机上的 Lisp 的一种方言。 [Overtone](http://overtone.github.io/) 是一个 Clojure 库，提供了大量的音乐制作工具。

泛音充当[超级对撞机](http://supercollider.github.io/)合成服务器的客户端。Supercollider 自 1996 年问世以来，提供了广泛的声音合成功能。Overtone 只是告诉 Supercollider 该做什么，让您轻松地在 Clojure 中编写声音。

香蕉钢琴充当 Clojure 程序的输入。这个程序将香蕉映射到一个音符，然后触发 Overtone 内置的钢琴采样器上的一个音符。结果是用水果演奏出美妙的钢琴声。当然，由于泛音和超级对撞机非常灵活，这可以用于更复杂的事情。

休息之后，香蕉钢琴演奏一些“瑞典爵士乐”的视频

[https://www.youtube.com/embed/EOjGsdDoicw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/EOjGsdDoicw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)