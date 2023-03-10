# 潮人转盘增加蓝牙 4.0

> 原文：<https://hackaday.com/2015/08/27/hipster-rotary-dial-adds-bluetooth-4-0/>

我们已经看到一些项目将旋转拨号盘转换为现代技术使用，但这个项目增加了一个新的组合:[它使用蓝牙 4.0](http://silent.org.pl/home/2015/08/09/hipster-phone-bluetooth-rotary-dial/) 。[Silent]为该项目使用了一个 [Nordic Semiconductor NRF51 DK 开发板](https://www.nordicsemi.com/eng/Products/nRF51-DK)，它是根据 Nordic SDK 源代码构建的，用于创建 HID(人机界面设备)。在他声称的大约一个小时的黑客攻击后，他能够让这个 Arduino 兼容的 SoC 开发板检测来自旋转拨号盘的脉冲，然后通过按键将适当的数字传递给连接的设备。这意味着他的设计可以与任何支持蓝牙 4.0 的设备兼容。它由一个大干电池供电，因为，引用[沉默]，“小硬币电池不够时髦”。

这是一个简单的项目，我们以前也见过旋转式手机，但这仍然是一个成熟的扩展项目。你可以在这个黑客的中心使用一个更小、更便宜的 Nordic 芯片，因为大多数开发板功能都没有使用。或者你可以做更多的黑客工作，增加对蓝牙 HSP 耳机模式的支持，然后将其连接到一部[老式手机](http://www.ebay.com/itm/Vintage-1960-Bell-System-western-Electric-500-Rotary-Telephone-Black-Phone-Desk-/221861397037)上，成为有史以来最时髦的蓝牙耳机。我们迫不及待地想看到一个潮人坐在咖啡店[里敲着打字机](http://hackaday.com/2015/08/27/turning-a-typewriter-into-a-mechanical-keyboard/)回答这个问题。开始吧，伙计们！

[https://www.youtube.com/embed/qh9mVBTcc8k?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/qh9mVBTcc8k?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)