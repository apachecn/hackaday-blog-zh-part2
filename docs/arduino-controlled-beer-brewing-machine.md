# Arduino 控制的啤酒酿造机！

> 原文：<https://hackaday.com/2013/12/13/arduino-controlled-beer-brewing-machine/>

[the_meatloaf]刚刚用 Arduino 对他的全自动啤酒酿造机进行了最后的润色。

这个项目是他计算机工程学位的一部分，花了[the_meatloaf]和两个机械工程师朋友一年的时间从零开始设计和建造整个系统。带有 4 按钮界面的 Arduino Mega 允许您编程、保存、加载、重命名和运行多达 26 种保存到 EEPROM 的不同配方。

像这样的自动化系统消除了原本复杂的酿造过程中的大部分猜测。机器首先使用 2000W 加热元件加热第一桶中的水，然后水通过伺服阀转移到糖化容器中，在那里由混合马达搅拌。然后，机器排出麦芽汁(糖化后产生的液体)，并按照程序喷洒谷物(向糖化罐中加入更多的水):[谢谢，[Chris，]澄清！](http://hackaday.com/2013/12/13/arduino-controlled-beer-brewing-machine/#comment-1133827)麦芽汁在设定的时间内煮沸，同时伺服控制的“料斗”自动添加啤酒花。最后，逆流热交换器使用冰水将溶液快速冷却至室温，然后分配溶液用于发酵。

虽然[肉卷]迄今为止最大的项目相当成功，但不幸的是，他无法享受它。承担 1000 美元预算的赞助商收回了这台机器。Drat。

[via [Reddit](http://www.reddit.com/r/arduino/comments/1srcm8/arduino_controlled_beer_brewing_machine/)