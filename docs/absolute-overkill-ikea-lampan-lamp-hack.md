# 绝对矫枉过正的宜家 Lampan 灯黑客

> 原文：<https://hackaday.com/2015/05/24/absolute-overkill-ikea-lampan-lamp-hack/>

有时候过度杀戮是不够的。[Jesus Echavarria] [为他的女儿](http://www.jechavarria.com/2015/04/22/hacking-a-lampan-ikea-lamp/)改装了一个宜家 Lampan 灯，增加了彩色 led、定时器、蓝牙色调控制和本地控制旋钮。结果是:一盏价值 5 美元的灯至少增加了 50 美元的魅力。我们来看看后者。

整个灯光系统基于 PIC 微控制器和用于彩色灯光表演的 LED。因为灯已经被制造成运行 40W 灯泡，而[耶稣]想要保留这种功能，他在构造中添加了 SSR。是的，额定功率是 5000 瓦，但这是他手头上的。

[![Top-Elements](img/a7b1c8deb469034a093fba2be6d77831.png)](https://hackaday.com/wp-content/uploads/2015/05/top-elements.jpg) 接下来是低压电源。[耶稣]需要 5V 的 PIC，并使用廉价的 USB 充电器作为快速和肮脏的 5V 转换器-一个不错的黑客。为了给需要 3.3V 电压的 HC-05 蓝牙模块供电，他在 5V 线路上连接了一个低压差稳压器。电平转换器 IC (74LVC07)直接获取两者之间的逻辑电压电平。

高压电源线的保险丝，周围的螺丝端子连接器，以及用于手动超越的电位计完善了硬件构建。

在软件方面，[Jesus]设置旋钮来打开和关闭内置灯以及控制 LED 环的颜色。当他的女儿想改变灯的颜色，但不想去找她的手机时，这是一个很好的接触。但当她这样做时， [SPP Pro 应用程序](https://play.google.com/store/apps/details?id=mobi.dzs.android.BLE_SPP_PRO&hl=en)通过蓝牙向灯中的 PIC 发送预编程的串行命令来设置颜色。

总而言之，这是一个不错的构建，有很好的文档记录，并且有足够的粗糙边缘，没有人会说这不是一个黑客。干得好[耶稣]！我们迫不及待地想看看他接下来会做什么… [机器人灯](http://hackaday.com/2011/09/08/anthropomorphizing-an-ikea-lamp-like-pixar-but-in-real-life/)有人吗？