# 基于树莓派的 SSTV 灯塔

> 原文：<https://hackaday.com/2013/10/06/sstv-beacon-based-on-a-raspberry-pi/>

[![](img/8d562eae52859559f6a27fe557f194fb.png)](http://hackaday.com/wp-content/uploads/2013/10/img_20130710_203436.jpg)

布达佩斯黑客空间与当地一家业余无线电俱乐部合作，创建了一个 [SSTV 信标](http://hsbp.org/rpi-sstv)放在一个闭路电视盒内，它拍摄周围环境的图像，并使用[慢扫描电视](https://en.wikipedia.org/wiki/Slow-scan_television)通过业余波段传输。

正如标题所述，build 使用 Raspberry Pi 处理从其相机拍摄的图像，然后使用 Ricofunk UHF 收发器以 433.425MHz 的主频通过空中传输它。在软件方面， [PySSTV](https://pypi.python.org/pypi/PySSTV) 用于将图像转换为频率/时间元组，UNIXSSTV 然后创建实际的音频文件，最后 [sox](http://sox.sourceforge.net/) 播放它。为了避免搞砸 Raspberry SD 卡，filsystem 的每个部分要么以只读模式挂载(比如/home 和/usr)，要么使用 ramdisk(比如/tmp 和 logs)。

计划、原理图和源代码都有了，所以他们希望其他黑客空间也能加入这个行列！