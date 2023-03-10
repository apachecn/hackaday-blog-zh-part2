# 用 Arduino 生成刺绣

> 原文：<https://hackaday.com/2014/02/15/generating-embroidery-with-an-arduino/>

[![Arduino Embroidery Generation](img/6dd4f495dd4dccca5ff4090cbce8962b.png)](http://hackaday.com/2014/02/15/generating-embroidery-with-an-arduino/embroidery/)

想要一种巧妙的方式将刺绣工艺与电子技术结合起来吗？开发开源刺绣机的人们通过使用 TFT 屏幕和 Arduino 生成 KDE 标志[的刺绣来演示他们的软件。](http://embroidermodder.github.io/news0.html#demo)

[绣花工具](http://embroidermodder.github.io/)是一款用于生成刺绣图案的开源工具。它会生成一个图案，并预览刺绣完成后的效果。这是一个具有 GUI 的跨平台桌面应用程序，但是 lib scene 库在后台完成了繁重的工作。这个库被移植到 Arduino 来完成破解。

虽然用 Arduino 生成刺绣图片看起来很整洁，但它并不太有用。然而，由于该库已经被移植，所以可以用它来控制其他硬件。有了合适的硬件，这可能是一个开源刺绣机的开始。

休息之后，看看正在生成的模式的视频。

[https://www.youtube.com/embed/KqiKfn4lxBk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/KqiKfn4lxBk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)