# Defcon Side Trip: Pololu 和机器人

> 原文：<https://hackaday.com/2014/08/23/defcon-side-trip-pololu-and-robots/>

在我们去拉斯维加斯参加 Defcon 期间，我们很幸运地找到了一些 Hackaday 读者可能会感兴趣的公司。总部设在该地区的公司之一是 Pololu(T2)，它是精细电子产品和机器人的制造商和供应商。在令人难以置信的幸运安排中， [LV Bots](http://www.lvbots.org/) ，拉斯韦加斯地区机器人建造者俱乐部，在我们在那里的同一个周末举办了一场活动。这是一个迷宫挑战，建造者将竞争建造最好的机器人，编写最好的代码，在最快的时间内让一堆电机和电子设备通过一个循线迷宫。

#### 男孩子

LV 机器人活动与 Pololu 在同一栋建筑中举行，不出所料，有不少 Pololu 员工尝试使用他们开发的东西，并让它穿过迷宫。至少有一个机器人是基于 Zumo 套件的，还有一些是基于 T2 3pi 平台的。有趣的是，Raspberry Pi 模型 B+是相当多机器人的大脑；这并不令人惊讶，但证明了 LV 机器人公司的人认真对待他们的循线迷宫*，并不断改进他们的构建。*

 *每个机器人和建造者团队都有三次机会。对于每个团队来说，第一次运行基本上致力于绘制整个迷宫。一个精心编程的算法试图让机器人绕过整个迷宫，并将所有的交叉点存储在内存中。对于第二次和第三次运行，机器人应该——理想情况下——在很短的时间内到达终点。这是最理想的情况，也是那个周末活动中唯一一个车队的代表。

最糟糕的情况是机器人没有正确的映射算法。例如:

[https://www.youtube.com/embed/1Sw2f_G4wM0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/1Sw2f_G4wM0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

然而，如果机器人能够找出地图上的所有节点，第二次和第三次运行会很快完成:

[https://www.youtube.com/embed/ggPLmUok-oA?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/ggPLmUok-oA?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

LV Bots 的工作人员也对整个竞争进行了总结:

[https://www.youtube.com/embed/h7kW9vi8dyQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/h7kW9vi8dyQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

#### 波洛卢

虽然我确实比正常工作时间晚到了一点，但[Ryan]和[Kevin]还是很友好地带我参观了他们的商店。这或多或少是你所期望的:一个巨大的房间，里面有取放机器、巨大的烤箱、锡膏分配器、足够的设备用于所有的测试和返工，还有一面巨大的墙，里面摆满了他们所有的产品。更有趣的设备之一是焊接机器人。是的，就像机器人拿着烙铁一样。以下是图片:

[![](img/1417ae6163b61a9f04cce5d0a69f3fc6.png)](https://hackaday.com/wp-content/uploads/2014/08/solderbot3.jpg)[![](img/9d6364a8a009e945c5827bbc8fa620a0.png)](https://hackaday.com/wp-content/uploads/2014/08/solderbot2.jpg)[![](img/b7efce723d2f25a97b1611ed7a666569.png)](https://hackaday.com/wp-content/uploads/2014/08/solderbot1.jpg)

几个小时后，机器不运转了。[Kevin]的确给我发了一段他们的 [A-Star 32U4 Micro](http://www.pololu.com/product/3101) 的制造过程的视频，如下图所示:

[https://www.youtube.com/embed/SQBhMQtHDaQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/SQBhMQtHDaQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

除了他们巨大的制造车间，这些人还带我去了他们的开发实验室，在那里他们提出了所有产品的设计。乐高玩具比比皆是，令人惊讶的是已经建成的配置。我会让图片库自己说话，如下所示。

* * *

### 男孩子

 [![Setting up for a run](img/d78e397063778aa510962f799b8a2415.png "LV Robots")](https://i0.wp.com/hackaday.com/wp-content/uploads/2014/08/lv-robots.jpg?ssl=1) Setting up for a run [![Blinky again](img/5c8d9418d118b3dc109f6f5df5fd6561.png "Ghost")](https://i0.wp.com/hackaday.com/wp-content/uploads/2014/08/ghost.jpg?ssl=1) Blinky again [![DSC_0003](img/eebbdc51cc0fa23eac6f3bead5c6c337.png "DSC_0003")](https://i0.wp.com/hackaday.com/wp-content/uploads/2014/08/dsc_0003.jpg?ssl=1)  [![DSC_0009](img/edaec6e0acf7554eb91006b2647f5917.png "DSC_0009")](https://i0.wp.com/hackaday.com/wp-content/uploads/2014/08/dsc_0009.jpg?ssl=1)  [![DSC_0023](img/ccdaa003ab05a99bf1cd30cef3130b1b.png "DSC_0023")](https://i0.wp.com/hackaday.com/wp-content/uploads/2014/08/dsc_0023.jpg?ssl=1)  [![LV Bots](img/27863f3b99d634e6fd61ba901f8e3612.png "LV Bots")](https://i0.wp.com/hackaday.com/wp-content/uploads/2014/08/lv-bots.jpg?ssl=1) LV Bots [![PacBot](img/3b1de9ae43a22fcb5329aaf5e02d495d.png "Wakka Wakka")](https://i0.wp.com/hackaday.com/wp-content/uploads/2014/08/wakka-wakka.jpg?ssl=1) PacBot [![DSC_0007](img/0c92e49ba0668322d61c09ae61e54ef1.png "DSC_0007")](https://i0.wp.com/hackaday.com/wp-content/uploads/2014/08/dsc_0007.jpg?ssl=1)  [![DSC_0005](img/f34f64051269ee9172ecfccaa2a20a08.png "DSC_0005")](https://i0.wp.com/hackaday.com/wp-content/uploads/2014/08/dsc_0005.jpg?ssl=1)  [![RaspiBotsB](img/7ab105ba5e31b4e41dc2d6dd8f141d95.png "RaspiBotsB")](https://i0.wp.com/hackaday.com/wp-content/uploads/2014/08/raspibotsb.jpg?ssl=1)  [![DSC_0030](img/4d55184a30226bf1f5dbf0fffa0332d4.png "DSC_0030")](https://i0.wp.com/hackaday.com/wp-content/uploads/2014/08/dsc_0030.jpg?ssl=1)  [![DSC_0004](img/95dda04db21d85a981fb5941b2f49e52.png "DSC_0004")](https://i0.wp.com/hackaday.com/wp-content/uploads/2014/08/dsc_0004.jpg?ssl=1)  [![The maze](img/655675715610e78c0dbbefe6d8b2ed9a.png "The maze")](https://i0.wp.com/hackaday.com/wp-content/uploads/2014/08/the-maze.jpg?ssl=1) The maze [![Blinky](img/90e6e2fe064a964461ef382ed1545233.png "DSC_0001")](https://i0.wp.com/hackaday.com/wp-content/uploads/2014/08/dsc_0001.jpg?ssl=1) Blinky [![DSC_0008](img/09c1a201cf5b82851fc74f5eb85c0eed.png "DSC_0008")](https://i0.wp.com/hackaday.com/wp-content/uploads/2014/08/dsc_0008.jpg?ssl=1) 

### 波洛卢

 [![The 'wall of samples'](img/d9d60f94fad9e2ba08fd8d304daf0169.png "DSC_0043")](https://hackaday.com/2014/08/23/defcon-side-trip-pololu-and-robots/dsc_0043/) The ‘wall of samples’ [![Thousands of dollars in pogo pins](img/224086b65bef9e73e103ea227c583d21.png "DSC_0052")](https://hackaday.com/2014/08/23/defcon-side-trip-pololu-and-robots/dsc_0052/) Thousands of dollars in pogo pins [!["The" Pololu](img/29ca958881743dcac3b86578e2a4980d.png "DSC_0044")](https://hackaday.com/2014/08/23/defcon-side-trip-pololu-and-robots/dsc_0044/) “The” Pololu [![Truly, important stuff happens in the design lab](img/f4596571c7bf1164c4b5723c83f290ac.png "Eggbot")](https://hackaday.com/2014/08/23/defcon-side-trip-pololu-and-robots/eggbot-2/) Truly, important stuff happens in the design lab [![DSC_0053](img/fa8d26cbadaf46db7da974fe0152b86b.png "DSC_0053")](https://hackaday.com/2014/08/23/defcon-side-trip-pololu-and-robots/dsc_0053/)  [![DSC_0055](img/7d5287f049e65d4fa1d9fd8d9ca03372.png "DSC_0055")](https://hackaday.com/2014/08/23/defcon-side-trip-pololu-and-robots/dsc_0055/)  [![DSC_0054](img/4a674b06194f2c907e9294985a72009f.png "DSC_0054")](https://hackaday.com/2014/08/23/defcon-side-trip-pololu-and-robots/dsc_0054/)  [![Hundreds of steppers](img/6339226c8ae71b60d77c26ba6c2ed94c.png "DSC_0039")](https://hackaday.com/2014/08/23/defcon-side-trip-pololu-and-robots/dsc_0039/) Hundreds of steppers [![DSC_0056](img/9e852b2c2ee6617cc4138e7cb4c21f41.png "DSC_0056")](https://hackaday.com/2014/08/23/defcon-side-trip-pololu-and-robots/dsc_0056/)  [![Shop floor](img/4e2047858e0d5099b126ad72f9c8d7e1.png "DSC_0042")](https://hackaday.com/2014/08/23/defcon-side-trip-pololu-and-robots/dsc_0042/) Shop floor [![DSC_0041](img/04262eb194951036f7579690b0a63835.png "DSC_0041")](https://hackaday.com/2014/08/23/defcon-side-trip-pololu-and-robots/dsc_0041/)*