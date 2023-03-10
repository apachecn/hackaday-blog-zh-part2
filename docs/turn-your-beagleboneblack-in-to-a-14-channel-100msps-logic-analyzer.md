# 将你的 BeagleBoneBlack 放入 14 通道、100Msps 逻辑分析仪中

> 原文：<https://hackaday.com/2015/02/19/turn-your-beagleboneblack-in-to-a-14-channel-100msps-logic-analyzer/>

鉴于其强大的功能，BeagleBoneBlack 是许多黑客的首选 SoC 这是理所当然的。[abhishek]来自印度 IIT-哈拉格普尔，主修 E&E，2014 年通过谷歌代码项目之夏(GSoC)申请了 beagleboard.org 的一个项目。他的项目 [BeagleLogic](https://github.com/abhishek-kakkar/BeagleLogic/wiki) 旨在使用 AM335X SoC 系列上的可编程实时单元实现一个逻辑分析仪，为 BeagleBone 和 BeagleBone Black 供电。

该项目有助于创建 PRU 与 sigrok 的绑定，还提供了一个基于 web 的前端，以便可以访问逻辑分析器，就像在 BeagleBone/BeagleBone Black 上使用 Cloud9 IDE 创建一个带有 BoneScript 的新应用程序一样。

除了作为调试工具的明显用途外，逻辑分析仪还可以作为学习工具，用于理解数字信号。BeagleLogic 将 BeagleBone Black 变成 14 通道、100Msps 逻辑分析仪。一旦被加载，它就以角色设备节点 **/dev/beaglelogic** 的形式出现。在独立模式下，它可以进行二进制捕获，无需任何特殊的客户端软件。当与 [sigrok 库](http://www.sigrok.org/)结合使用时，BeagleLogic 支持 30 多种不同数字协议的软件触发和解码。

该分析仪能够以 8 或 16 位对 10Hz 至 100MHz 的信号进行采样，最多可达 14 个通道。样本深度取决于可用内存，最多可为 BeagleLogic 保留 320MB。还有一个 web 界面，一旦安装在 BeagleBone 上，就可以从端口 4000 访问，并可用于少量捕获(最多 3K 样本)。

【abhishek】最近增加了 [BeagleLogic Cape](http://theembeddedkitchen.net/introducing-the-beaglelogic-cape/295) ，可以用来安全调试高达 5V 的逻辑电路。BeagleLogic 和[海角](https://github.com/abhishek-kakkar/BeagleLogic/wiki/The-BeagleLogic-Cape)的源文件可以通过他的 github repos 获得。[abhishek]在他的[网站](http://theembeddedkitchen.net/)上写了关于他的项目的博客，在那里可以找到更多的信息和链接。休息之后看一段 BeagleLogic 的视频。

[https://www.youtube.com/embed/CDbEAq33vdA?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/CDbEAq33vdA?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)