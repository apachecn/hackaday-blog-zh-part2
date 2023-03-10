# TorqueScreen:移动中的触觉反馈

> 原文：<https://hackaday.com/2015/01/26/torquescreen-haptic-feedback-on-the-go/>

如果你在过去的 15 年里一直在使用任何游戏机视频游戏(或者你已经获得了一部智能手机)，你就会知道“隆隆声”或“触觉”反馈在增强我们的屏幕(或触摸屏打字)体验方面发挥着关键作用。然而，这种隆隆声反馈令人惊讶地是布尔型的，自从 30 多年前开始在游戏中引入以来，还没有发展到更高的精度水平。作为回应，奥地利萨尔茨堡大学的[Martin]和他的设计队友推出了 [TorqueScreen](http://dl.acm.org/citation.cfm?id=2680579) ，这是一种移动触觉附件，对传统的力反馈进行了扭转。

扭矩屏幕的核心是一个陀螺仪，它连接到一个伺服系统，各自的旋转轴垂直对齐。当伺服旋转活动陀螺仪时，用户可以感觉到平板电脑绕伺服轴旋转的阻力。

该团队的会议演示模型采用了一个从旧硬盘中取出的无刷电机，由 Arduino 控制，由 Wii 双节棍手动驱动。目前只有一个旋转轴阻止旋转的变化，但万向节可能是这个项目的下一步。

我们以前肯定见过 budget [手持触觉设备](http://hackaday.com/2014/03/26/piezos-for-haptic-feedback/)，但这个项目允许响应的整个范围与陀螺仪绕伺服轴旋转的速度成比例。

除非你是在已经具备 torquescreen 功能的移动设备上阅读这篇文章，否则很难感觉到你可以用这个设置产生什么样的交互。不过，这个视频(休息之后)可以让你很好地了解你希望夹在平板电脑上的设备具有什么样的交互性。

[通过[有形、嵌入式和具体化交互会议](http://www.tei-conf.org/15/)

[https://www.youtube.com/embed/F9qThNldm2U?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/F9qThNldm2U?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)