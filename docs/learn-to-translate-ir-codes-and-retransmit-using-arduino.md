# 学习翻译红外代码并使用 Arduino 重新传输

> 原文：<https://hackaday.com/2013/09/27/learn-to-translate-ir-codes-and-retransmit-using-arduino/>

来自 EEVBlog.com 的[达夫·琼斯]带着“Arduino 粉丝男孩”离开花园小径，用不同的方法变得又脏又脏，以捕获、评估并重新传输 IR 遥控代码。捕捉和复制红外遥控代码并不是什么新鲜事，然而，[戴夫]开辟了自己的道路，并带领我们绕过一些“年轻玩家的陷阱”。

[Dave]需要一个倒计时定时器，可以远程开始和停止他的 Cannon 摄像机的录制，他在以前的 EEVBlog 帖子中使用一个商业学习远程控制单元简单地做到了这一点。粉丝们要求更好，因此他提供了这个优秀的教程，在示波器上从红外解码器(黄色轨迹)捕捉红外代码，并使用红外光电晶体管(蓝色轨迹)显示包含 38 KHz 载波频率的代码。任何一种捕获方法都可以很容易地用来检查传输的代码。从捕获的波形中获得的第二个经验是所用的编码调制类型。【戴夫】远程传输 NEC(日语)脉冲长度编码——可以参考[红外遥控技术](http://www.freescale.com/files/microcontrollers/doc/app_note/AN3053.pdf) (PDF)确定。了解编码方法后，手动转换这些位以供稍后在 Arduino 发射器草图中使用是很容易的。我们发现[Dave]让这个过程看起来非常简单，甚至选择自己写草图来复制和传输 IR 代码和载体，而不是走捷径去寻找现有的库。

视频中一个真正的知识宝库是当它不起作用的时候！在使用[salae 逻辑分析仪](http://hackaday.com/2009/03/06/tools-saleae-logic-logic-analyzer/)之前，我们开始跟踪【戴夫】的失误，以查看他的发射机是否偏离了频率，尽管他草图中的数学似乎是正确的。意识到数字写入程序导致速度变慢，他篡改了他的数学公式，以进行所需的频率校正。当然，他可以通过编写一些自定义端口控制来消除性能故障，但是逻辑要求在破解一次性解决方案时使用最快、最简单的解决方案。

[Dave 的]视频和源代码链接。

戴夫的 [Arduino 草图](http://gist.github.com/EEVblog/6206934)

[https://www.youtube.com/embed/BUvFGTxZBG8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/BUvFGTxZBG8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)