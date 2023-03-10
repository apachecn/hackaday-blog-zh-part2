# PeriUSBoost:一个 DIY USB 电池组

> 原文：<https://hackaday.com/2014/12/10/periusboost-a-diy-usb-battery-pack/>

如果你经常旅行，经常使用移动设备，或者在手机上运行有问题的 rom，你很可能有一个外置 USB 电池组。这些方便的设备可以让你给手机、平板电脑或 USB 供电的空气加湿器(是的，这些都存在)提供一些额外的能量。

[Pedro]的 [PeriUSBoost](http://hackaday.io/project/3591-periusboost) 是一款 DIY 手机充电解决方案。这是一个开关调节器，可以将电池电压提升到 5 伏 USB 标准。这是通过使用 [LTC3426](http://www.linear.com/product/LTC3426) 实现的，这是一种带有内置开关元件的 DC/DC 转换器。该 IC 采用小型 SOT-23 封装，需要一些外部无源器件。

USB 充电的一个有趣细节是 USB 数据线上的电阻配置。这些告诉设备有多少电流可以从充电器中提取。对于该器件，选择电阻将充电电流设置为 0.5 A。

虽然 0.5 A 的充电电流并不算很快，但它确实可以为 AA 电池充电。[Pedro]的测试结果是用两节 AA 电池给手机充满电，但在给设备供电时确实有点热。它可能不是放在口袋里的最佳设备，但它能完成工作。