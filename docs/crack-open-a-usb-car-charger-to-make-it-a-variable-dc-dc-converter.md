# 打开一个 USB 汽车充电器，使它成为一个可变的 DC-DC 转换器

> 原文：<https://hackaday.com/2015/08/13/crack-open-a-usb-car-charger-to-make-it-a-variable-dc-dc-converter/>

[Boolean90] [把一个便宜的 USB 车载充电器](https://www.youtube.com/watch?v=2IOs3g-52Zo)黑成了可变电源。他的概念证明是用这个作为变速电机控制器。最好的部分是没有被滥用，里面的调节器仍然在制造商的规格内运行。

虽然我们以前也见过类似的黑客攻击，但是 Boolean90 的视频非常酷，让我们可以深入了解这些廉价设备中使用的组件。该设备使用普通的 jelybean [MC34063A](http://www.onsemi.com/pub_link/Collateral/MC34063A-D.PDF) 在这里，它用于将汽车电池从 12 伏降至 5 伏，但也可以用于升压和逆变配置。

像所有开关降压转换器一样，MC34063A 使用 PWM(脉宽调制)信号来驱动电感和电容，从而有效地形成 LC 滤波器。通过控制脉冲宽度，可以调节输出电压。[Afrotechmods]有一个很棒的关于基本原理的[教程。调节由反馈电阻控制。[Boolean90]只是增加了一个可变电阻，以便控制输出电压。](https://www.youtube.com/watch?v=CEhBN5_fO5o)

整洁的 hack [Boolean90]！

[https://www.youtube.com/embed/2IOs3g-52Zo?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/2IOs3g-52Zo?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)