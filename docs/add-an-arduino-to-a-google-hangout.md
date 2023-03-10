# 将 Arduino 添加到 Google+ Hangout

> 原文：<https://hackaday.com/2012/10/22/add-an-arduino-to-a-google-hangout/>

[![](img/2412c3ff8eee873f00ecbd1df1064289.png "Google+ Hangout Arduino Control")](http://hackaday.com/?attachment_id=88603)

Google+ Hangouts 提供群组视频聊天功能，可以添加应用程序。[RobotGrrl]创建了一个 Node.js [web 应用程序来控制可以添加到 Hangout 的 Arduino](http://robobrrd.com/learn/googleplus/ "Arduino Web App") 。

有一个 Javascript 客户端运行在 Hangout 内部，并通过 WebSockets 与运行在 EC2 服务器上的 Node.js 服务器通信。服务器接收该客户端数据，并使用 TCP 套接字发送命令进行处理。Processing 处理与 Arduino 的通信，允许您从 Hangout 控制许多事情。

在这个简单的例子中，[RobotGrrl]演示了如何从 Hangout 切换 LED。这包括设置 EC2 实例的教程、服务器和客户端应用程序的完整源代码、控制 Arduino 的处理草图以及允许将应用程序添加到 Hangout 的代码。

这个例子展示了一些基本的东西，但是有很多东西可以用这个系统来控制。[RobotGrrl]甚至演示了一些从悬挂界面控制的机器人。

休息之后，请观看视频概述。

[https://www.youtube.com/embed/Y1bdxf9tZWw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/Y1bdxf9tZWw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)