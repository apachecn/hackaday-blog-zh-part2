# 简单有效的方法来测量 PWM…没有范围！

> 原文：<https://hackaday.com/2014/11/26/easy-and-effective-way-to-measure-pwm-without-a-scope/>

有时候，当一个项目开始时，你需要拼凑一个工具来完成它。无论是非常复杂的事情，如构建 3D 打印机来制造定制零件，还是相对简单的事情，如将灯泡和电池连接在一起以创建一个简单的连续性检查器，我们都必须在运行中想出一些东西。尽管可以使用示波器，[Brian]又名[schoolie]还是想出了自己的方法，在没有示波器的情况下[测量 PWM 周期和占空比，以防出现 PWM 紧急情况！](http://sonsofinvention.wordpress.com/2013/02/19/analyzing-pwm-period-and-duty-cycle-without-an-oscilloscope/)

他提出的系统如此简单，简直是天才之作。问题中的 PWM 信号通过一个压电扬声器与一个电阻并联。扬声器的输出然后被发送到 Android 设备的 FFT ( [快速傅立叶变换](http://en.wikipedia.org/wiki/Fast_Fourier_transform))应用程序，该应用程序生成波形图。[schoolie]然后在 MS Paint 中打开图片，使用光标的坐标和一点算术来计算周期和占空比。

由于没有使用示波器，这种方法相当准确，并且只使用了两个分立的电路元件(电阻和扬声器)。如果你在使用 PWM 时遇到困难，这肯定会有所帮助，而且比找示波器要便宜得多！