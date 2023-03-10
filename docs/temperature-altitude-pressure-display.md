# 温度、高度、压力显示

> 原文：<https://hackaday.com/2015/04/01/temperature-altitude-pressure-display/>

在最近的一次不丹之旅中，[electronut]希望有一种设备能够显示他在这个王国所到之处的温度和海拔高度。旅行结束回到家后，他用一些现成的零件制作了这个简单的温度、高度和压力显示装置。

经过短暂的搜索，他锁定了可以测量温度和压力的 [BMP 180 传感器](https://www.bosch-sensortec.com/en/homepage/products_3/environmental_sensors_1/bmp180_1/bmp180)，这种传感器可以从许多来源以分线板的形式获得。他根据压力计算高度。主要部件是 Arduino Pro 迷你克隆、BMP180 传感器和诺基亚 5110 LCD 模块。一个标准的 9V 电池为该设备供电。按钮界面允许他在按下时读取当前参数，从而节省电池寿命。

标准库允许他轻松地将 LCD 和传感器连接到 Arduino。他将硬件封装在一个定制的激光切割亚克力盒子里。结果比他希望的要大，所以下一次迭代可能会使用定制的 PCB 和 LiPo 电池来缩小它的尺寸。与此同时，我们认为给设备添加 RTC 和某种日志记录功能会很好，这样它就可以存储数据以供将来分析。原理图、代码和外壳图可通过他的 [Github](https://github.com/electronut/bmp180) 库获得。