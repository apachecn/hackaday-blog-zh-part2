# 使用这款新的 PIC 开发板，让您乐在其中

> 原文：<https://hackaday.com/2015/07/18/get-your-kicks-with-this-new-pic-development-board/>

虽然微控制器的开发板没有什么突破性的，但它们可能很贵，而且当它们试图将您可能使用的所有东西都放在一起时，通常会对您的工作造成过度的伤害…包括厨房水槽。当[Brian]注意到他的项目开始越来越多地使用 Microchip PIC24 时，是时候准备一个开发板了。

[![top-view](img/b732fd5e4ab52011ed99e5a2256a994f.png)](https://hackaday.com/wp-content/uploads/2015/07/top-view.jpg) 结果是一个小板，带有 USB、UART(通过 FTDI)的分线点，当然还有大量 GPIO 引脚，以及一个与子板匹配的插座，可以替换 PIC24FJ128GC006 或 DSPIC33EP256MU806，还有更多潜力。板上还封装了一个功率调节系统和双晶体，允许全速运行或功率啜吸模式。

原理图和 PCB 布局图(Diptrace 格式)以及与[github.com](https://github.com/briandorey/PIC24-Dev-Board)上的 MPLAB 一起使用的板模板文件可用。一旦你把一切都准备好了，你将需要一个 PIC 编程器，[Brian]正在使用一个可靠的微芯片 MPLAB ICD 3 编程器，但是自然地，其他人也是可用的。

微芯片最近宣布了他们自己的 PIC16F 系列的新开发板。好奇号板内置编程和调试支持(无需芯片套件)。设计该板的工程师[约翰·木桐]将于 7 月 30 日前往[参加我们关于设计过程的现场聊天](https://hackaday.io/event/6815-pcb-design-engineer-chat)。我们还将分发一些从生产线上下来的第一批主板…下周会有更多的消息。