# Rocketduino，用于高重力、高海拔测井

> 原文：<https://hackaday.com/2013/07/07/rocketduino-for-high-g-high-altitude-logging/>

![rocketduino](img/63e127b9269350fb9ecb68d4429f3127.png)

虽然发射火箭的刺激通常是在它们安全体面地返回地球时发现的，但最终你会想要一些飞行数据。气压、GPS 记录和加速度数据都是有用的东西，尤其是如果你试图完善你的工艺。reddit [上的【佐内斯】创建了一个数据记录板，专门为业余火箭爱好者创建的](http://www.reddit.com/r/rocketry/comments/1hlfx5/my_custom_arduino_mega_based_rocket_computer/)，这是一个难以置信的作品，经得起非常快和非常高的严格要求。

该板的设计是 Arduino Mega 和 Due 的盾牌，并配有足够的传感器来过度分析任何火箭飞行。GPS 记录 66Hz 的位置和高度，两个加速度计测量高达 55 G。气压、温度和指南针传感器通过 ZigBee 900MHz 无线电链路告诉地面站他们需要知道的所有数据。

因为这是一个 Arduino，设置飞行事件，例如打开主伞和减速伞，就像上传一点代码一样简单。这是为直径 4 英寸的火箭建造的，但他说它可能适合 3 英寸的火箭。我们迫不及待地想看一些视频。