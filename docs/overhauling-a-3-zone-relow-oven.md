# 检修 3 区回流炉

> 原文：<https://hackaday.com/2014/12/09/overhauling-a-3-zone-relow-oven/>

[Ed]拥有一台 3 区回流炉(他恰好用它来制造回流炉控制器)，但随着时间的推移，它的性能越来越差。传送带的速度变得如此不一致，以至于大多数通过烤箱的电路板都没有完全回流。[Ed]决定[把烤箱的内脏取出来，换上一个 Arduino](http://www.estechnical.co.uk/blog/entry/fixing-our-3-zone-reflow-oven) ，解决了皮带问题，并更换了烤箱不友好的用户界面

[Ed]在研究他的皮带速度问题时，发现皮带电机是由一个可调线性调节器控制的，没有反馈。虽然这本身看起来有点粗略，但马达也有一些机械问题，最终[Ed]完全取代了它。在意识到闭环速度控制确实有助于使烤箱更加稳定后，[Ed]决定彻底检查烤箱中的所有电子设备。

[Ed]希望尽可能少地定制硬件，所以他开始使用 Arduino Mega 和一些 MAX31855，用于测量烤箱中的多个热电偶。Arduino 控制皮带速度，并运行 PID 回路，控制烤箱 3 个区域的加热元件。Arduino 可通过不同的配置文件(存储在 EEPROM 中)进行编程，这些配置文件由 3 个区域温度和传送带速度组成。你没有自己的三区烤箱吗？查看一些我们在之前[展示过的](http://hackaday.com/2013/11/21/a-pair-of-toaster-reflow-oven-builds/) [DIY 回流焊炉](http://hackaday.com/2014/05/13/an-open-source-cortex-m0-halogen-reflow-oven-controller-with-lcd/)版本。