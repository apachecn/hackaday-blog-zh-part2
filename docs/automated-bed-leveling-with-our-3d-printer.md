# 使用我们的 3D 打印机自动调平床

> 原文：<https://hackaday.com/2012/04/23/automated-bed-leveling-with-our-3d-printer/>

![](img/967617845f5cb31e32a633d0ae99c885.png "bed")

任何拥有 RepRap 或其他 3D 打印机的人都知道平整床有多痛苦。为了获得高质量的打印，床(打印机打印的表面)必须精确水平，如果你的表面有一点点凸起，愿工程之神帮助你。[Atntias]正在开发一个解决这个问题的方案:[一个自动调平平台](http://www.thingiverse.com/thing:18468)，如果你已经有一张金属床，它根本不需要任何零件。

这个想法非常简单:只要将你的金属床接地，在你的热端尖端施加一个小电压。[Atntias]'代码([可在 GitHub](https://github.com/Atntias/probz) 上获得)探测床的表面，并拍摄出您当前床轮廓的 3D 网格。这可用作 GCode 偏移量，因此您的打印底部总是直接位于床的顶部。

虽然将床调平到微米级的效用对于 3D 打印机来说是值得怀疑的，但如果你想在打印机上研磨 PCB，这是至关重要的。[Atntias]表示，他的想法目前正在马林固件中实施，因此看起来我们未来将进行另一次固件更新。

感谢[technodream]发来这篇文章。休息后，请观看视频，了解整平床铺的过程。

[https://www.youtube.com/embed/tKFhiu2a64I?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/tKFhiu2a64I?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)