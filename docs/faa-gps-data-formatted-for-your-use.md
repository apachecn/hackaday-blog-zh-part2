# 美国联邦航空局 GPS 数据格式供您使用

> 原文：<https://hackaday.com/2013/02/14/faa-gps-data-formatted-for-your-use/>

![faa-gps-data-formatted-with-vb](img/f027f00ba8d5e0370a567f2ffd5175bf.png)

[Michael]以 GPX 格式发布了[最新的 GPS 数据集。这些数据集是付费更新的替代方案。由于](http://gpspilot.org/) [GPX](http://en.wikipedia.org/wiki/GPS_eXchange_Format) 是一个已发布的标准，它使用 XML 风格的位置数据格式【迈克尔的】时间花费在获取原始设置和寻找一种方法来为他的 Garmin EXTREX GPS 翻译它们。

原始数据来自——打住，这是满嘴的——美国联邦航空管理局的设施航空数据分发系统( [FADDS](https://nfdc.faa.gov/xwiki/bin/view/NFDC/FADDS) )。他必须申请许可才能下载并使用它来制作定制的 GPS。他获取了机场航路点和[导航台](http://en.wikipedia.org/wiki/Navaid)的设置，然后研究了附带的详细说明数据结构的文件，然后编写了自己的 Visual Basic 2010 程序来处理 GPX 文件。他说，他希望本着开放硬件/软件运动的精神，让它们变得可用。这可能是飞行员最感兴趣的(那种[在仪表板上放角的](http://hackaday.com/2012/10/12/nook-simple-touch-as-a-glider-computer/)，而不是[那种从地面观察飞机的](http://hackaday.com/2011/12/02/eight-dollar-airplane-for-really-bad-pilots/))，但我们确信对非飞行员来说有无数的用途。