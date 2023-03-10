# 开源，DIY 焊接机器人

> 原文：<https://hackaday.com/2015/05/05/open-source-diy-soldering-robot/>

在[Brian]开始销售自己的 Raspberry Pi 扩展板后，他发现自己需要一个可以为他焊接 40 引脚接头的机器人。他首先做了大多数人可能会做的事情，查找预先构建的解决方案。不幸的是，他找到的所有东西要么太慢，要么太大，要么和一辆新车一样贵。就在那时，他决定建造自己的焊接机器人。

这个机器人看起来与我们过去见过的许多 3D 打印机设计相似，只是做了一些调整。印刷电路板被安装在一块被称为“印刷电路板盒”的扁平铝片上。印刷电路板安装有定制的引脚，这些引脚穿入盒中。一旦 PCB 就位，就用另一小块铝片将其夹住。一台计算机缓慢地向一个方向移动盒子，沿着烙铁的路径一次一排地移动接头的针脚。

该机器配有两个烙铁，允许同时焊接两个引脚。当 PCB 盒滑动到位时，熨斗缩回。然后将熨斗放在针上加热。然后，两台挤压机将适量的焊料挤压到每个引脚上。焊料在接触热引脚时熔化，就像用手焊接一样。

该系统最初被设计为在 Windows 8.1 平板电脑上运行，但[Brian]发现该系统的内部电池在充当 USB 主机的同时不会充电。相反，他们在完整的 PC 上运行 Windows WPF 应用程序。所有的软件和 CAD 文件都可以在[Brian 的] [github](https://github.com/briandorey/Soldering-Robot-Project "github") 页面找到。另外，请务必查看下面的演示视频。

[https://www.youtube.com/embed/i9pd9sY0Tjg?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/i9pd9sY0Tjg?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[谢谢拉斯姆斯]