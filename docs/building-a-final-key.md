# 构建最终密钥

> 原文：<https://hackaday.com/2014/04/21/building-a-final-key/>

![Final Key](img/025b8f81d6bd90c7becf9f709063b636.png)

记住密码是一件痛苦的事情，有很多设备可以让它变得更容易。如果你想自己动手制作，这个指南[将带你完成这个过程。](http://cyberstalker.dk/finalkey/building/)

我们在之前讲过[最终键。这是一个一键式密码管理器，可以加密和存储您的密码。它充当配置的虚拟串行端口。当你按下按钮时，它就变成了一个键盘，输入正确的密码。](http://hackaday.com/2014/01/21/final-key-a-mooltipass-like-device/)

出于多种原因，创作者无意将它变成一个商业项目。相反，基于 [Arduino Pro Micro](http://arduino.cc/en/Main/arduinoBoardMicro) 提供了简单的构建指令。通过弯曲 DIP 引脚，可以将 [24LC512](https://www.microchip.com/wwwproducts/Devices.aspx?dDocName=en010828) EEPROM 直接焊接到 Arduino。几个电阻、一个按钮和一个 LED 灯就完成了这个项目。最后一步是用热胶填充，防止篡改。

[最终关键固件](https://github.com/DusteDdk/FinalKey)在 Github 上有，表壳可以从 [Shapeways](http://www.shapeways.com/model/1684349/case-for-arduino-pro-micro.html) 订购。如果你对硬件密码管理感兴趣，你也可以看看正在 Hackaday 上开发的 [Mooltipass](http://hackaday.io/project/86-Mooltipass) 。

【感谢 Lars 的提示！]