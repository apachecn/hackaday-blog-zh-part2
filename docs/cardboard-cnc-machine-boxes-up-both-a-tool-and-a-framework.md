# 硬纸板数控机床既是工具又是框架

> 原文：<https://hackaday.com/2015/03/01/cardboard-cnc-machine-boxes-up-both-a-tool-and-a-framework/>

想建立一个桌面数控机床，而不打破你的钱包？麻省理工学院媒体实验室的詹姆斯·科尔曼(James Coleman)、纳德亚·皮克(Nadya Peek)和伊兰·莫耶(Ilan Moyer)发明了一种模块化纸板 CNC(T1 ),它为你设计自己的机器提供了基础。

CNC 构建包括单轴线性工作台和单轴旋转工作台的设计说明，以及如何将多个轴组合在一起以构建特定机器的一些想法。无论是铣削木材、激光雕刻桌子，还是移取细菌样本，设计[[drop box](https://www.dropbox.com/s/aaw6ppl13x39pge/CRDBRD_STAGE.dxf?dl=0)和物理组件都可以满足您的最终应用。

也许这个项目最有趣的方面是，在高层次上，它不仅仅是一个 cnc，而是一个被称为*完形*的框架。这种体系结构使用户能够开发自己的机器配置，包括用高级 Python 代码链接在一起的多个软件节点。大多数高级计算是由调用编译 C 代码的 Python 库组织的。这个高级框架通过所需机器的运动学来处理指令，以向电机控制器输出命令。最后，顶层接口用两种替代方法抛弃了陈旧的 GCode:一个 Python 接口包含对过程的函数调用，一个远程接口通过 http 请求进行过程调用。而运动控制语言的缺点是命令没有标准化；然而，它们更容易被人阅读，这一点有利于格式塔框架的目标“被个人使用”

[![gestaltFramework](img/53aa7402821d7dbe04176ee606341034.png)](https://hackaday.com/wp-content/uploads/2015/02/gestaltframework.png)

在论文[ [PDF](http://www.pygestalt.org/VMC_IEM.pdf) ]中，[Ilan]表达了工具作为阻抗匹配设备的概念，这是一种扩展我们创造力的工具，可以将更广泛的形状弯曲和变形为我们想象的形式。当我们的手不够精确和脆弱时，工具可以弥补这个缺陷。格式塔和 Cardboard CNC 是创建一个框架的第一步，这样任何人都可以设计和实现自己的阻抗匹配设备，无论他们是编织钢缆还是雕刻木头。

麻省理工学院媒体实验室的人是这个低成本机械领域熟悉的重量级人物，尤其是那种可以装进手提箱的机械。我们很高兴看到一个直接面向社区的建筑。

via[[CreativeApplications.net](http://www.creativeapplications.net/objects/make-something-that-makes-almost-anything-cardboard-cnc/)