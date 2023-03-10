# 只要把你的嘴唇凑在一起就能打开一盏灯

> 原文：<https://hackaday.com/2013/05/18/just-put-your-lips-together-to-turn-on-a-lamp/>

![whistler-lamp-control](img/4c11ece36fd7471debdb56c06cfab9d8.png)

嵌入的图像是一个控制器板，[Limpkin]开发的[增加了哨声控制作为家庭自动化选项](http://www.limpkin.fr/index.php?post/2013/04/26/The-whistled%3A-how-to-remake-a-dozen-years-old-project-the-right-way)。它的有效范围约为 15 英尺，能很好地探测到来自不同人的口哨声。这是一个测试对象(用隐藏的摄像机拍摄)对着白色 LED 灯吹口哨来打开它。

电路板很小。[Limpkin]在他的测试视频开始时举起它，这给人一种很好的比例感。一端有一个桶形插孔，电路板通过它获得电源。另一端有一个双导线螺丝端子，用于切换您的设备。当连接重外部负载时，N 沟道 MOSFET 保护电路。它能驱动相当大的 90 瓦功率。如果你正在寻找转换电源额定设备，你需要把你自己的继电器带到聚会。

音频处理由电路板中央的飞思卡尔 ARM Cortex M4 芯片处理。串行线调试(SWD)时钟和数据引脚都连接到焊盘，因此这是可以实现的。[Limpkin]发布了原理图、gerbers 和代码模板。但他没有公布他用于处理的算法，所以如果你想在家里做这个，你需要自己去弄清楚。如果你需要帮助，你应该看看这个基于口哨的遥控器。

[https://www.youtube.com/embed/1eIxAMKNphw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/1eIxAMKNphw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)