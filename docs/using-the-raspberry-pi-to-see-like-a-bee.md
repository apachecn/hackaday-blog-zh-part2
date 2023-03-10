# 用树莓皮像蜜蜂一样看东西

> 原文：<https://hackaday.com/2014/05/01/using-the-raspberry-pi-to-see-like-a-bee/>

![Bee](img/4eaf8cc99586760625f2365540a65eca.png)

Raspberry Pi 板相机有一个孪生兄弟，称为 NoIR 相机，这是一种没有红外阻挡滤光片的相机，允许任何人拍摄一些用“不可见”红外光照亮的场景，调查植物的健康状况，以及其他一些很酷的东西。这款相机中的传感器不仅仅对红外光敏感——它还可以通过另一种方式对紫外光谱进行研究，并向我们展示蜜蜂和其他昆虫看到的东西。

用小型相机检查紫外光谱的唯一问题是，相对而言，相机对可见光和红外比对紫外光更敏感。为了窥视这个奇怪的世界，[奥利弗]需要一个紫外线通过过滤器，一个只允许紫外线通过的过滤器。

通过将滤镜放置在静物和相机之间，[奥利弗]能够照射深紫外光源，并在紫外光下捕捉花朵的图像。然而，右上方的图像并不是相机拍摄到的——蜜蜂看不到红色，所以绿色通道被转移到红色，蓝色通道被转移到绿色，UV 图像被放置在蓝色通道曾经的位置。

[https://www.youtube.com/embed/7gsajzhIPF8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/7gsajzhIPF8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)