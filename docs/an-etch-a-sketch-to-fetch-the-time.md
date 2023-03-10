# 一幅用来消磨时间的速写

> 原文：<https://hackaday.com/2014/03/28/an-etch-a-sketch-to-fetch-the-time/>

对于一个从未使用过步进电机、实时时钟或从零开始建造任何东西的人来说，[Dodgey99]在建造他的[蚀刻草图时钟](http://www.instructables.com/id/Arduino-Etch-A-Sketch-Clock/)时，已经做了一件很好的工作来使它们符合他的意愿。

他使用两个 5V 步进电机和 ULN2003 驱动器。这些电机安装在背面，通过滑轮旋转旋钮。它们有点慢；画出时间大约需要 2 . 5 分钟，但黑客的目的是观看蚀刻草图。[Dodgey99]正致力于用速度更快的 Nema 17 电机取代这些步进电机。[Dodgey99]为 Arduino 使用了一个 EasyDriver 来驱动它们。他在这个时钟中有一个 Arduino 芯片套件，以节省 BOM，但你可以使用普通的 Arduino。他省略了 5V 调节器，因为 EasyDriver 有一个。

[Dodgey99]已经发布了三个时钟草图:一个用于设置 RTC，以便在 Etch-A-Sketch 完成后显示正确的时间，一些用于测试硬件和采样数字外观的代码，以及用于替换测试代码的主代码。

这个计时蛋糕上的糖衣是他制作的丙烯酸底座和支架。在他的安装试验中，他学到了在草图上钻孔的宝贵一课。你不能以编程方式摇动蚀刻草图，所以他用 Nema 17 旋转它。跳完之后检查一下。

如果你注意的话，你会发现几个小时前我们刚刚看到了这个项目的完全相反的东西:[一个由旋转蚀刻草图旋钮](http://hackaday.com/2014/03/27/laser-cutter-becomes-an-etch-a-sketch/)控制的数控工具(激光切割机)。

[https://www.youtube.com/embed/XkKFoPMufoI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/XkKFoPMufoI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)