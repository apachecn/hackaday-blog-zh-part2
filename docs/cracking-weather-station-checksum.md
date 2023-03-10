# 破解气象站校验和

> 原文：<https://hackaday.com/2015/01/30/cracking-weather-station-checksum/>

[BaronVonSchnowzer]正在开发一些家庭自动化，并选定了一种廉价的环境温度传感器，出售这种传感器是为了增加家庭气象站收集的数据。他发现射频协议已经被逆向工程，并将利用这些信息从每个房间的传感器中获取数据。以真正的黑客方式，他将自己的进步推广到互联网上，让其他人受益。具体来说，他[对环境 F007TH】使用的校验和进行了逆向工程。](https://eclecticmusingsofachaoticmind.wordpress.com/2015/01/21/home-automation-temperature-sensors/)

他是在尝试了为接收传感器的射频通信而编写的 Arduino 草图后进入这条赛道的。由于协议的[校验和](http://en.wikipedia.org/wiki/Checksum)还没有计算出来，代码的一个特殊部分被证明是一个用于过滤损坏消息的过滤器。弄清楚校验和字节是如何工作的并不是一个简单的过程。这次冒险让他将 13k 个样本转储到一个电子表格中，看看对类似的 5 字节消息集和 1 字节校验和集进行排序是否会对情况有所帮助。故事的其余部分是一些令人印象深刻的模式匹配，导致最终的算法。现在[BaronVonSchnowzer]和任何使用这些模块的人都可以用最有效的方式过滤掉损坏的数据。