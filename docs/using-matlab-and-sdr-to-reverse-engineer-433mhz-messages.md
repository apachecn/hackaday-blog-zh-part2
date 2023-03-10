# 利用 MATLAB 和 SDR 对 433MHz 报文进行逆向工程

> 原文：<https://hackaday.com/2015/02/16/using-matlab-and-sdr-to-reverse-engineer-433mhz-messages/>

世界各地的黑客都对 SDR 乐此不疲——从 Hackaday 上的相关帖子数量可以明显看出这一点。又何乐而不为，硬件便宜又容易获得。有各种各样的软件工具可以用来钻研和探索，比如 SDR#、Audacity、HDSDR 等等。[伊利亚斯]关注 SDR 项目已经有一段时间了，这激起了他的兴趣，足以让他开始玩这个项目。他心中没有任何真正的项目，所以他专注于研究可用于分析 433MHz RF 传输的方法和工具。他描述了使用 MATLAB 来[恢复 SDR](https://ilias.giechaskiel.com/posts/rtl_433/index.html) 正在接收的传输的过程

他首先研究了现有的工具来揭示协议的细节。测试设备使用 Arduino UNO 和 rc-switch 库，通过一个普通且廉价的 433MHz 模块进行传输。SDR#用于记录传输，Audacity 允许[伊利亚斯]可视化结果。wav 文件。但真正有趣的是他用 MATLAB 记录信号分析的地方。

他使用 [RTL-SDR 包](https://uk.mathworks.com/hardware-support/rtl-sdr.html)配合[通信系统工具箱](https://uk.mathworks.com/products/communications/)进行频谱分析、噪声过滤和包络提取。MATLAB 可能不是最容易使用的，也不是最便宜的，但其强大的功能和可以轻松读取来自 SDR 的数据的事实使其成为一个有趣的工具。要全面了解 SDR 到底是怎么回事，请查看[为什么您应该关注软件定义无线电](http://hackaday.com/2015/02/12/why-you-should-care-about-software-defined-radio/)。