# 对 NAND 闪存设备管理算法进行逆向工程

> 原文：<https://hackaday.com/2014/08/06/reverse-engineering-a-nand-flash-device-management-algorithm/>

[![unsoldered flash chip](img/cba58378ab79a088625bff3e94980913.png)](https://hackaday.com/wp-content/uploads/2014/08/sd-fux-9-xscale.jpg)

把你的手放在下巴下面，因为这里有一个长达 6 个月的[令人瞠目结舌的逆向工程工作](http://joshuawise.com/projects/ndfslave):从一个(不那么)坏的 SD 卡上取回数据。正如你从上面的图片中所猜测的，[Joshua]的第一步是拆下卡的闪存芯片，因为拆下后发现只有集成的 SD-to-NAND 闪存控制器被损坏。然后将 flash 焊接在试验板上，以便连接到 Digilent Nexys-2 FPGA 板。[Joshua]设法找到了一个类似的闪存数据表，检查了他的有线总线是否可靠，并在他的计算机上生成了两个 12GiB 的转储文件。

为了从转储中提取有意义的数据，他首先必须了解 SD 到 NAND 控制器是如何工作的。在他的精彩文章中，他为我们提供了闪存技术的背景，因此我们的读者可以更好地了解我们今天的芯片面临的挑战。随着闪存在保持相同大小的情况下集成更多的存储空间，它们变得不太可靠，并存在一些应该注意的问题。因此，控制器必须执行[数据白化](http://en.wikipedia.org/wiki/Whitening_transformation)(因此相邻的数据块没有相似的内容)，在闪存周围均匀地分布数据写入(因此物理块具有相同的预期寿命)，并最终支持[纠错码](http://en.wikipedia.org/wiki/Error-correcting_code)(因此损坏的位仍然可以恢复)。我们将让我们的用户想象，当你对控制器一无所知时，这种技术的实现是多么复杂。[Joshua]因此，他必须做大量的研究，对他提取的数据进行大量的统计分析，如果没有其他办法，就使用暴力…