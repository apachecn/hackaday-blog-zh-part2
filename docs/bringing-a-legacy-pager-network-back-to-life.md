# 让传统的寻呼机网络起死回生

> 原文：<https://hackaday.com/2014/12/30/bringing-a-legacy-pager-network-back-to-life/>

[Jelmer]最近在一次行动中发现了他的旧寻呼机，并决定启动它以重温他收到寻呼的美好回忆。他很快发现传呼机的号码不再有效，传呼机的网络完全关闭。为了让他的寻呼机起死回生，[Jelmer]建造了自己的[基于 OpenWRT 的寻呼机基站](http://jelmerbruijn.nl/pocsag-encoder/)，它模拟 POCSAG RF 寻呼机协议。

[杰尔默]打开他的传呼机，开始探测信号，以确定传呼机使用的协议。不久，他发现了实现 [POCSAG 寻呼机协议的射频接收器和解码器 IC。](http://en.wikipedia.org/wiki/POCSAG)【Jelmer】开始查阅稀疏的 POCSAG 文档，收集足够的信息来自己实现该协议。

[Jelmer]使用 HLK-RM04 WiFi 路由器模块作为他的大脑，它可以与控制 SI4432 射频收发器的 ATMega 对话。路由器运行 OpenWRT 并产生 POCSAG 控制信号，这些信号由 SI4432 IC 发送。[Jelmer]成功地使用该设置向他手头的几个寻呼机发送控制信号，并计划将来使用该设置发送可定制的警报。[Jelmer]确实注意到，在许多国家操作这种设备可能是非法的，所以一如既往，在处理这个项目之前，请检查当地的频率分配和法律。休息之后，请观看视频，其中寻呼机由[Jelmer]的发射机初始化。

[https://www.youtube.com/embed/lpLzPt_0Xtw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/lpLzPt_0Xtw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)