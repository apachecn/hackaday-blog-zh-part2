# 使用锐红外传感器的 3D 扫描仪

> 原文：<https://hackaday.com/2013/12/21/3d-scanner-using-a-sharp-infrared-sensor/>

[Fernando]发来了一条关于他正在做的一个宠物项目的线索。这是在 3D 扫描仪上拍摄的有趣照片。他使用步进电机来旋转被扫描的物体，并使用 Arduino 进行控制，但真正的新奇之处在于他使用传感器的方式。[Fernando]在垂直表面上安装了一个 Sharp GP2D120X，并使用第二个步进电机在扫描过程中提升传感器。正如你在视频中看到的(插播在广告之后)，这导致扫描被放在一个上升的螺旋中。

夏普传感器既便宜又体面，但你显然不会获得惊人的准确性。尽管如此，利用几次测量的平均值，他最终得出了一个不错的结果。令人高兴的是，[Fernando]已经发布了代码，用一个更精确的传感器重新调整它应该很容易。看到一个基于激光的传感器与这种代码配对会很有趣。

[https://www.youtube.com/embed/ZQCR-mz3MDU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/ZQCR-mz3MDU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[https://www.youtube.com/embed/6BBKihqe2b4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/6BBKihqe2b4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)