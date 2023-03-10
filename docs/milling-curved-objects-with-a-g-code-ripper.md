# 用 g 代码开膛手铣削弯曲物体

> 原文：<https://hackaday.com/2014/07/31/milling-curved-objects-with-a-g-code-ripper/>

![HaD Mouse](img/3e88bc5b881a1449b19b13a809cc3aaa.png)

铣削和刨平平面是 CNC 刨槽机的重点，但是曲面呢？业余爱好数控机床和 3D 打印机的自动调平变得越来越普遍，但 Scorch Works 正在做相反的事情:[使用数控机床上的探针触摸探针将 g 代码](http://www.scorchworks.com/Blog/auto-probing-with-g-code-ripper/)文件转换成可以在曲面上铣削的东西。

该技术几乎与[自调匀整器](http://www.autoleveller.co.uk/cnc-probe-guide/)完全相反，后者是使用 MACH3 或 LinuxCNC 机床铣削和传送不完全平坦或垂直于床身的物体的首选工具。在这种情况下，连接到刳刨机的接触式探针扫描弯曲零件，对 g 代码文件应用双线性插值，然后开始加工。

探头可以用在任何东西上——在下面的视频中，你可以看到一块垂直于床大约 30 度的塑料上的完美雕刻，棒球棒上的字母雕刻，以及保证让你的项目在 Hackaday 上出现的方法。

[https://www.youtube.com/embed/dzX0JXX5iCc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/dzX0JXX5iCc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[https://www.youtube.com/embed/vjOMwEOcJbQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/vjOMwEOcJbQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)