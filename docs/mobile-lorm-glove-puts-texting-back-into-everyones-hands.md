# 移动 Lorm 手套让发短信回到每个人手中

> 原文：<https://hackaday.com/2015/03/16/mobile-lorm-glove-puts-texting-back-into-everyones-hands/>

如果你一直在通过智能手机和你的朋友发短信或聊天来消磨时间，很可能你没有太多考虑让这一切发生的两个感官:你的视觉和听觉。然而，聋哑人不能参加这些活动；对许多人来说，我们大多数人喜欢用手机进行的远程交流是不可能的。进入柏林艺术大学设计研究实验室。在这里，他们开发了[移动 Lorm 手套](http://www.design-research-lab.org/projects/mobile-lorm-glove/)，这是一种通过智能手机实现双向远程通信的触觉设备。

对于聋哑人来说，Lorm 是一种用于交流的触觉技术。Lorm 是一系列映射到字母表字符的手势。为了与他人交流，戴手套的用户可以直接在手掌上的压敏输入上追踪 Lorm。为了接收信息，手背上的小型振动马达振动，以指示 Lorm 中编码的信息。

本来，要和聋哑人交流，就要先学会 Lorm。然而，使用移动 Lorm 手套，我们只需知道如何发送文本消息，Lorm 解码由运行在经典 Atmega328 微控制器上的查找表处理。对于目光敏锐的人来说，手套的背面似乎在将连续的手指轨迹转录成离散的运动振动方面能力有限。然而，由于有四个移位寄存器和 32 个运动强度级别，设计者用一种称为“漏斗幻觉”的技术来处理每个马达，通过逐渐改变马达之间的强度来模拟连续运动。更多技巧和细节，看一下他们的[会议论文](http://www.tiii.be/wp-content/uploads/2012/03/127-248-gollner.done_.pdf)。

戴上这种手套，与任何拥有智能手机的人进行日常交流都会变得更加容易。我们感到高兴的是，仅仅一个蓝牙模块、一个 Atmega328 和一组压力传感器和马达就可以让任何手机用户绕过学习曲线，开启新的对话。

[https://www.youtube.com/embed/FLfa9ni7X3I?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/FLfa9ni7X3I?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)