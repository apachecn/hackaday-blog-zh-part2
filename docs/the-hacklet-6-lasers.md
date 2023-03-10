# 小窍门 6——激光

> 原文：<https://hackaday.com/2014/07/04/the-hacklet-6-lasers/>

![Hacklet 6](img/e0fc0854c08d7bc2c8c0c74194b09536.png)

本周的黑客攻击都是关于激光的，自 1960 年以来，激光一直为黑客们提供单色光。[[西奥多·梅曼](http://en.wikipedia.org/wiki/Theodore_Maiman)演示了第一台工作的激光器，他自己也是一名黑客/制造者，在他父亲的家用电子实验室里学过电路。从那以后，激光在黑客社区中变得非常流行，这并不奇怪。

[![laserwelder](img/435649fb5d799406b50f1e510fa2eefc.png)](http://hackaday.io/project/189-Laser-Welder-Retrofit) 【麦曼的】第一个激光是用闪光管泵浦的，类似于【麦康纳的】项目中的 YAG 激光来[恢复一个激光焊机](http://hackaday.io/project/189-Laser-Welder-Retrofit)。他得到了一台 1985 年的 400W Lumonics 激光焊接机。这台焊机最初是泰克买的，用来焊接钛 CRT 法兰。随着时间的推移，电焊机被卖给了(麦康纳的)公司，这家公司一直使用它，直到阿诺拉德控制系统失灵。人们努力用新的伺服系统和开放式 CNC 控制系统来更新它，但这项工作从未完成。这台激光器在[macona]买下之前已经用了 12 年，现在他用 LinuxCNC 让它起死回生。该项目有了一个辉煌的开端，因为他已经有了输出约 200 瓦的激光。

[![d0c96d91](img/8ce01d6b385a4dfc370f8ebbc84b6de3.png)](http://hackaday.io/project/1025-650nm-5mw-Laser-Build) 在稍微低一点的功率方面我们有【雷霆之声】 [5mW 可见红色(650nm)激光](http://hackaday.io/project/1025-650nm-5mw-Laser-Build)。[ThunderSqueak]在她的其他项目中需要一个具有良好聚焦光学系统的校准激光器。她在一个塑料盒子里安装了一个模块，并增加了一个开关。一个快速的构建，但它在她的一些更大的项目上获得了回报——比如她的[低成本二氧化碳激光构建](http://hackaday.io/project/1023-Low-Cost-CO2-Laser-Build)，我们[早在 5 月份就在博客](http://hackaday.com/2014/05/05/building-a-co2-laser-in-a-hardware-store)上对其进行了专题报道。

[![la-cutter](img/987143f25bd5a4745b880fef622931ab.png)](http://hackaday.io/project/316-Simple-DIY-laser-cutter)

[phil]使用 buildlog 2.x 作为他的[简易 DIY 激光切割机](http://hackaday.io/project/316-Simple-DIY-laser-cutter)的灵感。激光功率来自低成本的 K40 激光管和激光头。他的框架是铝挤压成型，表面覆盖着 [Dibond](http://graphicdisplayusa.com/en/products/dibond/dibond/) ，这是一种用于户外招牌的铝复合材料。动力来自 NEMA 17 步进电机。[phil 的]许多零件都是由 HDPE 塑料加工而成的，尽管看起来它们也可以 3D 打印。我们打赌这个建成后会是一个真正的工作狂。

[![la-cutter2](img/f149835844c189d5dd5726b4dd38ab41.png)](http://hackaday.io/project/361-Homemade-PCB-Mill-%2F-Laseretcher)【ebrithil】正在研究一种组合[激光雕刻机/PCB 蚀刻机](http://hackaday.io/project/361-Homemade-PCB-Mill-%2F-Laseretcher)，它将使用固态激光模块。他的布局是许多其他工厂和 3D 打印机上看到的标准龙门系统。Y 轴上的双步进器增加了对中央皮带的需求。他的 Z 轴是一个旧 DVD 驱动器捐赠的。它有足够的力量举起一支笔，并应该足够准确地聚焦任务。他已经用低功率紫色激光和黑暗物质进行了几次很好的测试。

[![openexposer](img/63c0b3fcdbdc5f1ce55cebc6991ad135.png)](http://hackaday.io/project/1129-OpenExposer-) 【马里奥】正在他的 [OpenExposer](http://hackaday.io/project/1129-OpenExposer-) 中创造一个令人难以置信的可变激光工具，它可以做任何事情，从立体印刷 3D 打印到用激光竖琴制作音乐。这里的天才之处在于[马里奥]对激光打印机零件的重复利用。每台激光打印机都使用相同的基本设置:一台激光器，一面扫描镜，以及将光束扩展到整个页面宽度的光学元件。[Mario]已经从 OpenExposer 得到了一些很棒的照片。这个项目是[hack aday 奖的看点之一。](http://hackaday.io/prize)

[![ramenspec](img/d4301276899e3fe003d44e09f7d6093f.png)](http://hackaday.io/project/1279-DIY-3D-Printable-RaspberryPi-Raman-Spectrometer)【fl @ C @】正在用他的 [DIY 3D 可打印 RaspberryPi 拉曼光谱仪](http://hackaday.io/project/1279-DIY-3D-Printable-RaspberryPi-Raman-Spectrometer)挖掘事物的物理学一面。拉曼光谱仪通常非常昂贵，它能告诉我们给定的材料样品由哪些元素组成。[fl @ C @]激光器是一种 532 纳米 150 兆瓦的激光器，它通过令人眼花缭乱的镜子和透镜阵列反弹。得到的数据被一个树莓 Pi 处理，给出一个完整的光谱分析。[fl @ C @]参加了他的项目 Hackaday Prize，我们在六月份的时候特别报道了他的简历。

这就是本周的小技巧，直到下周，不要只是坐在那里想知道[为什么激光没有做很酷的事情](https://www.youtube.com/watch?v=MJ8UlkFj-1E)。让它发生，并张贴在 [Hackaday.io](http://hackaday.io/) 上！