# Atmel 宣布推出 SmartConnect WiFi 模块

> 原文：<https://hackaday.com/2014/03/01/atmel-announces-smartconnect-wifi-modules/>

[![Atmel SmartConnect](img/b791d39df0ae36e4ff2828516b7ef982.png)](http://hackaday.com/2014/03/01/atmel-announces-smartconnect-wifi-modules/atmel-smartconnect/)

本周，我们与 Atmel 讨论了他们针对物联网应用的新 [WiFi 解决方案。早在 2012 年，Atmel 收购了 Ozmo，这是一家使用](http://atmelcorporation.wordpress.com/2014/02/24/atmels-smartconnect-targets-the-iot/) [WiFi Direct](http://en.wikipedia.org/wiki/Wi-Fi_Direct) 专注于点对点 WiFi 解决方案的公司。这些设备被称为 [SmartDirect](http://www.atmel.ca/products/wireless/wifi/wi-fi_direct.aspx "Atmel SmartDirect") ，已经面市一段时间了。

Atmel 刚刚宣布了一个新的产品线:SmartConnect。这超越了 WiFi Direct 的点对点特性，支持连接到标准接入点。SmartConnect 系列专为嵌入需要连接到网络的低成本设备而设计。

SmartConnect 系列的第一批设备将是基于两种芯片的模块:Atmel SAMD21 Cortex-M0+微控制器和 Ozmo 3000 WiFi 片上系统。还有一个机载天线和射频屏蔽罐。这是一个 WiFi 模块的下降，这是由 FCC 认证的。您可以通过 SPI 将您的微控制器连接到该器件，获得支持 WiFi 的完全认证设计。

使用该模块有两种方式。第一种是作为附加模块，类似于现有的模块。主机微控制器通过 SPI 与模块通信，并利用其命令集。第二种方法是将模块用作独立器件，应用代码在内部 SAMD21 微控制器上运行。Atmel 表示，独立选项将只在个案的基础上可用，但我们希望这对每个人开放。如果 Arduino 工具链可以针对这种微控制器，它可能是廉价 WiFi 设备的一个伟大的开发平台。

[![SmartConnect Architectures](img/173e827dc82f71297e64fa009855a720.png)](http://hackaday.com/2014/03/01/atmel-announces-smartconnect-wifi-modules/atmel-smartconnect-modes/)

The Add-On and Standalone Architectures

乍一看，这个模块与其他 WiFi 模块非常相似，包括我们在过去讨论过的[cc 3000。然而，也有一些显著的差异。一个主要特性是内置了对 TLS 和 HTTPS 的支持，这使得构建具有安全连接的设备变得更加容易。这在部署通过互联网连接的设备时至关重要。](http://hackaday.com/2013/01/12/finally-ti-is-producing-simple-cheap-wifi-modules/ "Finally, TI is producing simple, cheap WiFi modules")

Atmel 也声称在电源管理方面有所改进。该模块可以在 1.8 V 至 3.3 V 的电池电压下直接运行，无需外部调节，深度睡眠电流为 5 nA。显然，操作能力会更高，但这将大大有助于偶尔连接到互联网的设备。他们还暗示了价格，称该模块将接近类似 WiFi 解决方案当前价格的一半。SmartConnect 计划于 6 月 15 日发布，因此我们希望在今年夏天了解更多信息。

我们总是很高兴看到更好的连接解决方案。如果 Atmel 推出一款允许更便宜、更安全的 WiFi 模块的设备，它将成为构建物联网设备的重要组成部分。预计到 2020 年，物联网设备将达到 500 亿台，我们希望看到试图抢占市场份额的硅公司在这一领域取得长足进步。