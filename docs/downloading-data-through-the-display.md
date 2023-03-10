# 通过显示器下载数据

> 原文：<https://hackaday.com/2014/12/14/downloading-data-through-the-display/>

HIPAA——美国电子医疗保健文档标准——在电子记录的安全性上花费了大量的措辞和官僚主义，明确区分了医疗保健工作者对记录的*使用*和医疗保健工作者对记录的*披露*。同样，2002 年的《联邦信息安全管理法》也做了同样的区分；不应被*披露*或传输的记录应该在与网络断开的系统上使用。

这种区分*使用*和*披露*或者传播当然是一场闹剧；如果你能在屏幕上显示某样东西，它就能被传播。[Ian Latter]刚刚在 T4 的 Kiwicon 上做了一个演讲，这个演讲提供了实现这个目标的工具。他称之为 thruglasxfer(TGXf ),它确实如罐头上所说的那样:任何可以在屏幕上显示的东西都可以被传输。你需要的只是合适的工具。

[伊恩]是怎么做到的？有二维码，奇怪的是。[Ian]设计了一个协议和应用程序，允许人们通过屏幕下载文件。通过使用 TGXf，任何人都可以加载本地存储在计算机上的文件，通过 QR 码显示二进制数据，并用智能手机或微型摄像机记录这些数据。然后对该视频进行分析，恢复数据，并传输文件，从而挫败了系统管理员心中的所有安全措施。

![ThruKeyboardXfer (TKXf) keyboard stuffer](img/cb16458ae22530d7e5894b05b038c830.png)

ThruKeyboardXfer (TKXf) keyboard stuffer

将二进制数据显示为 QR 码会带来另一个问题。如何在一个锁定的系统上安装一个将原始数据转换成二维码的应用程序？这是[Ian]的另一个锦囊妙计，叫做 ThruKeyboardXfer (TKXf)。这需要一个硬件设备来模拟一个 USB HID 键盘，简单地通过模拟一个键盘将数据推送到计算机。

TKXf 对二进制数据进行编码，这些数据从一台电脑(或智能手机)的串行端口发出，并通过另一台电脑的键盘输入。可以通过 USB HID 键盘接口将单个文件(即一个将数据编码为 QR 码的应用程序)或连续的数据流发送到计算机中。

为了演示他的系统，[Ian] [上传了一段视频](https://www.youtube.com/watch?v=2_8GlFdlb0Y)，视频中智能手机通过笔记本电脑屏幕从 YouTube 下载 PDF 文件。这种文件传输的唯一要求是将电话直接指向屏幕；从电脑向智能手机发送数据不需要 WiFi 或蜂窝网络。

如果这听起来像是从即将出版的[科利·多克托罗]雅小说的页面上撕下来的，你可能离得不远了:几乎所有关于安全和隐私控制的官方建议，[包括 NIST](http://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-53r4.pdf)出版的出版物，都区分了文件的*使用*和文件的*分发*或*披露*。在屏幕上显示信息和通过网络发送信息有明显的区别。通过在显示器上传输二进制数据，[伊恩]已经踢开了那扇门，将每一台显示器和每一名员工都变成了安全隐患。

* * *

[https://www.youtube.com/embed/2_8GlFdlb0Y?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/2_8GlFdlb0Y?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

谢谢[罗曼]送来这个。