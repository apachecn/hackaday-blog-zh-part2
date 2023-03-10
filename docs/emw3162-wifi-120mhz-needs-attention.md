# 物联网乐趣的另一个无线电模块–emw 3162

> 原文：<https://hackaday.com/2015/03/24/emw3162-wifi-120mhz-needs-attention/>

廉价无线电模块的可用性使它们在我们最近看到的越来越多的项目中无处不在。通常的解决方案是使用基于 ESP8266 器件的几个模块中的任何一个。[Willem]来信与我们分享了他使用另一个无线电模块的[体验 MXChip 的 emw 3162](http://hackaday.io/project/4128-emw3162),它的[售价为 10 美元，不如 ESP8266 模块](http://www.seeedstudio.com/depot/EMW3162-WiFi-Module-p-2122.html)便宜，但它是一个功能更强、功率更大的设备。

EMW3162 ( [PDF 数据表](http://www.joinmx.com/uploadfiles/soft/EMW/DS0006E_EMW3162_V2.2.pdf))是一款低功耗嵌入式 WiFi 模块，集成无线局域网和 STM32F205 Cortex-M3 微控制器，运行“自托管”WiFi 网络库和软件应用堆栈。微控制器有 1M 闪存，128k RAM，运行频率为 120MHz。由于 MXChip 是 Broadcom 的合作伙伴，他们被允许使用 [WICED_SDK](https://www.broadcom.com/products/wiced/wifi/) 。

板载 ARM M3 意味着各种有用的接口都可用:UART、SPI、I2C、ADC、DAC、PWM、定时器、GPIO 和 JTAG flash 接口。好消息可能是功耗数据——该模块被吹捧为低功耗，数据表显示当连接到接入点但没有数据传输时为 7mA。以 20 千比特/秒传输时，电流消耗约为 24mA，在 11 千比特/秒时上升至 320mA。

[Willem]在 Github 上有他的[emw 3162 _ WICED 库](https://github.com/willemwouters/EMW3162_WICED)，但也看看 MX chips[MICO(基于微控制器的互联网连接操作系统)库](https://github.com/MXCHIP/MICO)。目前，他用 Linux 操作系统，用 gnu gcc 编译器和 JLINK JTAG 程序员。他还拥有 WICED SDK，以及一个内置 120MHz arm 芯片的 WiFi AP。听听其他用户对这个无线电模块的体验会很有意思。请在下面的评论中告诉我们吧！