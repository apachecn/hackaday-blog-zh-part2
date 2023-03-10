# 电动卡丁车有 Arduino 大脑

> 原文：<https://hackaday.com/2014/07/26/electric-go-cart-has-arduino-brains/>

![arduino powered go cart](img/665c5b93df05be901f4a329607dd5efc.png)

哦，时代变了。早在 30 年代，大众甲壳虫就被设计得便宜、简单，便于一般车主自己维护。如今，现代汽车的各个方面都由某种计算机控制。至少我们的卡丁车免于这场不可修复的电子噩梦。嗯，那不再是完全正确的了。历史正在重演，因为[InverseCube]已经建造了一辆完全由 Arduino 控制的电子卡丁车。我是不是忘了说【InverseCube】才 15 岁？

这个项目从一个旧的气体驱动的手推车框架开始。一旦燃气发动机被拆除，车架被清理干净并上漆，一个[hobbying Xerun](http://www.hobbypartz.com/07e-c-xerun-150a-sd.html)150 a 无刷电子速度控制器(ESC)和一个 Savox [BSM5065](http://www.savoxusa.com/Savox_BSM5065_450KV_Pro_Spec_700_Class_Brushless_O_p/savbsm5065p450.htm) 450Kv 电机被安装在车架上，负责沿着道路移动手推车。三个并联的 5 芯锂聚合物电池为电机提供大约 20 伏的电压，最高时速约为 30 英里/小时。在需要充电之前，以 15 英里的中等速度快速行驶大约可以行驶 30 分钟。方向盘上装有一个电位计，用来控制推车的速度。Arduino 读取电位计的值，然后向电子悬架控制系统发送相应的脉宽调制信号。

除了油门控制，Arduino 还负责车辆的其他操作方面。有一堆 LED 灯，可以用作前灯、尾灯、转向灯、刹车灯，甚至还有一个用作倒车灯。你可能想知道为什么要用 Arduino 来控制像刹车或大灯这样简单的东西。[InverseCube]在代码中编程了一些逻辑，如果启用了 ESC 制动功能，如果油门低于空档或如果 ESC 启用开关关闭，则保持刹车灯亮起。前灯有 3 种亮度，全部由微控制器提供的 PWM 信号控制。

方向盘中央还安装了一个液晶显示器。这也是由 Arduino 控制的，并显示油门值、灯的状态和电池的电压。

via [reddit](http://www.reddit.com/r/arduino/comments/2bqbpe/i_posted_a_while_ago_about_my_arduino_gokart/)