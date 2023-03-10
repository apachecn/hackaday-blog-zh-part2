# 使用网络摄像头和 Python 读取用电数据

> 原文：<https://hackaday.com/2014/12/29/reading-power-use-data-with-a-webcam-and-python/>

正如任何黑客都会证明的那样，每当一个重要的工具丢失时，你还不如重新构建一个！当[Matt]试图测量他父母家的耗电量时，他发现自己正处于这种境地。他把电表的发射器留在了家里，所以合乎逻辑的做法是安装一个网络摄像头和一个 python 脚本来监控他父亲的电表，而不是回去拿他的电表。

他手边的功率计是一个 GEO Minim 电力监视器。他发现很难直接从这个特定的仪表中提取数据，所以他没有深入研究仪表中的任何通信协议，而是在一个带 LED 的盒子中安装了一个网络摄像头，并用专门编写的 Python 脚本进行监控。该脚本能够看到仪表的细节，然后将所有相关数据报告给计算机。[Matt]已经把这些代码放在他的项目网站上，供任何人使用。

这是一个很好的解决方法，不需要太深入地研究有问题的仪表的内部工作原理。不过，如果这更符合你的风格，你也可以[构建自己的电源监控系统](http://hackaday.com/2014/08/01/electricity-monitoring-with-a-light-to-voltage-sensor-mqtt-and-some-duct-tape/)！