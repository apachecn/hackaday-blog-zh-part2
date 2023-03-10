# 用冷气操纵高空火箭

> 原文：<https://hackaday.com/2015/06/20/steering-high-altitude-rockets-with-cold-gas/>

业余火箭研究已经流行了很长时间，设计范围从小型玩具比例模型火箭到带有可操纵尾翼的大型液体燃料设计。波特兰州立大学的一个团队正在研究一些大型的业余火箭，这些火箭可以飞到很高的高度。由于火箭飞得越远，大气层就越稀薄，一旦火箭到达高空，导向鳍就不那么有效了。一组学生解决了这个问题，他们设计了一个冷气反应模块来控制高空火箭。

该小组选择氮气作为他们的冷气推进剂，储存在碳纤维罐中。通过调节器后，气体被输送到几个气体螺线管，然后到达一个定制的 3d 打印的[德拉瓦尔喷嘴](https://en.wikipedia.org/wiki/De_Laval_nozzle)。英特尔 Edison 用于驱动系统，该系统使用 MPU-6050 计算火箭的方向。控制回路利用方位信息，通过几个喷嘴口中的任何一个喷射燃气来操纵火箭。

该系统确实有一些限制:螺线管不是开就是关，不可变，并且它们不是非常快。即使有这些限制，该团队仍然相信，明年他们的模块将在一个全新的定制火箭中进行首次飞行。这个团队也很棒，他们把所有的设计文件都开源了，这样你就可以自己构建了(尽管他们警告说这有点复杂和危险)。休息后，请观看视频，了解冷气体反应系统的试运行。

谢谢你的提示，[内森]！

[https://www.youtube.com/embed/2UBRPR6j1LQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/2UBRPR6j1LQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)