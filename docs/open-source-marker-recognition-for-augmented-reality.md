# 用于增强现实的开源标记识别

> 原文：<https://hackaday.com/2014/08/24/open-source-marker-recognition-for-augmented-reality/>

![marker](img/fe9a73f40a842994b3aa34783e1b7239.png)

[Bharath]最近上传了基于 OpenCV 的模式识别平台的源代码，该平台可用于增强现实，甚至机器人。它是用 C++构建的，并利用 OpenCV 库在单个帧内翻译标记符号。

这个程序开始时一次只关注一个物体。选择这种方法是为了避免创建包含图像中所有斑点信息的附加数组；这可能会引起一些问题。

虽然这种实现没有通过多帧跟踪标记信息，但它确实为将模式识别集成到计算机系统中提供了良好的基础。该教程简单易懂，易于准备。整个程序和源代码可以在 Github 上找到，Github 没有许可证，任何人都可以使用。广告之后是节目的视频:

[https://www.youtube.com/embed/vmF9pStl5OM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/vmF9pStl5OM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)