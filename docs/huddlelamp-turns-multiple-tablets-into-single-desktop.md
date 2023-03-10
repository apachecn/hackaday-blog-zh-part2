# HuddleLamp 将多台平板电脑变成单一桌面

> 原文：<https://hackaday.com/2014/10/24/huddlelamp-turns-multiple-tablets-into-single-desktop/>

想象一下，你有一群人围着桌子坐着，他们有各种各样的移动显示设备，你希望这些设备一起行动。也许你希望它们是一个更大的显示器上的窥视孔，当你在桌子上移动它们时，可以显示显示器的不同部分。或者，您可能希望能够通过手指手势在这些设备之间拖放。HuddleLamp 让你做到这一切。

它是如何工作的？基本上，一个 3D 摄像机位于桌面上方，监视你的移动显示器和你的手。通过机器视觉的魔力，服务器将正确的图像发送到组中的每个屏幕。(HuddleLamp 中的“灯”是布置在空间上方的台灯，内置 3D 摄像头。)

一个非常好的接触是，作者还提供了 JavaScript 对象，您可以将这些对象嵌入到 web 应用程序中，使设备能够加入群组，而无需下载特殊的软件。一个新的设备会闪现一个计算机视觉程序可以识别的识别模式。一旦完成，服务器开始将整个显示的正确部分发送到新设备。

休息时间下方的视频展示了可能的互动。

[https://www.youtube.com/embed/XkmwG588zp0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/XkmwG588zp0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

如果你想更深入地了解它们是如何协同工作的，下载他们的论文(PDF 格式)并阅读一下。它详细介绍了屏幕检测所需的一些设计选择，以及如何将来自 3D 相机的深度数据与普通图像流集成在一起。