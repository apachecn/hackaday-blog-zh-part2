# 游泳池/热水浴缸监控和数据收集

> 原文：<https://hackaday.com/2015/06/01/poolhot-tub-monitoring-and-data-collection/>

游泳池和热水浴缸，虽然令人愉快，但需要监控和维护，以保持水的清洁和清澈。[bhuebner]不喜欢用测试条和水测试套件不断测试他的热水浴缸的生命体征。为了自主监控他的热水浴缸的水，他想出了一个他称之为 [SpaSitter](http://www.instructables.com/id/Build-Your-Own-Spa-or-Pool-Monitor/?ALLSTEPS) 的项目，记录并跟踪水质指标。

[![spa sitter ](img/305edc79aa66fa78c622c12c5e0b195b.png)](http://cdn.instructables.com/FH0/7HOQ/H7UR8256/FH07HOQH7UR8256.LARGE.jpg) 硬件基于一个 [Nanode](http://www.nanode.eu/what-is-nanode/) (想想 Arduino 带板载以太网)。三个传感器连接到纳米电极上，并放置在他的热水浴缸的水中。传感器测量 pH 值、 [ORP](http://www.ozoneapplications.com/info/orp.htm) 和温度。这些数据随后被上传到[xively.com](http://xively.com/)，在那里数据不仅被存储，还会随着时间的推移被跟踪并以图表的形式显示出来。在手机上检查生命体征也会变得有点乏味，所以[bhuebner]设置了一个电子邮件通知，如果其中一个测量的数据流超出了预定的范围。他仍然必须手动添加化学物质，并希望在下一个项目修订中看到一些自动化。

[布纳]提供了他的[代码](https://github.com/brianhuebner/OpenSpaMonitor2/tree/master/Nanode_SpaSitter_monitor_V_1_0),还张贴了详细的说明，包括如何校准传感器，供任何想做同样事情的人使用。