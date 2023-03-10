# Teensy 3 上的裸机编程

> 原文：<https://hackaday.com/2014/04/14/bare-metal-programming-on-the-teensy-3/>

![Teensy](img/4e527e112f49bec36054d865c01f4efe.png)

Teensy 3.x 系列主板是令人惊叹的作品，体积小，适合试验板，IO 引脚数量少，处理器功能强大，所有价格都不到 20 美元。[Karl Lunt]几乎喜欢 Teensy 3 的所有功能，除了一个:Arduino IDE。是的，现存的最糟糕、最流行的 IDE。为了解决这个问题，[Karl] [建立了一个裸机开发环境](http://www.seanet.com/~karllunt/bareteensy31.html)，幸运的是，他选择与我们分享。

[Karl]正在使用 [CodeBench Lite](http://www.mentor.com/embedded-software/sourcery-tools/sourcery-codebench/overview/) 用于编译器、链接器、汇编器和所有其他 GCC 乐趣，但是 CodeSourcery 套件没有 IDE。Visual Studio 2008 Express 是[Karl]选择的环境，但几乎所有其他 IDE 都会做同样的工作。当然，make 实用程序是必需的，为飞思卡尔 K20 微控制器获取[文档也不是个坏主意。](http://www.freescale.com/webapp/sps/site/prod_summary.jsp?code=TWR-K20D50M&fpsp=1&tab=Design_Tools_Tab#)

最终的结果是[卡尔]能够为青少年 3 岁发展。x 和他选择的 IDE。他能够用新的工具链快速设置一个“闪烁 LED”程序，尽管将文件上传到 Teensy 需要 Teensy Loader 应用程序。