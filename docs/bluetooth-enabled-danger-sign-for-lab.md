# 实验室蓝牙危险标志

> 原文：<https://hackaday.com/2014/10/29/bluetooth-enabled-danger-sign-for-lab/>

[A Raymond]在工作中有一些空闲时间，他决定利用这些时间制作一个无线警示牌。根据他的博客资料，他是一名应用物理学的博士生。他的实验室使用高功率激光系统。他的工作是使用这个系统，但是只有在它被学院科学家们连上之后。激光系统的状态由一个手动开关盒改变，该开关盒控制实验室入口周围的警告标志。不幸的是，如果你在楼上办公室，跑到楼下检查后才知道这件事。[A Raymond 的]承认懒惰最终战胜了他——他想要一个在舒适的办公室里显示激光状态的标志。他有一个可以使用的旧标志，但他想找到一种方法让它与楼下的开关盒通信。经过一番思考，他决定使用蓝牙技术，使用 Sparkfun 和 Arduino Uno R3 的一对 [BlueSMiRF](https://www.sparkfun.com/products/12582) 蓝牙模块

他建造了一个金属盒，从主开关盒中截取电缆，将一个 BlueSMiRF 和 Uno 安装到其中。在得知开关盒通过三根单独的状态线发送 12V 交流信号后，他对这些线进行了半波整流，并对它们的电压进行了分压，这样 Uno 就不会烧毁。相反，它确定哪条状态线有有效电压。并通过蓝牙连续发送“g(绿色)”、“y(ellow)”或“r(ed)”信号。在接收端，[A Raymond]拆除了标牌，将另一个 BlueSMiRF 和 Uno 与一些绿色、黄色和红色 led 一起安装进去。led 会响应相应的蓝牙信号而亮起。

结果是一个警告标志，它总是与配电盘的状态保持同步。我们以前报道过使用蓝牙的项目，从[长毛绒鸟](http://hackaday.com/2014/08/15/bluetooth-low-energy-beacons-in-a-flock-of-birds/)到[相机](http://hackaday.com/2014/09/12/controlling-a-point-and-shoot-with-bluetooth/)–【A Raymond 的】无线信号是一个好公司。他指出，当“危险”灯亮起时，它“丢失”了一个高音调的呜呜声。如果他决定添加一个伴随的(恼人的)声音，他不会错[像这样的东西](https://www.youtube.com/watch?v=0cVlTeIATBs)。不管怎样，我们确信[A Raymond]很高兴他不用在使用激光之前在楼层间来回走动。