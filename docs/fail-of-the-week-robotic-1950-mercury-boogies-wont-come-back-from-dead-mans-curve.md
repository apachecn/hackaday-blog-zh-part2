# 本周失败:机器人 1950 水星布吉，不会从死人曲线回来

> 原文：<https://hackaday.com/2014/09/18/fail-of-the-week-robotic-1950-mercury-boogies-wont-come-back-from-dead-mans-curve/>

[戴夫]想用遥控的 1950 年水星制造一个 Arduino 机器人。他移除了汽车的遥控部分，保留了驱动和转向马达。这个想法是在格栅地产中使用三个超声波测距仪，并根据检测到的最长距离向前移动汽车。

他最初使用 Seeed 电机控制器和一些焊接到传感器上的 Grove 电缆来驱动转向。它前进了，但只是前进，而且[戴夫]认为马达控制器和汽车的转向马达没有很好地配合。

[Dave]想出了用继电器来给电机供电和确定极性的主意。现在，这辆奔驰有一半的时间在转向和躲避障碍物，但它也因为撞到墙壁而被撞破。他发现他的传感器排列使汽车立即转向，并决定用一个簧片开关和一个稀土磁铁从车轮上给程序信息。唯一的问题是触发簧片开关所需的磁铁的口径太重太强。[戴夫]并得出结论，他只是不能行使对汽车的控制，他需要的那种。而且会自己造机器人底盘。

更新:休息后看看[戴夫]的车的视频。

* * *

**[![2013-09-05-Hackaday-Fail-tips-tile](img/4ddcb45ba24697ecb36e5a2da073e8dc.png)](mailto:tips@hackaday.com?Subject=[Fail of the Week]) 每周失败是一个每周三运行的黑客专栏。通过写下你过去的失败和[给我们发送一个故事的链接](mailto:tips@hackaday.com?Subject=[Fail of the Week])，或者发送你在互联网旅行中发现的失败报道的链接，来帮助保持乐趣。**

 [https://www.youtube.com/embed/0UqfoBVGo5E?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/0UqfoBVGo5E?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)