# 台式电源恒流 EZ-SET

> 原文：<https://hackaday.com/2014/03/05/bench-power-supply-constant-current-ez-set/>

[![constant_current_mod3](img/e5783df773662f5b54ad730d3ec89af2.png)](http://hackaday.com/wp-content/uploads/2014/03/constant_current_mod3.jpg)

这里有一个很好的技巧，如果你有一个更便宜的支持恒流限流保护(CC 模式)的台式电源，并且设置或检查最大电流限制的唯一方法是断开电路，短路电源输出，然后检查或设置你的限制，你可能会发现非常有用。是啊，真痛苦！[Ian Johnson]用几个电路专家的台式电源忍受着这种痛苦，并决定做点什么。在找到他的 CSI3003X-5 电源的电路图下载后，他能够反向工程一个[黑客，让你按下一个新按钮，拨入最大电流设置](http://www.ianjohnston.com/index.php?option=com_content&view=article&id=95)。你的第一个猜测是，他只是添加了一个瞬时按钮来短路电源输出，但你错了。[Ian]的解决方案不需要您移除负载，此外，当您设置电流限制时，负载可以继续运行。为此，他将电流显示读数从输出分流电阻的 0-3 伏切换到数字电位计的 0-3 伏输出，该电位计通常用于设置电源的恒流限制。如此简单，令人困惑的是为什么设计师没有包括这个功能。

虽然这是一个任何人都可以实现的简单修改，但是[Ian]仍然不高兴。[Gerry Sweeney]的评论使他走上了通过实现 555 瞬时信号将电路从电流负载读数切换到电流设置读数来消除繁琐的多按钮按压的道路。此第二模式意味着您只需开始按下上下 CC 设置按钮，它会立即切换显示以读取您选择的最大电流，几分钟后，显示会切换回读取实际负载电流。太棒了。就像昂贵的大男孩玩具一样。

[Ian]也不会止步于简单的一次性黑客工作。他设计了一个带有布线和连接器的适当 PCB，制作了一个易于安装的套件，几乎是电路专家台式电源(CSI3003X-5、CSI3005X5、CSI3003X3、CSI3005XIII)的插件转换套件。这不是一个 100%的插件套件，因为你必须将 3 根电线焊接到现有的信号和接地电路点上，但涵盖这项任务的视频似乎微不足道。

这种黑客可以很好地与市场上的许多其他电源工作，因为电路专家只是重新标记这些单元。目前，只有在休息之后列出的模型是已知的工作与这个黑客。如果你发现其他人，请在评论中列出。

休息之后，我们将链接到所有三个渐进式修改视频，以防你想学习如何修改自己的电源，或者你可以从[Ian]订购一个预建套件。

增加空载恒流设置。

[https://www.youtube.com/embed/ajfQF3cOm-E?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/ajfQF3cOm-E?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

用 555 芯片和继电器替换前面板按钮开关

[https://www.youtube.com/embed/Y3rjHu_1jg0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/Y3rjHu_1jg0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

用于 CC 改造的新 pcb。

[https://www.youtube.com/embed/xyunCIWkHjQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/xyunCIWkHjQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

单变量输出 0-30VDC 0-3A 台式电源 [#CSI3003X-5](http://www.circuitspecialists.com/bench-top-power-supply-csi3003x-5.html) 单变量输出 0-30VDC 0-5A 台式电源 [#CSI3005X5](http://www.circuitspecialists.com/dc-bench-power-supply-csi3005x5.html) 双变量输出 0-30VDC 0-3A 台式电源 [#CSI3003X3](http://www.circuitspecialists.com/bench-power-supply-csi3003x3.html) 双变量输出 0-30VDC 0-5A 台式电源 [#CSI3005XIII](http://www.circuitspecialists.com/bench-power-supply-csi3005xiii.html)