# 电源频率显示

> 原文：<https://hackaday.com/2013/12/12/mains-frequency-display/>

[James]住在英国，那里的电力频率应该是 50Hz，但它往往会根据供求关系而波动。他决定要一个显示器来追踪这个。

现在，[国家电网网站](http://www2.nationalgrid.com/uk/industry-information/electricity-transmission-operational-data/)显示了最近 60 分钟的实时图表。但这太简单了。是时候拿出烙铁了！

带着铅笔和纸，[詹姆斯]草草记下了一些如何计算频率的想法——他决定计算 200 个周期，这意味着在 50.000 赫兹的频率下，需要 4 秒钟。下一个问题是获得足够精确的工作时间源。ATtiny84 不行(太不准确)，外部晶体也不行(太贵)——但实时时钟呢？就是这张票！他使用的是 DS3231 RTC 芯片，在+/- 2ppm 32.768kHz 时已经足够精确。

一些数学，编程和焊接之后，显示器就完成了！他甚至添加了一个上/下箭头来显示电力的最新趋势。

好样的[詹姆斯]！去年[Ch00f]做了一个类似的项目，他拆下了一个 194 分立晶体管时钟套件，看看它是如何工作的——顺便说一句，他需要知道从他的墙上发出的 60Hz 有多准确！