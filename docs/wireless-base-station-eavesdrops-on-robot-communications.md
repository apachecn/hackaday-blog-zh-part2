# 无线基站窃听机器人通信

> 原文：<https://hackaday.com/2013/03/18/wireless-base-station-eavesdrops-on-robot-communications/>

![wireless-base-station-evesdrops-on-robot-communications](img/d2e9a5bd97ed424ffb646a145dbac910.png)

good[博士鬣蜥]一直在研究一对机器人，它们使用 mRF24J40MA 无线收发器相互通信。这给调试带来了挑战，因为他真的没有一种简单的方法来监控这些通信。他的解决方案是[建造自己的基站](http://www.dr-iguana.com/prj_fitzy_and_carraldo/prj_fitzy_and_carraldo_basestation_alpha/index.html),这样他就可以用电脑监控每个机器人在说什么。

他为这个项目制作了自己的董事会。USB 连接由 FTDI 芯片 FT232RL 提供。这将 USB 通信转换为 dsPIC33 微控制器的串行通信。FTDI 芯片具有相当精细的间距，但如果你对工艺相当熟悉，仍然可以使用墨粉转移来制造足迹。[鬣蜥博士]拍摄了一些无人居住的电路板的特写图像，这可能会让你对烙铁有点紧张。电路板的另一端装有和他在机器人上使用的相同的微芯片无线模块。

经过一点返工(注明在照片标签上)，他得到了这个运行。现在，他可以捕获所有的无线通信，并查看问题是由发送方还是接收方造成的。