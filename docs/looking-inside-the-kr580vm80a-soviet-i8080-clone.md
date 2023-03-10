# 查看苏联 I8080 克隆体 KR580VM80A 的内部

> 原文：<https://hackaday.com/2015/03/07/looking-inside-the-kr580vm80a-soviet-i8080-clone/>

Zeptobars 的人运气很好，有时深入研究历史芯片，有时为了我们的利益揭露假设备。在所有这些令人惊叹的镜头背后，是数百个小时的辛勤工作。来自 Zeptobars 的[Mikhail]最近向我们透露了工程师[Vslav]所做的非凡工作，他花了 1000 多个小时对苏联 kr 580 VM 80 a 进行逆向工程，这是那个时代最受欢迎的微控制器之一，也是 i8080 的直接克隆。

但在[Vslav]开始创建原理图和 Verilog 模型之前，芯片需要去盖和蚀刻。当他们向下蚀刻时，他们创造了一系列芯片的[高分辨率图像。在这个过程结束时，他们能够确定芯片有 4758 个晶体管(与传言的 6000 或 4500 相反)。完成图像后，他们能够注释骰子的各个部分，创建 Verilog 模型和原理图。一项严格的兼容性测试证实了他们的 Verilog 模型的准确性。所有的源数据都可以通过(CC-BY-3.0)许可从他们的网站上获得。如果这看起来很有趣，一定要看看他们的一些工作，我们之前已经介绍过了，比如](http://zeptobars.ru/en/read/kr580vm80a2)[比较真的和假的北欧骰子](http://hackaday.com/2015/02/23/nordic-nrf24l01-real-vs-fake/)以及[如何计算出这些去盖芯片的工作方式](http://hackaday.com/2014/05/26/ken-shirriff-explains-the-tl431/)的惊人描述。如果这对于你来说太难了，那就试试稍微简单但同样棒的 PCB 分层过程[。](http://hackaday.com/2015/03/05/deconstructing-pcbs/)