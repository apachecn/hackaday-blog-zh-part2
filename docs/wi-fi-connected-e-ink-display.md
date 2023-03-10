# Wi-Fi 连接的 E-Ink 显示器

> 原文：<https://hackaday.com/2015/02/16/wi-fi-connected-e-ink-display/>

实施 Scrum 项目管理方法的人经常在一个大白板上记录他们所有的任务。然而，拥有最新的图表来确保项目正常进行是很有用的。[Sprite_TM]通过构建一个 [Wi-Fi 连接的 E-Ink 显示器](http://spritesmods.com/?art=einkdisplay&page=1)来增强白板。

Interfacing with E-Ink displays isn’t easy. A variety of voltages are needed, and the connectors used are tiny. We’ve seen some nice solutions, such as the [RePaper](http://hackaday.com/2013/07/29/2013-open-hardware-summit-badge-includes-epaper-display/) display. [Sprite_TM] chose the ED060SC4 display which is available from eBay and has been [throughly reverse engineered](http://essentialscrap.com/eink/). A custom breakout board was built up to connect to the tiny FPC pins and generate the required voltages using the [LT1945](http://www.linear.com/product/LT1945) DC/DC converter.

下一步是增加无线网络。ESP12 模块是一个显而易见的解决方案。该模块提供 Wi-Fi 连接和能够控制显示器的处理器。该显示器由平板电池供电，这使得它完全是无线的，可以工作约 200 天。

一个简单的激光切割外壳将所有的部分结合在一起，并包含将屏幕粘在白板上的磁铁。在软件方面，图像被传输到 ESP12 的处理器并直接加载到屏幕上，因为 ESP12 没有足够的 RAM 来存储整个屏幕的数据。所有的固件都可以通过克隆一个 [Git 库](http://git.spritesserver.nl/espeink.git/)得到。