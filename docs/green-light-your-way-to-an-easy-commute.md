# 用美国不安全的交通灯为你的通勤开绿灯

> 原文：<https://hackaday.com/2014/08/31/green-light-your-way-to-an-easy-commute/>

还记得《杠杆作用》(第五季，第三集)的那一集吗，亚历克用马文用无线方式把所有的街灯换成绿色，这样他们就能赶上一辆 SUV 了？你嗤之以鼻，说“这太不真实了！”…事实上，他们是对的。密歇根大学 (PDF 警告)的一项[新研究显示，让你的早晨通勤一路绿灯是多么容易。](http://lab11.eecs.umich.edu/content/pubs/ghena14green_lights.pdf)

该研究指出，美国很大一部分交通灯都是通过 900Mhz 和 5.8 GHz ISM 频段进行无线通信，完全没有加密。为了连接到 5.8Ghz 交通信号，您只需要 SSID(设置为广播)和适当的协议。在这项研究中，研究人员使用了一种公众无法获得的无线网卡，但他们指出，通过一点社会工程，你可能会得到一张。另一个途径是 [HackRF SDR](http://hackaday.com/2013/08/01/hackrf-or-playing-from-30-mhz-to-6-ghz/) ，它可以用来监听和传输所需的协议。一旦连接到网络，您将需要默认的用户名和密码，这可以在交通灯制造商的网站上找到。要访问 900Mhz 网络，您需要上述所有设备和一个 16 位的从属 ID。这可能是蛮力造成的，正如研究显示的，没有 ID 大于 100。现在，您可以完全访问，不仅仅是一个交通信号，而是连接到网络的每个信号。

一旦进入网络，你有两个选择。在 [VxWorks 操作系统](http://wikipedia.org/wiki/VxWorks)中完全开放的调试端口允许你读-修改-写任何内存寄存器。或者通过发送(n) UDP 包，其中最后一个字节对控制器键盘上按下的按钮进行编码。使用遥控键盘，您可以冻结当前的路口状态，修改信号定时，或改变任何灯的状态。然而，硬件故障管理单元(MMU)仍将检测任何非法状态(相互冲突的绿灯或黄灯)，并接管熟悉的 4 路红灯闪烁。由于技术人员必须出来手动重置交通信号才能从非法状态中恢复，您可以将网络上的每个十字路口都变成 4 向停车点。

所以下一次你在红灯前停下来，并且看起来要花很长时间去改变，留意那些刚刚为他们的通勤开绿灯的黑客。

谢谢你的提示[马特]