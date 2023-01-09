# Arduino 恒温器包括假期模式

> 原文：<https://hackaday.com/2014/12/19/arduino-thermostat-includes-vacation-mode/>

(威廉的)恒温器坏了，他想升级。他发现了一些现成的互联网恒温器，但它们都非常昂贵。他知道他可以用一小部分成本建造自己的 T1。

主单元使用 NTP 同步其时间。这将自动保持最新信息，并与夏令时保持同步。还有一个备用实时时钟芯片，以防断网。该装置可通过物理控制面板或网络界面进行控制。该系统包括一个漂亮的“度假模式”，当你离开时，它会将温度设置为凉爽的 60 华氏度。在你回家之前，它会自动将温度调节到更舒适的温度。

[威廉的]家被分成三个热区。每个区域都有自己的控制面板，包括一个 LCD 显示屏和简单的控制。这些区域可以通过各自的控制面板或中央面板进行单独配置。这些面板包括 DHT22 温度和湿度传感器、LCD 显示器、键盘和辅助电子设备。这个项目显然是经过深思熟虑的，并且包含了许多其他的小特性，使它易于使用。