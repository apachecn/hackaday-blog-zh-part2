# BrickPi Bookreader 1 和 2 朗读平板电脑或书籍，您可以选择

> 原文：<https://hackaday.com/2014/05/10/brickpi-bookreader-1-and-2-read-tablets-or-books-aloud-you-choose/>

![BrickPi Bookreader 2](img/13ef2e8d7c116b565fcee01b3a5548ef.png)

你是否曾经想看一本好书放松一下，但由于不得不实际阅读和翻页的麻烦而无法做到？好吧，现在 BrickPi 为这个问题提供了两个解决方案。无论您的文档是在平板电脑上还是在实体书上，它们都能帮您解决问题。

原始的[阅读器](http://www.dexterindustries.com/BrickPi/projects/brickpi-bookreader/)将大声读出平板电脑上显示的文本。![brickpi bookreader](img/64875b39014c3a64c1f578ff20770ec1.png)这不是一个在平板电脑上运行的应用程序，它是一个完全独立的设备，可以“读取”平板电脑屏幕。正如你从 BrickPi 的名字可以猜到的那样，这个操作背后的大脑是一个树莓 Pi。相机拍摄显示文本的照片，Raspberry Pi 使用光学字符识别将该图像文件转换为文本。然后，文本到语音引擎用机器人发出的声音朗读文本。为了改变页面，Raspberry Pi 控制乐高 Mindstorms 手臂在平板电脑屏幕上滑动，整个过程重复进行。

BrickPi 收到了许多关于 Bookreader 的反馈，要求提供一个可以阅读真正书籍并翻页的版本。进入[阅读器 2](http://www.dexterindustries.com/BrickPi/projects/brickpi-bookreader-2/) 。两个版本之间的大部分部分是相同的，唯一的例外是翻页方式。乐高组件仍然使用，但这次有两个马达。马达 1 旋转一个压在要翻页的页面上的乐高轮。一旦这一页被推到足够的程度，马达 2 就会转动一只手臂来完成翻页。电机 1 然后反向旋转，以展平无意中开始翻转过程的任何页面。

[https://www.youtube.com/embed/zq5yddaIxC8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/zq5yddaIxC8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

via [ [嵌入式实验室](http://embedded-lab.com/)