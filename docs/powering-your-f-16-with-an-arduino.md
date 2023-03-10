# 用 Arduino 为 F-16 提供动力

> 原文：<https://hackaday.com/2014/11/14/powering-your-f-16-with-an-arduino/>

当你身边有一架 F-16，并且想要一些闪烁的导航灯时，你会怎么做？我们确切地知道一种闪烁灯光的方法，显然我们也知道。当被要求帮助新墨西哥州的国家核科学和历史博物馆修复一架 F-16 时，[克雷格] [拿出了唯一一件应该用来闪烁空中优势战斗机导航灯的工具](http://www.spudcentral.com/potd/141114.html)。

[克雷格]的朋友正在为核博物馆修复一架 F-16，像任何有足够好奇心的人一样，他问让导航灯再次工作有多难。[克雷格]认为一个 Arduino 可以做到这一点，加上一个加载了几个 mosfets 的护盾，旧 F-16 上的导航灯将再次复活。

这块板不只是开关灯。由于[克雷格]使用的是发光二极管，这不是你反复开关普通白炽灯时看到的那种柔和的光。为了模拟这一点，[克雷格]正在用一个 PWM 引脚复制牛顿冷却定律。结果非常棒——在新墨西哥参议员和一名准将将军的揭幕仪式上，一切进展顺利。你可以在下面看到发布视频，以及来自[Craig]构建日志的一些视频。

[https://www.youtube.com/embed/kfMw8MljeAU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/kfMw8MljeAU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[https://www.youtube.com/embed/xlN3S4EcViI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/xlN3S4EcViI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[https://www.youtube.com/embed/Dpg1vnI-B7I?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/Dpg1vnI-B7I?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)