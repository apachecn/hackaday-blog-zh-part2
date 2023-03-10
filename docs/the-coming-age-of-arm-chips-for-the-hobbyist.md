# 爱好者的 ARM 芯片时代即将到来

> 原文：<https://hackaday.com/2012/08/13/the-coming-age-of-arm-chips-for-the-hobbyist/>

8 位 Arduino 的时代可能很快就要结束了。当然，在闪烁的 led 和打开的继电器中总会有 AVR 的一席之地，但要做任何酷的事情——播放 MP3，驱动 LCD 显示器，或运行 CNC 机器——你需要 32 位芯片的能力。[Brian Carrigan]提供了一个很棒的教程,介绍如何开始使用这些更大、更强大的微处理器，以及如何超越 8 位 PIC 或 AVR。

这些新的 32 位芯片功能更强大，但对业余爱好者来说并不友好。我们发现的大多数 ARM 芯片都被装进了间距非常小的 QFN 或 QFP 封装中，这些封装需要回流焊炉才能焊接到电路板上。事实上，我们只能找到[一个适合试验板开发的通孔 M0](http://octopart.com/lpc1114fn28%2F102%2C12-nxp+semiconductors-22360689) 芯片。这并不容易在几个小时内完成一个电路，因此需要非常强大的微控制器的建设者将更加依赖于开发板。

已经有很多基于 ARM 的 32 位开发板可用，包括来自 [Leaf Labs](http://leaflabs.com/store/) 的产品、[极其便宜的 STM 发现板](http://hackaday.com/2012/05/30/video-review-stm32f0-discovery-board/)、 [Kinetis KL25Z Freedom 板](http://www.element14.com/community/community/knode/dev_platforms_kits/element14_dev_kits/kinetis_kl2_freedom_board?view=overview)、异常强大的 [BeagleBone](http:/http://beagleboard.org/bone/) 以及永久推迟的 [Arduino(过期)](http://arduino.cc/blog/2011/09/17/arduino-launches-new-products-in-maker-faire/)。

这些板都不是特别新的发展；他们都来过这个街区一两次。然而，32 位开发比当前的 8 位 PIC 和 AVR 圣战有更多的选择。我们将通过以下问题将评论交给 Hackaday 读者:您使用的是什么超大型开发板？对于初学者来说什么是好的，他们应该注意什么？