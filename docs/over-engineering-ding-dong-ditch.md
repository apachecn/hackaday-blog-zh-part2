# 过度工程化的丁咚沟

> 原文：<https://hackaday.com/2014/12/11/over-engineering-ding-dong-ditch/>

一天，[萨米]最好的朋友[马特]提到他有一个无线门铃。令人惊讶。更令人惊讶的是，任何人都可以花 20 美元买到软件无线电，花 4 美元买到来自易贝的小型无线电模块，花 40 美元买到 GSM 分线板。将这些部件连接在一起，你就有了一个可以在地球上任何地方按[Matt]门铃的装置。是的，这是终极的过度设计的丁咚沟，这是一个很好的例子，表明如果你知道拿起烙铁的哪一端，你可以开多远的玩笑。

仅仅知道[马特]有无线门铃是不够的；[Samy]需要知道频率、调制方案以及门铃发出的信号。有些信息可以通过查找 FCC ID 找到，但是[Samy]找到了更好的方法。当[Matt]不在家时，[Samy]只是在用 RTL-SDR 电视调谐器观看瀑布图时按了几次门铃。小型廉价遥控器通常会使用几个常见频率——315 MHz、433 MHz 和 900 MHz。最终，[Samy]发现门铃发射的频率是–433.8 MHz。

在捕捉到门铃的无线电信号后，[Samy]无畏地看着音频波形。它看起来像这个门铃使用开关键控，或者只是打开二进制“1”的无线电，关闭二进制“0”。在 Audacity 中，门铃传输的一切都变得非常清晰，通过 SparkFun 提供的价值 4 434 MHz 的发射器，[Samy]可以复制门铃的输出。

对于其余的构建，[Samy]使用的是来自 Adafruit 的迷你 GSM 蜂窝分线板。该模块监听任何包含“门铃”一词的短信，并向 Arduino 发送信号。Arduino 然后用发射器发出门铃代码。它是邪恶的，而且被过度设计了。

现在，丁咚沟项目就建在[马特]家对面的某个地方。据报道，该设备运行良好，希望没有被滥用太多。下面视频。

[https://www.youtube.com/embed/BnwBdeQB7vQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/BnwBdeQB7vQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)