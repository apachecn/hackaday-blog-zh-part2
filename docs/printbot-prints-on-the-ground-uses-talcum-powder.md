# PrintBot 在地上打印，使用滑石粉

> 原文：<https://hackaday.com/2014/10/07/printbot-prints-on-the-ground-uses-talcum-powder/>

是的，这是一个打印机器人，但它不是 3D 打印机。尽管它被称为 [Printbot](http://www.instructables.com/id/The-PrintBot/?ALLSTEPS) ，但不要将其与其他可能以‘Print’开头、以‘bot’结尾的产品混淆。Printbot 一半是 Roomba，一半是老式喷墨打印车驱动，剩下的一半是运行 Windows CE 的小型 PC。

这个机器人的全部目的是在地板上画/写/打印东西。不，不是墨水，是爽身粉！Roomba 在一个轴上驱动，因为粉末在机器人的尾流中系统地落下。它一次工作一行，类似于逐行扫描电视在屏幕上显示图像的方式。Printbot 上的 PC 从 USB 驱动器读取 8 位灰度图像，对图像进行重新采样，并一次一行地将图像输出到外部微控制器。微控制器负责驱动 Roomba 前进，并移动料斗的位置，将粉末分配到正确的位置。看看下面的小照片。那个黑白条纹不是为了好看。它是编码器定位系统的一部分，负责将料斗的位置反馈给微控制器。

为了分发爽身粉，有一个漏斗作为漏斗。漏斗中心下方是一个钻头，可以防止粉末掉落。一个小的 DC 马达旋转钻头一段特定的时间，恰到好处的粉末从漏斗状喷口出来。然后将漏斗移至下一个需要粉状沉积物的位置，并重复该过程。

现在，如果有人能拿出一个机器人真空跟随打印机器人，并清理所有的混乱！

你觉得这个很酷但是不要挖爽身粉？看看这个[类似的设置](http://hackaday.com/2007/09/07/posterbot-hack-a-roomba-into-poster-printer/)，它使用记号笔以点阵样式书写。

[https://www.youtube.com/embed/ukxT9QqYgG0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/ukxT9QqYgG0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)