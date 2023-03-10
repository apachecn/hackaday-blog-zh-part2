# 一种小型水下航行器:纳米探索者

> 原文：<https://hackaday.com/2014/10/25/a-compact-underwater-vehicle-the-nanoseeker/>

纳米探索者号是一种鱼雷形状的小型水下航行器。[John]将 Nanoseeker 设计成完全封闭的飞行器:推进器和控制鳍都位于管子的直径范围内。推进器是导管式的，侧面有通风口，控制鳍集成在导管组件的背面。

[John]设计了一个紧凑型 PCB 来驱动车辆，其中包括一个 STM32F4 和几个传感器。MPU-9150 提供 IMU 功能，TI 的两个双电机驱动器 IC 控制油门和控制鳍。[John]还增加了蓝牙无线电遥控功能。对于那些想要近距离观察的人来说，示意图的[图像已经上传到他的博客上。](http://blog.huv.com/2014/08/nanoseeker-new-board.html)

该开发板正在运行 [MicroPython](http://micropython.org) ，这是一个针对微控制器优化的小型 Python 实现。虽然[约翰]的硬件平台看起来很棒，但他的软件还在起步阶段。我们期待看到他的项目如何发展，因为他的项目是我们见过的最小的水下运载工具之一。

[via [危险原型](http://dangerousprototypes.com/2014/10/22/dirtypcb-nanoseeker-v2-1/)