# 通过点烟器测量汽车发动机转速

> 原文：<https://hackaday.com/2014/06/10/measuring-car-engine-rpm-via-the-cigarette-lighter/>

[![delorean](img/404bd90d86fe299da83104acbbcd50e4.png)](https://hackaday.com/wp-content/uploads/2014/06/del.png)

有时我们会忘记用一个简单的示波器可以做多少事情。在这个视频中【Ben】用泰克借给他的一个来测量他的德罗宁发动机转速。通过检查汽车主电源 12V 电压，人们可能会注意到出现的电压尖峰与发动机转速直接相关，因为它们是由点火线圈的感应冲击产生的。很明显，从每秒峰值数得出每分钟转数的乘法运算取决于你的发动机配置(4 缸，v6…)。

[Ben]使用的方法是在(交流耦合)汽车 12V 快速傅立叶变换(FFT)上搜索高幅度尖峰，以获得可靠的测量结果，因为他的汽车中存在许多电气噪声源。然而，在视频的最后，他提到，利用简单的电压比较器和足够高的基准电压源，仍有可能获得良好的测量结果。

[https://www.youtube.com/embed/t0ToYhjYV9I?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/t0ToYhjYV9I?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)