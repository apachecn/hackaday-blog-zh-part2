# 用数控铣床切割钥匙

> 原文：<https://hackaday.com/2014/01/03/key-cutting-with-a-cnc-mill/>

![key2_zpsc260d079](img/4f8e4b16f3a60accffc11119fd5b8c13.png)

锁匠那里复制一把钥匙要花 2 美元？但是这有什么意思呢？这里有一个简单的方法[用数控铣床切割你自己的钥匙！](http://www.chaski.org/homemachinist/viewtopic.php?f=43&t=95853)

【Bolsterman】现在“*工作”*为一家出租各种房产的房地产公司工作。每当有人搬走，锁需要尽快更换。他们使用西勒奇锁，可以更换为任何密码组合。新钥匙通常用打孔机或钥匙切割机切割——他几年前就有一把，但已经扔掉了。他不想为他在房地产公司的新工作买一台新的，他决定看看将他的小型台式 CNC 变成他自己的私人钥匙切割机有多难。

[Bolsterman]将他的磨机改造成钥匙切割机所需要的只是一个 3/8 的 90°埋头钻头，其末端打磨成大约 0.055 英寸宽的平面(0.035 英寸是工厂钥匙的宽度，但稍微留一点余地会更容易制作钥匙)。然后你只需简单地将钥匙肩部的磨口归零，使用方便的西勒奇别针图表(包含在原始链接中)，切出凹槽！

为了实现这一切的自动化，[Torrie Fischer]基于[Bolsterman 的]技术创建了一个 python 脚本来生成密钥的 GCode 它托管在 [Noisebridge 的 Wiki](https://noisebridge.net/wiki/Key_Milling) 上——来看看吧！

但是如果这一切看起来太费力，你可以[打印一个新的密钥来代替……](http://hackaday.com/2011/05/31/a-keygen-for-the-real-world/)