# 使用 Arduino 的太阳能电池板系统监控装置

> 原文：<https://hackaday.com/2015/03/05/solar-panel-system-monitoring-device-using-arduino/>

[卡尔]最近用太阳能电池板系统升级了他的房子。该系统补充了他从电网获得的电力，通过使用来自太阳的免费(如啤酒)能量来填充电池组。该系统配备了一个基本的电表，它实际上只显示电池板产生的总电量。[Carl]想从他的系统中获取更多数据。他设法用 Arduino 构建了自己的显示器。

这种构建的技巧与系统的工作方式有关。该面板包括一个 LED 灯，每度电闪烁 1000 次。[Carl]意识到，如果他能够监控 LED 闪烁的频率，他就可以确定在任何给定时刻大约产生了多少能量。我们过去已经看到过类似的项目。

像大多数新接触技术的人一样，[卡尔]通过拼凑他在网上找到的其他例子建立了他的项目。他开始使用一个草图，这个草图最初是通过测量车辆通过两点之间的时间来计算车辆的速度。[Carl]采用了这种代码，并将其修改为使用单个光敏电阻来检测 LED。他还用几个发光二极管制作了一种 VU 计。电表的增减与电表的读数成正比。

[Carl]不断改进他的系统。他增加了一个液晶面板，这样他不仅可以看到准确的当前测量值，还可以看到当天的最高测量值。他把所有的电子设备放在一个塑料盆里，用一根带状电缆把液晶面板移到一个更方便的位置。他还让他的朋友[Andy]清理 Arduino 代码，以便其他人可以更容易地使用。