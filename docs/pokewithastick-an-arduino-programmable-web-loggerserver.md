# Pokewithastick，Arduino 可编程网络记录器/服务器

> 原文：<https://hackaday.com/2013/10/08/pokewithastick-an-arduino-programmable-web-loggerserver/>

[![](img/b09492dc731b80a953971f4cce12e1db.png)](http://hackaday.com/wp-content/uploads/2013/10/ver2-4.jpg) 
【斯图尔特】向我们透露了他非常好的项目:[神奇宝贝](http://www.pokewithastick.com/bigboard.html)。这是一个基于 ATMEGA1284P 的 Arduino 兼容板(硬件，而非尺寸),可以通过编程收集数据并将其发布到 Thingspeak 或 Xively 等互联网日志网站。

正如你在上面的图片中看到的，它有一个小的 50x37mm 毫米的尺寸(大约 2 英寸 x1.5 英寸)。pokewithastick 由一个 Wiz820 以太网模块、一个 micro-SD 卡插槽、2 个串行端口、一个电池供电的实时时钟(RTC)、一个无线电连接器(用于通常的 nRF24L01 2.4GHz 无线电)、一个电源和用户 LED 以及最后一个重置按钮组成。板上有两个电源轨，可以分开(5v + 3.3V)或合并(仅 3.3V)，这可能允许您将 Arduino 屏蔽连接到它。如果安装了适当的(Arduino)引导程序，您可以使用标准的 6 针接头或通过串行编程器对电路板进行编程。

该项目是开放的硬件，已经使用 [Kicad](http://www.kicad.org/display/KICAD/KiCad+EDA+Software+Suite) 设计，所有文件可以下载[作为 zip 文件](http://www.pokewithastick.com/philes/PCB_bigboard.zip)。