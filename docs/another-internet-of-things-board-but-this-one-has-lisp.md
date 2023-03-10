# 另一个物联网板(但这个有 Lisp)

> 原文：<https://hackaday.com/2014/10/23/another-internet-of-things-board-but-this-one-has-lisp/>

在我们经常去的圈子里，使用路由器作为开发板是一个长期的宝贵传统，最终中国的设计公司注意到了这一点。最近几个月出现了一些“物联网”板，它们采用低端路由器中的 SoC，将与 USB、一些 GPIOs 和相当多的内存封装在一块板上，并将其称为开发板。ZERO Plus 也不例外，但是它包含了一个非常有趣的特性:它使用 Lisp 作为自己的母语。

Zero 组合很像你所期待的被移植到物联网主板上的路由器 SoC:它使用 [Ralink RT5350](https://wikidevi.com/wiki/Ralink_RT5350) SoC，提供 802.11b/g/n，有 32MB 内存，8 或 16 M 闪存，I2C，I2S，SPI，USB，两个 UARTs 和 14 个 GPIOs。通过分线板支持网络摄像头、温度和湿度传感器、显示器和 Arduino，该分线板似乎包含标准的 DIP 大小的 ATMega328，

不过，所有这些都可以在其他几十种电路板上找到。真正让它与众不同的是 Lisp 开发环境。编程调零就像你所期待的一样优雅，一个“根据时间切换 LED”程序看起来像这样:

```
(define LED_On (lambda ()(dev.gpio 11 "out" 1)))
 (define LED_Off (lambda ()(dev.gpio 11 "out" 0)))
 (define CurrentTime? (lambda ()
    (int (time.strftime "%H" (time.localtime (time.time))))))
       (define Night?
          (lambda ()
            (and
            (> ( CurrentTime? ) 16) (< ( CurrentTime? ) 23)
          )
       )
    )
 (if (Night?) (LED_On) (LED_Off)

```

围绕更深奥的编程语言构建的开发板并不是什么新鲜事； [Espruino](http://www.espruino.com/) 为 ARM 微控制器带来了 Javascript，而[MicroPython 项目](http://hackaday.com/2013/11/27/interview-with-damien-george-creator-of-the-micro-python-project/)是一项惊人的事业[和成功的 Kickstarter](https://www.kickstarter.com/projects/214379695/micro-python-python-for-microcontrollers) 为嵌入式世界带来了 21 世纪的基础。不过，Lisp 我想没人会想到这一点。不过，这是让你的产品与众不同的好方法。