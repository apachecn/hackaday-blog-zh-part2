# CuteUino:只使用 Arduino 中每个项目都需要的部分

> 原文：<https://hackaday.com/2013/03/20/cuteuino-only-use-the-parts-of-the-arduino-that-you-need-for-each-project/>

![CuteUino](img/3ae7073cff58be456dec3646a4a8b1b6.png)

[Fran]正在开发她自己版本的 Arduino。出于显而易见的原因，她称之为可爱的诺。这东西的大小相当惊人，正好在 SD 卡的轮廓之内。但这并不意味着你不会得到你所习惯的设备的力量。她把它分成了几个模块，这样你就可以只选择项目需要的组件。

主板显示在右侧，包括顶部和底部。它将 ATmega328p(很难相信我们可以在中断后在剪辑中辨认出芯片封装上的标签)放在 TQFP-32 封装中，焊接在她所谓的大脑模块的下面。您还可以看到从安装在电路板顶部的母引脚接头伸出的超长引脚。在这些引脚接头内，您会发现时钟晶体、状态 led 和一个电容器。另一个模块是 FTDI 板，用于将 AVR 芯片连接到 USB 端口。

你肯定想看看[她为这个项目](http://www.frantone.com/designwritings/design_writings.html#cuteuino)发布的原型帖子。她使用了一种非常有趣的技术，将两块单面电路板结合在一起，制成一个 3 层 PCB。未覆铜的一侧手工贴上铜箔，作为过孔的接地层。整洁！

[https://www.youtube.com/embed/OqW0eQiR1lE?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/OqW0eQiR1lE?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[谢谢丹尼尔]