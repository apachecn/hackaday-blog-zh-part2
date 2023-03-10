# 从 LED 灯泡中窃取 WiFi

> 原文：<https://hackaday.com/2014/07/06/stealing-wifi-from-led-lightbulbs/>

[![LIFX Wireless LED PCB](img/ccbe4c064e2e24839e87f7334a65aa21.png)](http://hackaday.com/?attachment_id=126107)

早在 2012 年，LIFX 灯泡在 Kickstarter 上推出，并获得了相当大的成功。这款无线 LED 灯泡结合了 WiFi 和 6LoWPAN，可以在您的房间内创建一个灯泡网络。上下文信息安全[查看了这些设备](http://contextis.co.uk/blog/hacking-internet-connected-light-bulbs/)，发现了一些安全问题。

LIFX 系统有一个主灯泡。这是唯一连接到 WiFi 的灯泡，它通过 6LoWPAN 向其余灯泡发送所有命令。为了保持网络畅通，如果需要，任何灯泡都可以成为主灯泡。这意味着 WiFi 凭证需要在所有灯泡之间共享。

查看协议，发现了一个包含 WiFi 凭证的加密二进制 blob。使用 [AVR Raven](http://www.atmel.ca/tools/AVRRAVEN.aspx) 评估套件可以很容易地恢复这个二进制文件，但是由于它是加密的，所以不可读。

砸开一个灯泡后，他们在主板上发现了 JTAG 插头。一个 [BusBlaster](http://dangerousprototypes.com/docs/Bus_Blaster) 和 [OpenOCD](http://openocd.sourceforge.net/) 用于与芯片通信。这允许固件被转储。

通过使用 [IDA Pro](https://www.hex-rays.com/products/ida/) ，他们确定 AES 被用于加密 WiFi 凭证。再做一点工作，就可以提取出密钥和初始化向量。有了这些信息，无线发送的 WiFi 凭证就可以被解密。

好消息是 LIFX 修复了这个问题。现在，他们根据 WiFi 凭证生成一个加密密钥，防止使用全球唯一的密钥。

[via [reddit](http://www.reddit.com/r/electronics/comments/29tdrz/hacking_into_internet_connected_light_bulbs/)