# 嘉实多虚拟漂移:戴着虚拟现实头盔的司机以每小时 80 英里的速度编写代码

> 原文：<https://hackaday.com/2015/06/20/castrol-virtual-drift-hacking-code-at-80mph-with-a-driver-in-a-vr-helmet/>

驾驶一辆全新的 [670 马力的 Roucsh stage 3 野马，同时戴着虚拟现实护目镜](http://masterofshapes.com/castrol-virtual-drift/)。听起来很疯狂，对吧？这正是嘉实多油的广告公司想出来的。他们不想只是拍广告，他们想做真实的东西。进入[Adam 和 Glenn]环节，他们是负责将数据从汽车传输到高端游戏电脑的工程师。计算机在虚幻引擎下运行自定义模拟。埃尔托罗机场提供了一大片空旷的停机坪，让汽车行驶时不用担心撞到任何现实世界的障碍物。

Oculus Rift 从未被设计成在移动的车辆内操作，因此它对[亚当和格伦]提出了独特的挑战。每当汽车转向或旋转时，Oculus 的车载惯性测量单元(IMU)就会认为司机[Matt Powers]在转头。有一次[马特]试图开车，而游戏引擎让他坐在乘客座位上转向一边。解决方案是在车上安装一个 9 自由度的 IMU，然后从裂缝中减去该 IMU 的运动。

GPS 数据来自一个[实时动态(RTK) GPS 单元。](https://en.wikipedia.org/?title=Real_Time_Kinematic)不幸的是，GPS 的更新速率为 5Hz 对于时速接近 100 英里的汽车来说还不够快。在模拟开始时，GPS 被认为是虚拟世界和现实世界的结合。其余数据来自 IMU 和汽车自带的 CAN 总线。【亚当和格伦】使用了一个带有[微芯片 mcp2515 can 总线接口](http://www.microchip.com/wwwproducts/devices.aspx?dDocName=en010406)的 Arduino 来读取诸如转向角、油门位置、刹车压力和车轮打滑的数值。数据然后被传递给虚幻引擎。[Arduino 代码已在 Github](https://github.com/theDrGray/castrolVR) 上发布，尽管该团队不得不清理一些福特专有的 CAN 消息数据以避免诉讼。值得注意的是，[亚当和格伦]在这一点上没有得到福特的任何支持，他们只是嗅了嗅 CAN 网络，以确定每个消息 ID。

最终的视频有好莱坞的待遇。“游戏中”的镜头已经被预先渲染的序列取代，看起来如此之好，以至于我们会认为整个事情都是假的，如果我们不知道的话。

点击过去的最后广告和一些幕后镜头的休息。

[https://www.youtube.com/embed/PX_HAIOQYes?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/PX_HAIOQYes?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[https://www.youtube.com/embed/fkobHlXKFY8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/fkobHlXKFY8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[https://www.youtube.com/embed/zZiM-8TTkmM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/zZiM-8TTkmM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)