# 令人满意的“构建”项目的方式

> 原文：<https://hackaday.com/2014/01/29/satisfying-way-to-build-projects/>

![build button 01_27](img/01d55a015c8b6e8882c4265871605fb7.png)

当你为你的下一个重大创造写代码时，你可能一天要构建/调试项目 100 次。当然，键盘热键可以完成工作，但是它真的那么令人满意吗？[Victor]提交了这个快速项目，将一个[紧急停止按钮转换成一个“构建”按钮](http://roteno.com/?q=build_button)。

从表面上看，这个项目使用的是一款搭载 ATMEGA32U4 的 [Teensy 2.0](http://www.pjrc.com/store/teensy.html) 。由于这部分有一个 USB 控制器，让它[模仿一个键盘](http://www.pjrc.com/teensy/usb_keyboard.html)是小菜一碟。电路也很简单；按钮触点从地连接到数字输入。在检测到“按压”时，Teensy 将发送键盘组合来构建您的项目:Ctrl-B，F7 等。如果您喜欢在 Arduino IDE 中工作，这也可以上传草图(Ctrl-U)。

不过，为“构建”你的项目增添一点乐趣是有代价的。除了失去一个小东西，你还得放弃一个珍贵的 USB 接口。[Victor]确实提到了蓝牙，但这可能会超出您对此类项目的预算。Teensy 的一个可能的替代方案是在低成本的独立 Arduino 上实现[虚拟 USB。](http://hackaday.com/2014/01/18/usb-datalogging-with-arduino-using-v-usb/)

[https://www.youtube.com/embed/sBbFbR4EEoc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/sBbFbR4EEoc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)