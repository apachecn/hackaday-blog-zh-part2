# 天才少年黑客的眼控轮椅进展

> 原文：<https://hackaday.com/2015/05/28/eye-controlled-wheelchair-advances-from-talented-teenage-hackers/>

来自德国杜伊斯堡的 14 岁和 15 岁的孩子米里贾姆·斯托泽尔和她的朋友保罗·福尔廷正在制作一款眼球运动控制器轮椅。他们受到了 [Eyewriter 项目](http://eyewriter.org/)的启发，我们已经[跟踪这个项目很长时间了](http://hackaday.com/2009/11/11/eyewriter-is-the-fruit-of-the-kaneye-project/)。Eyewriter 是 Tony Quan 的朋友为他建造的。2003 年，Tempt1 被诊断出患有退行性神经疾病 ALS，现在除了眼睛之外完全瘫痪，但已经能够使用眼睛作家继续他的艺术。

这是他们从乐高头脑风暴开始的第一次飞跃。眼球跟踪器部分由一个安全玻璃框架、一个常规网络摄像头和 IR SMD LEDs 组成。他们从网络摄像头上移除了红外阻挡过滤器，使其在所有照明条件下都能工作。图像处理由 Odroid U3 处理，这是一款紧凑的低成本 ARM 四核 SBC，能够运行 Ubuntu、Android 和其他 Linux OS 系统。他们最初尝试了 Raspberry Pi，与 Odroid 的 13~15fps 相比，它只能做到大约 3fps。代码是用 Python 写的，使用 OpenCV 库。他们正在学习 Python。Arduino 用于通过 H 桥控制器控制电机，也用于校准眼球跟踪器。连接到 Arduino 模拟端口的电位计允许根据个人需求调整跟踪器。

过滤网络摄像头视频流以获得瞳孔位置，并将其与前、后、左、右四个预设位置进行比较。可以使用电位计调整预设。目前手动激活的启动开关用于确保轮椅仅在被命令时移动。他们的计划是以后用舌头激活或者脸颊肌肉抽搐检测来代替这个开关。

第一次测试是在一个小型机器人平台上进行的。在当地的一次比赛中获胜后，他们买了一把二手轮椅，重新开始。这一次，他们尝试了树莓 Pi 2 model B，它能够以大约 8~9fps 的速度工作。没有 Odroid 好，但价格是它的一半，这似乎是一个可行的解决方案，因为他们的目标是尽可能便宜。他们希望获得任何帮助来提高性能——可能是改进他们的代码或更有效地利用所有四个内核。对于更大的轮椅，他们使用回收的汽车挡风玻璃刮水器电机和一些继电器来开关它们。他们还使用 3D 打印机打印了摄像机的外壳和帮助轮椅转向的轮子。更多细节也可在[【myri jam】的博客](https://zerozeroonezeroonezeroonezero.wordpress.com)上获得。他们[记录了他们的建造](https://zerozeroonezeroonezeroonezero.files.wordpress.com/2015/05/paper_auge-rollstuhl-jufo2015_stoetzer-foltin.pdf)(德语，pdf)，并把目光投向了德国国家科学博览会。该团队正在进行文档的英文翻译，并将很快在 NC 许可下发布所有设计文件和源代码。