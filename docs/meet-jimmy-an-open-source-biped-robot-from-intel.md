# 认识一下 Jimmy:来自英特尔的开源双足机器人

> 原文：<https://hackaday.com/2014/05/29/meet-jimmy-an-open-source-biped-robot-from-intel/>

![Jimmy_Arm_Up](img/af4c8186309658c27e6f0f0139bcfd32.png)

英特尔首席执行官[布莱恩·科兹安尼克]在 Re/Code 大会上宣布了吉米，这是 21 世纪机器人项目的第一个机器人。这个项目是英特尔常驻未来学家布莱恩·戴维·约翰逊的主意。我们喜欢这个项目的宣言:

> 机器人是:先想象出来的。易于构建。完全开源。极度社会化。有意迭代。充满人性和梦想。为她/他/自己着想。

吉米可能还没有达到这些水平，但他绝对令人兴奋。首先，他不是建在英特尔总部的秘密实验室里。吉米的大部分工作都是在 Trossen Robotics 公司完成的，这个名字在 Hackaday 很出名。Trossen 的[Matt]和[Andrew]描述了休息后他们视频中的所有细节。

这个版本的吉米是一个研究机器人，这意味着他不会便宜。吉米展示了英特尔 i5 NUC 主板、20 个 Dynamixel 伺服系统、5052 铝制框架和一系列传感器。一个 4S 14.8v 4000mAh LiPo 电池可以为吉米提供 30 到 60 分钟的充电时间，所以一定要准备一些备用电池。吉米最引人注目的地方是他的 3D 打印外壳。21 世纪机器人项目给了他大而友好的眼睛和特征，这肯定会有助于他们目标的社会方面。

Jimmy 完全是关于开源的。他可以运行两种版本的 Linux: Ubuntu 14.04 LTS 版或 Yocto Pokey 的定制版。在相同的硬件上运行和开发有很多优点。没有专门的工具链用于交叉编译，没有 NFS 共享来移动二进制文件。如果你需要做出改变，你可以插上显示器(或启动 VNC 会议)，用吉米的车载电脑做任何事情。Jimmy 的软件栈是基于 DARwIn OP T1 平台的，ROS 移植也在进行中。

我们对吉米很感兴趣，但他的价格是 16，000 美元，有点超出我们的预算。值得庆幸的是，一个更小的 Jimmy 消费者版本很快就可以买到，价格大约是它的十分之一。

[https://www.youtube.com/embed/wRZn7_lpD2U?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/wRZn7_lpD2U?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[https://www.youtube.com/embed/YCd4glKBCxM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/YCd4glKBCxM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)