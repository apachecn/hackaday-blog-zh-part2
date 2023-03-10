# 创新:核心竞争力

> 原文：<https://hackaday.com/2014/10/14/retrotechtacular-core-competencies/>

正如上面这位风度翩翩的官员会告诉你的那样，早期的数据处理机和 ADP 系统采用两种类型的磁芯用于存储和其他目的。这部 1961 年的美国陆军训练电影[介绍了铁氧体磁芯](http://www.youtube.com/watch?v=X0WnddW5gZI)的特性，铁氧体磁芯通常由镍合金和其他磁性材料制成。由于这只是一个系列的第一部分，金属带类型的磁芯是涵盖在一些其他部分，我们还没有找到。

将磁芯用于随机存取存储器建立在变压器理论的基础上，并提供了一种坚固耐用的低功耗解决方案，直到半导体开始流行。在那之前，不起眼的铁氧体磁芯有许多用途，而且做得非常好。阿波罗制导计算机有可擦除磁心存储器，它的大部分软件存储在磁心绳存储器中。

这部电影涵盖了很多理论，而且非常清晰简洁。它首先解释了什么是磁芯以及为什么使用它，然后描述了磁芯如何用来存储比特，以及它们将信息传输到其他磁芯的方法。同时，它提供了双稳态器件的背景知识，并根据磁化力和磁通密度解释了磁化行为。

![B-H curve](img/d995d325e75a027b500abceb90f18b62.png)本质上，磁芯可以根据绕组的方向和引入电流的导体末端在两个方向上磁化。施加的磁化力与流过它的电流量乘以绕组的匝数成正比。随着磁芯上的磁力增加，示出磁化力 H 和磁通密度 B 之间关系的曲线图最终在达到饱和点时变平。当电流停止或减少时，磁心材料保持大部分磁性，这就是所谓的剩磁。

为了克服铁芯的剩磁，需要一定量的磁力，称为矫顽力。一旦这个力使磁通密度回到零，曲线就会向相反的饱和极限移动。在这些极限之间，可以确定磁滞回线。

为了影响第二磁芯，第一磁芯的输出绕组连接到第二磁芯的输入绕组。每个内核都引入了一个移位绕组，以防止二进制状态切换回初始值。最后，这位风度翩翩的军官将解释代表你刚刚所学内容的简化逻辑图。

[https://www.youtube.com/embed/X0WnddW5gZI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/X0WnddW5gZI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[感谢 Martin 发送此邮件]

Retrotechtacular 是一个每周专栏，以旧时的黑客、技术和媚俗为特色。通过[发送您对未来分期付款的想法](mailto:tips@hackaday.com?Subject=[Retrotechtacular])，帮助保持新鲜感。