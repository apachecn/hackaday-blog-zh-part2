# 测量乐高的寿命

> 原文：<https://hackaday.com/2013/04/19/measuring-the-lifespan-of-lego/>

![lifespan-of-LEGO](img/43024a9038bff24604733141d8be3171.png)

有多少次你可以把两块乐高拼在一起，然后在它们用坏之前再把它们拆开？答案是 37112。至少这是一个测试案例确定的数字。[Phillipe Cantin]对这个奇怪的问题很感兴趣，所以他建造了上面的测试装置来测量乐高的寿命。

组装在一起的设备相当精巧。它使用两个伺服电机进行测试，每个电机都由 Arduino 驱动，Arduino 正在记录 SD 卡上的计数。两个白色乐高零件中的一个被拧到了上层伺服系统的一个臂上。那个伺服系统向下压在黄色带子里面的配对零件上。仔细看，你会发现黄色是集成电路拉具的手柄端。当下伺服机构上的支柱向拉具的一个臂移动时，它会紧紧地抓住下乐高积木，这样上伺服机构就可以将两者分开。除了组装和拆卸步骤之外，还有一个验证步骤，即提升配对零件，以便反射传感器可以验证它们是否结合在一起。[Phillipe]在零件损坏之前，让设备连续运行十天。

不要错过他在休息后对项目的视频描述。

[https://www.youtube.com/embed/Tnb-LUM0yd4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/Tnb-LUM0yd4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[via [Reddit](http://www.reddit.com/r/arduino/comments/1cehuy/arduino_used_to_determine_usable_lifespan_of_legos/)