# 公寓入口莫尔斯电码锁

> 原文：<https://hackaday.com/2012/04/09/apartment-entry-morse-code-lock/>

[Bozar88]住在一栋公寓大楼里，它的前门有一个蜂鸣器。客人在门旁边的面板上找到你的名字，按下按钮就可以在每个公寓单元的入口打电话。他决定增加一个莫尔斯电码密码来扩展内置功能，这个密码可以自动打开安全入口 ( [翻译为](http://translate.google.com/translate?sl=auto&tl=en&js=n&prev=_t&hl=en&ie=UTF-8&layout=2&eotf=1&u=http%3A%2F%2Fwww.elektroda.pl%2Frtvforum%2Fviewtopic.php%3Ft%3D2262211))。

他设计了一个电路，并蚀刻了自己的电路板，非常适合安装在壁挂式电话内部。它使用 ATtiny2313 来实现编码功能。该设备连接到内部通信线路，以便检测来自入口面板的输入按钮按压。这里有一些保护措施，使信号保持在 5V 或 5V 以下。输出是双重的。微控制器可以使用晶体管驱动麦克风线路，当输入代码时，它会向用户提供音频反馈。为了打开门，opt 隔离的三端双向可控硅开关元件(全部在一个封装中)进行连接，以启动入口门上的电子锁扣。

休息后的视频不是英文的，但仍然很容易理解正在演示的内容。

[https://www.youtube.com/embed/CUYceXnb_zY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/CUYceXnb_zY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[感谢 RicoElectrico]