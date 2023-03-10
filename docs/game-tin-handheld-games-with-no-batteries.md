# 游戏锡:没有电池的手持游戏

> 原文：<https://hackaday.com/2014/10/16/game-tin-handheld-games-with-no-batteries/>

任何和游戏机一起长大的人都知道他们有多喜欢 AA 电池。[Nick]的[游戏机](http://www.shifthack.com/game-tin/features/)通过运行由太阳能充电的超级电容器解决了这个问题。

控制台基于一个 [EFM32](http://www.silabs.com/products/mcu/lowpower/pages/efm32g-gecko.aspx) 微控制器:一个为低功率应用设计的 ARM 设备。128×128 像素单色内存显示屏提供低 fi 图形，同时保持低功耗。

有两个太阳能电池和一个 [BQ25570](http://www.ti.com/product/bq25570) 能量收集 IC 为超级电容充电。该芯片负责[最大功率点跟踪](http://en.wikipedia.org/wiki/Maximum_power_point_tracking)，以充分利用太阳能电池。如果天黑了，连接 USB 电源可以在 30 秒左右为设备充电。

10 F Maxwell 超级电容器可以在没有阳光的情况下在设备上运行 1.5 小时的游戏，设备在阳光下无限期运行。由于内存显示，具有较低刷新率的应用将具有低得多的功耗。

游戏 Tin 是开源的，正在使用 KiCad 开发。你可以从 Bitbucket 中抓取所有 EDA 文件[。[尼克]也在衡量对游戏锡的兴趣，并希望将其作为一个套件发布。](http://www.shifthack.com/game-tin/source/)