# Arduino 电源逆变器

> 原文：<https://hackaday.com/2013/06/21/an-arduino-power-inverter/>

如果你有几块太阳能电池板，或者你想从几块 12 伏的电池中获得 120/230 伏的交流电，你需要一个电源逆变器。当然，你可以去任何一家大商店买一个，或者你可以像[迈克尔] [一样，自己做一个](http://techmind.dk/arduino-singleboard/inverter-12v-dc-til-230-volt-ac-med-arduino/)(丹麦语，[翻译](http://translate.google.com/translate?js=n&sl=auto&tl=en&u=http://techmind.dk/arduino-singleboard/inverter-12v-dc-til-230-volt-ac-med-arduino/))。

[Michael]发现自己拥有一些卤素灯变压器，并决定利用它们制造一个 DC 到交流电源逆变器。逆变器相当简单——只需要变压器、几个 MOSFETS 和一个用于软件控制的 ATMega0168，该软件控制包括一个防止启动时功率浪涌的“软启动”功能。

该电路非常简单，可以在家里进行蚀刻，尽管阻焊膜和一个良好的绝缘外壳可能是这种应用的理想选择。