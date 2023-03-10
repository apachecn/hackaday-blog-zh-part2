# 创建扫描单色仪

> 原文：<https://hackaday.com/2014/11/22/creating-a-scanning-monochromator/>

如果你出于研究目的需要特定波长的光，获得这种光的天真方法是一个白色光源，一个棱镜和一个小狭缝，它将穿过你个人的月亮专辑封面的黑暗面。这实际上是一个可怕的想法；你不仅不会有一个参照，知道你让什么波长的光通过光学狭缝，棱镜本身会比其他的吸收更多的一种波长的光。

解决方案是一个单色仪，一个执行相同研究任务而没有所有缺点的设备。[Shahriar]得到了一台旧的手动单色仪[，并决定将它变成一台执行自动扫描的设备](https://www.youtube.com/watch?v=veETVeEsaNM&feature=youtu.be)。

单色仪的关键是一个衍射光栅，这是一个镜面，上面有许多以阶梯图案排列的平行细槽。由于衍射光栅的表面，可以像棱镜一样根据光谱分离光线。与棱镜不同，它实际上是第一面镜子，这意味着所有波长的光都或多或少地被同等反射。

通过在单色仪的刻度盘上增加一个步进电机，[Shahriar]能够自动扫描设备的整个范围。单色仪内部是一个光电倍增管，它对入射光进行采样，并将其转化为电压。通过对该电压进行采样并用 MATLAB 绘制，Shahriar 能够绘制出该设备范围内每个波长的光的强度。这一切都在下面的视频中得到专业的解释。

[https://www.youtube.com/embed/veETVeEsaNM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/veETVeEsaNM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)