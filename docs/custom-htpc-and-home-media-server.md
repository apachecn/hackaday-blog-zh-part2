# 自定义 HTPC 和家庭媒体服务器

> 原文：<https://hackaday.com/2013/10/07/custom-htpc-and-home-media-server/>

[Benoit Frigon]的建造是对整洁的致敬:他的 HTPC 和 T2 媒体服务器都是充满功能的优雅作品。他有相当的诀窍在这种形式的因素干净的构建；[他的 PBX 服务器](http://hackaday.com/2013/06/19/pbx-blade-for-multiple-extension-home-telephony/ "PBX blade for multiple extension home telephony")在今年夏天早些时候获得了高度赞扬。

对于 HTPC，[Benoit]掏空并清洗了一个旧的 DVR 机箱，并对其进行了改造，以容纳一个迷你 ITX 板。他增加了支架来支撑主板，然后草拟了 IO 防护罩的模板，作为切割背板的指南。DVR 外壳的正面最初有一个 4 位 7 段显示器和几个简单的按钮。虽然[Benoit]保留了原来的按钮布局，但他选择用 20×2 字符的 LCD 来代替分段显示。新的显示器通过 HTPC 上的 python 脚本来控制，该脚本运行 XBMC 12.0 的 OpenElec Linux 发行版。

如今，HTPC 的硬盘托架变得更轻了，因为[Benoit]决定将他的媒体存储迁移到一个单独的服务器上。在新的家庭媒体服务器内部是另一个迷你 ITX 主板，内置运行 Ubuntu Server 的 Atom N2800。通过 [WinTV HVR-2550 电视调谐器](http://www.hauppauge.com/site/products/data_hvr2250.html)和 [TVHeadend 软件](https://tvheadend.org/)进行电视直播。外壳最初将调谐器悬挂在背面的 IO 支架上(其他地方都没有)，这使得卡的其他部分在内部没有支撑，非常危险。[Benoit]通过构建一个额外的铝制支架来牢固地固定 PCIe 竖板和调谐器，解决了这个问题。查看两个版本的页面，获取可下载的模板、软件详情和材料清单。