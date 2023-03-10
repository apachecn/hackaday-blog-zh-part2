# 利用门把手的导电性来探测入侵者

> 原文：<https://hackaday.com/2014/03/30/using-a-door-handle-conductivity-to-detect-intruders/>

[![](img/e6e5515e202410921964e27b317cac54.png)](http://hackaday.com/wp-content/uploads/2014/03/dqsdqsdq.png)

有时最简单的项目可能会非常有趣，只要它们有很好的文档记录。我们希望 Hackaday 的读者也认为【Alexander】开发的门传感器属于这一类。他没有使用普通的方法，如磁铁+簧片开关，而是决定使用触板和门的导电性来检测有人走进。他组装的装置包括一个 Arduino，一个 PowerSwitch Tail(一条可以切换 120vac 和 3-12vdc 直流控制电压的电源线)，一个由 8 节 AA 电池组成的电池组和两个用于门连接的鳄鱼夹。

大多数新爱好者可能会止步于此，但[亚历山大]检查了他的平台的功耗，并继续努力降低功耗。因此，他默认将微控制器置于关断模式，并使用 AVR 外部中断将其唤醒。以防初学者看不懂[Alexander]的代码，他居然在自己的网站上放了一个很好看的流程图。休息后嵌入的是系统工作的视频。

[https://www.youtube.com/embed/bhM0mf_cdxk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/bhM0mf_cdxk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)