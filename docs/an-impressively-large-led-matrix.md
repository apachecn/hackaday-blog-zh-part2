# 令人印象深刻的大型 LED 矩阵

> 原文：<https://hackaday.com/2013/10/26/an-impressively-large-led-matrix/>

一个居家修补者能完成的更令人印象深刻的项目之一是某种展示。最终的项目不仅产生了许多闪闪发光的东西，而且驱动数百个 led 本身就是一项成就。[杨奇煜]决定他想建立自己的 LED 显示屏，[最终有了伟大的东西](http://faitmain.org/volume-3/ledmatrix.html)(法语，[谷歌翻译](http://translate.google.com/translate?sl=fr&tl=en&js=n&prev=_t&hl=en&ie=UTF-8&u=http%3A%2F%2Ffaitmain.org%2Fvolume-3%2Fledmatrix.html&act=url))。

杨奇煜没有走极端，自己为这个巨大的 LED 显示屏制作电路板，而是在 DealExtreme 上找到了一个非常便宜的 [16×32 LED 显示屏。一旦这些套件被拼凑在一起，[Fabian]将它们安装在一个木制框架中，并开始将显示器连接在一起。](http://dx.com/p/diytj-16-x-32-dual-color-dot-matrix-module-kit-green-white-202393)

最初的计划是用 Arduino 来驱动这些，但由于像素太多，他很快就用完了 RAM。用更大的 ATMega1284p 替换 Arduino 后，[Fabian]找到了他需要的 RAM，并开始研究一些有趣的可视化技术。

当然，康威的《生命的游戏》在最终版本中有所表现，但[费边]也设法用快速傅立叶变换制作了一个光谱仪。这是一个非常漂亮的组合展示，让我们想自己买几个。