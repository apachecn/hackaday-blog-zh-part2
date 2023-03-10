# 外在动机:遥控飞机的智能天线跟踪器

> 原文：<https://hackaday.com/2014/09/01/extrinsic-motivation-smart-antenna-tracker-for-rc-aircraft/>

长途 FPV(第一人称视角)飞行可能是少数。保持视频馈送活动通常需要高增益定向天线。走向定向会产生保持天线指向飞机的麻烦。[Brandon 的] [智能天线跟踪器](http://hackaday.io/project/2150)被设计成自动完成所有这些工作。你会问，这是什么巫术？答案其实很简单:遥测！许多飞行控制系统有一个可选的遥测发射器。[Brandon]正在使用 3DRobotics APM 或 PixHawk 系统，它们使用 3DR 的 915 MHz 无线电。

机载无线电向地面站发送遥测数据，包括飞机的纬度和经度。智能天线追踪器配有接收这些数据的接收器和自己的 GPS，知道飞机的准确位置、航向和速度。使用平移和倾斜安装，智能天线跟踪器可以将天线直接指向机载系统。由于 FPV 天线位于云台上，它也将指向飞机并保持良好的视频连接。

像这样的系统的一个问题是处理一架直接从头顶飞过的飞机。飞机或旋翼机飞行的速度比天线系统移动的速度快。当飞机靠近时，有一些商业系统通过切换到较低增益的全向鞭状天线来处理这个问题。这将是对[布兰登的]设计的巨大补充。