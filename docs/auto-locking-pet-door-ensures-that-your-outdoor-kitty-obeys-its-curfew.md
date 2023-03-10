# 自动锁定宠物门确保你的户外猫咪遵守宵禁

> 原文：<https://hackaday.com/2012/04/04/auto-locking-pet-door-ensures-that-your-outdoor-kitty-obeys-its-curfew/>

![auto-locking-pet-door](img/70d95388113902f8e5c6bdb5710a1367.png "auto-locking-pet-door")

如果你有一只自由进出你家的宠物，你可能会发现自己想要更严密地管理它们的进出。当危险的动物可能潜伏在附近时，[tareker]想让他的猫在晚上呆在室内，但他不想让它成为一个麻烦。

他手头上已经有了上锁的宠物门，他破解了这个门来自动控制他的猫的进出。他安装了一对簧片开关，以确定门是向外打开(猫离开)还是向内打开(猫回来)，并使用 Arduino Nano 跟踪状态。每当夜幕降临后，附在门框上的伺服电机检测到猫安全地呆在里面，就会把门锁上。

虽然他还增加了一个 RGB LED 来反映门的状态，但他正在考虑将它连接到互联网，以便他可以从他当时可能在的任何地方控制和检查门。