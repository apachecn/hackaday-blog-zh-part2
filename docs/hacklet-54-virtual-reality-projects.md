# hack let 54–虚拟现实项目

> 原文：<https://hackaday.com/2015/07/03/hacklet-54-virtual-reality-projects/>

虚拟现实终于成熟了。黑客、制造商和工程师多年来一直梦想创造沉浸式界面。从第一个飞行模拟器到今天的手机供电的头戴显示器，虚拟现实一直是一个令人兴奋的领域。今天的许多进步都是由黑客创造的，他们受到了 20 世纪 90 年代早期的虚拟系统的启发。25 年后的今天，我们看到了惊人的进步——不仅是在商业系统中，也在开源虚拟现实项目中。本周的 Hacklet 是关于 [Hackaday.io 上最好的虚拟现实项目！](https://hackaday.io)

[![vr1](img/7a4404d8d9a3bf3bc1a292c5c1dda708.png)](https://hackaday.io/project/6442) 我们从【j0nno】和 [D.I.Y 虚拟现实](https://hackaday.io/project/6442)开始。【J0nno】对 VR 产生了兴趣，决定自己打造头戴显示器。他的目标是创建一个具有全头部跟踪和开源软件栈的设置。他希望在 200 澳元的预算内完成这项工作。[J0nno]从 Ritech3d-V2 VR 护目镜开始，这是谷歌 cardboard 项目的塑料实现。为了显示，他使用了 5.6 英寸 1280 x 800 TFT LCD。跟踪是光学的，使用红外发光二极管和 PS3 眼睛摄像头。[J0nno]的背景是软件，所以他在设置 [OpenVR](http://mclightning.com/openvr/) 和[感知](https://github.com/cybereality/Perception)方面做得很好。硬件方面对他来说有点陌生。但是这并没有阻止[j0no ]!本着真正的黑客精神，他在从事 D.I.Y 虚拟现实工作时，正在学习所有关于电阻和驱动 led 的知识。

[![vr2](img/1dba8809c0f3c3864f435789e4999b01.png)](https://hackaday.io/project/1972) 接下来是【乔希·林赛】带着[数码手套:最后的动作捕捉手套](https://hackaday.io/project/1972)。Digitabulum 是一款动作捕捉手套，旨在能够模仿大多数其他动作捕捉系统。它还被设计成成本相对较低。每手 400 美元，比大多数其他产品都便宜，尽管我们仍然希望看到更便宜的东西。[Josh]正在使用惯性传感器，而且有很多。具体来说，他使用了不少于 17 个来自 ST 微电子公司的 [LSM9DS1](http://www.st.com/web/catalog/sense_power/FM89/SC1448/PF259998) 惯性测量单元(IMU)传感器。像这样的 IMU 传感器将多个速率陀螺仪、加速度计和磁力计集成到一个单元中。基本上每个手指的每个部分都有自己的传感器套件。正如你可能想象的那样，这是相当多的数据要处理。Altera Max II CPLD 和 ST Arm 处理器有助于将数据浓缩为 VR 引擎可以处理的内容。[Josh]已经在这个项目上工作了一年多，他取得了很大的进展。原型手套看起来棒极了！

[![vr3](img/9ca8b352dbcf110b23b8ad458b2b2160.png)](https://hackaday.io/project/1689) 【托马斯】用 [Oculus Rift 特色的起重机控制](https://hackaday.io/project/1689)将增强现实带到桌面上。起初只是业余爱好的实验变成了[托马斯的]大学主要项目。他把 Oculus Rift 连接到一个玩具起重机上。起重机上的立体摄像机向操作员发送视频图像。摄像机安装在由 Rift 头部跟踪单元驱动的云台机构上。简单的操纵杆控制允许[Thomas]移动动臂和降下绳索。屏幕显示显示起重机的当前状态。裂缝的使用使这成为一个身临其境的演示。人们可以很容易地看到，将这一系统应用到现实世界中会使起重机操作对起重机操作员来说更加安全。

[![vr4](img/609fa43696e12e42101372864510b3d5.png)](https://hackaday.io/project/5935) 终于有了【阿卡迪亚实验室】配 [DIY 增强现实设备](https://hackaday.io/project/5935)。这个项目是 2015 年 Hackaday 奖的[Arcadia Labs]参赛作品，它使用两个 320 x 240 的屏幕来创建一个增强现实头戴显示器。虽然分辨率比不上 Oculus Rift 或 HTC Vive，但[阿卡迪亚实验室]对此还可以。他们正在寻求一种成本更低的开源增强现实替代方案。跟踪是通过 IMU 实现的，而 PS3 眼睛摄像头提供视频。一个树莓皮控制了这场表演。仅仅使用 Pi 的 SPI 接口,[Arcadia Labs]就能够在显示器上获得每秒 50 帧的画面，然而 USB PS3 Eye camera 将事情限制在每秒 10 帧左右。这个项目现在正在紧张的开发中，所以和我们一起去看看[阿卡迪亚实验室]的结局吧！

如果你想要虚拟现实的好处，看看我们新的[虚拟现实项目列表！](https://hackaday.io/list/6571-virtual-reality-projects)我错过了你的项目吗？不要害羞，只要[在 Hackaday.io](https://hackaday.io/adam) 上给我留言。如果你在美国的左海岸，去看看[社会虚拟现实会议和博览会](http://www.socalvr.com/)。Hackaday 是赞助商。这项活动将于 7 月 12 日在加州大学欧文分校举行。

这就是本周的 Hacklet，一如既往，下周见。同样的黑客时间，同样的黑客频道，带给你最好的 Hackaday.io！