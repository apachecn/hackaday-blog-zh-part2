# 一个带电子表的网络速度计

> 原文：<https://hackaday.com/2015/07/30/an-internet-speedometer-with-a-dekatron/>

[Sprite_tm]和我们大多数人一样，对更早的计数和控制电子的方式很着迷。在一次黑客大会上，他发现一个旧的迪卡龙电子管与一个简单的旋转电路相连。对这种霓虹迷恋的处方是用一个迪卡龙做点什么，但是再做一个旋转电路就太可惜了。相反，他决定做一些有用的事情，并最终用这个老式显示管建造了一个互联网速度表。

像所有古董电子管一样，迪卡龙需要大约 400 伏的电压才能发光。在谷歌搜索了一下之后，[Sprite]发现了一个在升压转换器的帮助下驱动带 AVR 的 Dekatron 的项目。借用用微控制器控制升压转换器的想法，[Sprite]用互联网上最受欢迎的物联网东西 ESP8266 构建了一个电路，只需要一个 12 伏的壁式电源和少量部件。

控制迪卡龙的旋转发光仅仅是建造的一半；这个设备也是一个互联网速度计。为了读出他的网速，[Sprite]正在使用一个可管理的交换机，该交换机允许[SNMP](https://en.wikipedia.org/wiki/Simple_Network_Management_Protocol)读取网络接口上输入和输出的八位字节数。通过为 ESP8266 编写一个简单的 SNMP 客户端，该设备可以读取进出管道的堵塞程度。

随着一个丙烯酸案件新鲜出炉的激光切割机和一个非常好的工作弯曲丙烯酸与热风枪，[雪碧]有一个微小的设备，告诉他有多少互联网，他目前正在使用。他有一个它运行速度测试的视频，你可以查看下面的视频。

[https://www.youtube.com/embed/MxaG1fdYVN8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/MxaG1fdYVN8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)