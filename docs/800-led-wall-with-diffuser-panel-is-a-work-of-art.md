# 800+ LED 墙和扩散板是一件艺术品

> 原文：<https://hackaday.com/2014/07/20/800-led-wall-with-diffuser-panel-is-a-work-of-art/>

![LED Wall](img/2a8433f58ff554eb3896237b33032ca0.png)

当你把 800 多个可单独寻址的超高亮度 RGB LEDs 放在一个巨大的漫射面板中时，会发生什么？你[变得牛逼](https://www.suprmasv.com/projects/237/custom-sound-reactive-led-wall)。这就是你得到的。

[Epoch Rises]是一个小型电子音乐和互动技术二人组，他们为自己的现场表演和演出创建很酷的互动项目(如这堵墙)。他们喜欢他们的 WS2812B LEDs。

这面墙很酷的一点是，它可以接受任何视频输入，可以通过声音或音乐、iPad 来控制，甚至可以自己生成随机图像。800 个 led 由 Teensy 3.0 使用来自 [Paul Stoffregen](https://www.pjrc.com/about/) 的 [OctoWS2811](https://www.pjrc.com/teensy/td_libs_OctoWS2811.html) 库控制，该库能够仅使用一个 Teensy 微控制器以高达 30FPS 的速度驱动 1000 多个 led。它的工作原理是使用直接内存访问将数据串行发送到 Teensy 的内存中，然后直接发送到 led，开销非常小——它毕竟是一个 Teensy！

作为互动的补充，他们还为 Kinect 编写了一个应用程序，允许墙壁对人们在它面前跳舞做出反应！

[https://www.youtube.com/embed/uLGzVp6OlqQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/uLGzVp6OlqQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

下次让我们看他们做一个更大的——就像这个 [1470 像素的舞台墙！](http://hackaday.com/2011/11/20/this-giant-hand-made-led-matrix-must-be-ours/)