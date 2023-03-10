# 安蒂尼的 AES-CMAC 85

> 原文：<https://hackaday.com/2015/02/20/aes-cmac-on-an-attiny85/>

[Blancmange]用 ATtiny85 做了一个[定制的门铃](http://realhamster.com/stash/GateBuzzer/)。与大多数商业产品不同，这款产品实际上试图确保安全，使用 AES-CMAC 进行消息签名。

硬件非常简单，上图显示了原型机的布局。它使用 ATtiny85 进行控制，带有一个 [LM380N](http://www.ti.com/product/lm380) 音频放大器和一个低成本 315 MHz 接收器。

更令人印象深刻的是固件。使用 AVR 汇编，[Blancmange]设法将所有内容都放入 ATtiny85 的 8kb 闪存中。这包括 AES-CMAC 的实现，一种基于 AES 密码的[消息认证码](http://en.wikipedia.org/wiki/Message_authentication_code)。发送设备使用双方共享的密钥对请求进行签名，接收方验证消息是否来自可信的发送方。

幸运的是，汇编代码被很好地注释了。如果你曾经想了解一些复杂的 ASM 汇编，这是一个很好的项目。源代码已经发布到公共领域，所以我们其他人可以在这个便宜的微控制器上轻松实现加密。