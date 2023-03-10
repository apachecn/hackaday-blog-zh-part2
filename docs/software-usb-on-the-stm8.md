# STM8 上的软件 USB

> 原文：<https://hackaday.com/2014/03/02/software-usb-on-the-stm8/>

![STM8](img/9b65b020377fa703cd12f7a57f94bbb2.png)

由于 V-USB，基于软件的 USB 现在非常流行，在非常小和低功率的微控制器上有很多用途。[ZiB]想知道是否有可能在 STM8 微控制器(谷歌[翻译](http://translate.google.com/translate?sl=ru&tl=en&js=n&prev=_t&hl=en&ie=UTF-8&u=http%3A%2F%2Fziblog.ru%2F2014%2F02%2F20%2Fprogrammnyiy-usb-na-mikrokontrollerah-stm8.html&act=url))上用软件实现[一个 USB 控制器，并且成功了。](http://ziblog.ru/2014/02/20/programmnyiy-usb-na-mikrokontrollerah-stm8.html)

STM8 与我们常见的 AVR 和 PICs 等 8 位微处理器有所不同。[ZiB]选择了 STM8S103F3，尽管当连接 12MHz 晶体时，STM8 系列中的任何芯片都可以用于该项目。

在大量 nop 的帮助下，构建从生成 USB 信号开始。这段代码并不占用太多空间——只有 300 字节，[而接收代码](http://ziblog.ru/2014/02/22/programmnyiy-usb-na-stm8-chast-2.html)(谷歌[翻译](http://translate.google.com/translate?sl=ru&tl=en&js=n&prev=_t&hl=en&ie=UTF-8&u=http%3A%2F%2Fziblog.ru%2F2014%2F02%2F22%2Fprogrammnyiy-usb-na-stm8-chast-2.html&act=url))的大小也差不多。

代码还没有完全出来，但是[ZiB]已经证明在 STM8 上实现基于软件的 USB 是可能的。所有代码都可以下载(俄语评论)和一个视频演示项目如下。如果有人想把这个项目翻译成英语，我们会在这里发布你的作品的链接。

[https://www.youtube.com/embed/vVaZwpc_c-g?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/vVaZwpc_c-g?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)