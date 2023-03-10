# 把便宜的电压表变成 I2C 显示器

> 原文：<https://hackaday.com/2013/08/25/turning-cheap-voltmeters-into-i2c-displays/>

[![Voltmeter I2C Displays](img/184344b65a87f5d460665942ccd2c2e4.png)](http://hackaday.com/?attachment_id=101894)

[Tom]一个项目需要 8 台显示器。他想控制他们在 I2C，并试图降低成本。一些供应商生产 I2C 可控七段显示器，但每个售价约 10 美元。[汤姆]认为他可以黑掉便宜的电压表来得到同样的结果，每次大约 3 美元。

[Tom]买的电压表用的是 8 位 [STM8S003F3P6](http://octopart.com/datasheet/stm8s003f3p6-stmicroelectronics-20733190-10633907) 微控制器。他对设备进行了逆向工程，并重新创建了原理图，以找出 I2C 和编程引脚的位置。然后，他将其连接到一个 STM8 发现开发板，该开发板具有集成的编程器。

硬件解决后，是时候更换新的固件了。幸运的是，[ba0sh1]已经为[编写了一个类似用途的固件](http://www.ba0sh1.com/hacking-a-cheap-led-voltmeter/ "Hacking a Cheap LED Voltmeter")，它可以很容易地被改编。该代码实现了一个软件 I2C 从机，它从总线上读取数据并显示出来。这些都可以在 [Github](https://github.com/t0mpr1c3/I2C-LED "I2C LED on Github") 上找到。

最终的结果是 I2C 控制的显示器，价格只有原来的三分之一。下次你在一个项目中需要一堆这样的东西时，考虑买一些便宜的电压表。