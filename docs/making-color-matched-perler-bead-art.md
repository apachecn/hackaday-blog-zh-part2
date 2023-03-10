# 制作颜色匹配的佩勒珠艺术

> 原文：<https://hackaday.com/2012/06/01/making-color-matched-perler-bead-art/>

![](img/c1c2c0e8c95a533c492234d5320bfd4c.png "Perler")

你可能记得一年级或二年级时的佩勒珠；这些小塑料珠被放入一个钉板中，然后熨烫成一个结实的彩色塑料片。最近，由于一些人用塑料制作了 8 位和 16 位视频游戏精灵，Perler beads 出现了某种程度的复兴，但仍然需要付出巨大的努力来制作一个过得去的 Sonic 或 Mega Man。

[Jon Wilson]送来了一个令人敬畏的[珠子图案生成器](https://sites.google.com/site/degenatrons/other-stuff/bead-pattern-generator)，它可以拍摄视频游戏精灵的彩色图像——以及几乎任何其他图片——并将它们转换成 Perler 珠子图案。一个牛逼的功能就是配色；[Jon]找到了 Perler 珠子每种颜色的 RGB 值，他的程序从原始图像中选择最接近的匹配。

[Jon]开始为他的珠子图案生成器开发 GUI 应用程序，但是因为他的孩子不再喜欢珠子了，所以 GUI 还没有完成。有一个命令行 Python 脚本，它可以获取图像并输出珠子图案的 PDF，这对于除了最复杂的设计之外的所有设计来说应该绰绰有余。