# 建造一个廉价的飞机 ADS-B 无线电接收跟踪站

> 原文：<https://hackaday.com/2014/01/16/build-a-cheap-airplane-ads-b-radio-receiving-tracking-station/>

你家上空或家附近有商业或通用航空飞过吗？你想知道更多关于这些飞机的信息吗:身份、航向、速度、高度，也许还有 GPS 数据以及更多信息？那么[Rich Osgood]正好有适合你的项目，而且建立起来并不昂贵。[Rick]演示了使用廉价的 USB 加密狗欧洲电视调谐器风格的 SDR(软件定义的无线电)调谐器，您可以花不到 30 美元获得[收听自动相关监视-Broadcas (ADS-B)](http://www.richardosgood.com/blog/2014/01/14/track-airplanes-with-rtl-sdr-and-ads-b/) (死链，尝试[互联网档案版本](https://web.archive.org/web/20140122012824/http://www.richardosgood.com:80/blog/2014/01/14/track-airplanes-with-rtl-sdr-and-ads-b/) ) 1090 MHz 模式“S”或 978 MHz 模式“UAT”信号定期从这些飞机上传输。

他指导我们配置无线电，使用更好的天线来改善接收效果，然后介绍详细的软件安装和设置，以控制无线电接收器，并将最终解码数据推送到映射软件。如果你住在商业航空公司附近，这看起来是一个迷人而有趣的项目。这种黑客行为不需要许可证，因为你只听不发，而且这些是合法接收的公开频道。

有些频率在法律上是不允许窃听的——住宅无线电话和蜂窝频率的私人通信，仅举几个例子([联邦法规第 47 篇第 15.9 部分](http://www.gpo.gov/fdsys/pkg/CFR-2012-title47-vol1/xml/CFR-2012-title47-vol1-sec15-9.xml))。所以请记住，即使您的设备没有受到此类接收的限制，您也必须小心，并保持在合法的频率范围内。还要注意，仅仅因为你有合法权利在某些频率上拦截对话或数据，公开分享拦截的内容或接收或解码的任何细节可能是非法的(只是为了记录而说)。

我们想知道[Rick]是否可以与[G. Eric Rogers]合作，升级[Eric]的[机动望远镜飞机跟踪系统](http://hackaday.com/2012/05/04/automatic-airplane-tracking-what-radar-systems-engineers-do-for-kicks/)，将无线电遥测数据推断为矢量数据，这样他的 Arduino 就可以不依赖视频信号进行跟踪。那次合并可能会让他们都上运输安全管理局的黑名单。

休息之后，请加入我们，获取一些额外的信息链接，并观看关于设置、安装和使用这种廉价飞机跟踪装置的视频。

维基百科上有关于 ADS-B 的更多细节，rtl-sdr.com 瞄准器在“ [RTL-SDR 教程:廉价 ADS-B 飞机雷达”上有一个很好的帖子，其中包括如何为 1090 MHz 频率建造自己的天线](http://www.rtl-sdr.com/adsb-aircraft-radar-with-rtl-sdr/)

[https://www.youtube.com/embed/sf1HL8qvx_o?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/sf1HL8qvx_o?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)