# 给旧液晶显示器注入活力

> 原文：<https://hackaday.com/2013/01/18/breathing-life-into-an-old-lcd/>

![panel](img/99087def1d8e9933b36656d4a8894617.png)

从一个垃圾抽屉的深处，[亚历克斯]的朋友拿出一个旧的单色液晶显示器。这是一个古老的低分辨率显示器，不幸的是没有自己的控制器芯片。不过，不用担心，因为在 FPGA [Alex] [的帮助下，我找到了如何驱动这个显示器](http://forum.gadgetfactory.net/index.php?/topic/1502-low-res-monochrome-hitachi-lcd-driver/)。

该显示器的背面有八个日立 LCD 驱动器、六个列移位器和两个行移位器，使 LCD 能够显示 256×128 像素的图像。但是，如果没有 LCD 控制器，[亚历克斯]就不能只向 LCD 发送静态图像。相反，他必须像 VGA 显示器一样不断刷新显示器。

在标题为*日立 LCD 控制器/驱动器 LSI 数据手册的 1500 页 PDF 的帮助下，* [Alex]能够在 Papilio One FPGA 板的帮助下将像素转储到显示器上的 ICs 中。很多工作只是为了展示美丽的(莉娜)，但她不会有任何其他方式。