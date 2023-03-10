# 问 Hackaday:纸质 USB 名片能存在吗？

> 原文：<https://hackaday.com/2014/08/25/ask-hackaday-can-paper-usb-business-cards-exist/>

[![swivel business card](img/75cd40b579d7ebf06d223168fc39679b.png)](https://hackaday.com/wp-content/uploads/2014/08/swivel.jpg)

swivelCard Kickstarter 活动最近得到了大量的媒体报道，并做出了一些令人印象深刻的声明，因为他们的目标是以 3 美元的单价开发 USB 和 NFC 名片。虽然我们在 Hackaday [上展示的大多数 USB 功能的名片是由标准 FR4](http://hackaday.com/2014/06/17/designing-the-second-version-of-my-business-card/) 制成的，但这种特殊的名片是由纸张制成的，因为项目描述称该团队获得了专利

> 将普通纸张转换成 USB 驱动器的系统。

正如你所猜测的，这激起了我们的兴趣，因为到目前为止，我们看到的所有基于纸张的技术大多由印刷电路板或 T2 纸电池组成。因此，在普通纸张上打印 USB 驱动器(如视频所说)将涉及打印功能性 USB 和 NFC 控制器。

足够幸运的是，在谷歌上快速搜索其中一张图片中显示的专利([专利 1](https://www.google.com/patents/US8047443) 、[专利 2](https://www.google.com/patents/USD632298) )让我们了解到，在印刷的 USB 焊盘下嵌入了一个存储电路，这可能意味着该团队设计了一个专用集成电路( [ASIC](http://en.wikipedia.org/wiki/Application-specific_integrated_circuit) ，或者他们只是找到了一个可以用于自己目的的集成电路。从视频中，我们了解到“每张卡都有一个唯一的 ID，可以单独编程”(卡，而不是 UID)，并且它可以设置为打开任何网页 URL。后者甚至可以在卡片分发后被修改，暗示最终收件人将前往一个“www.swivelcard.com/XXXX”类型的地址。因此我们被弄糊涂了

> 想象一下，给你的名片上有图片、视频、演示文稿和网站，让收件人可以与之互动！

项目描述包含的段落。

这就引出了我们的一个关键问题:考虑到用户可能使用 Linux、Windows、Mac 或任何其他操作系统，什么样的 USB 驱动器可以让他访问特定的网站？它们都有类似的 USB 枚举过程和不同的击键来启动浏览器…我们大胆的猜测是，它可能被检测为其中有单个 html 文件的存储。不幸的是，我们的 USB 检测过程不包括在视频中。

我们的最后一个问题:有没有可能在一张薄薄的纸上同时嵌入 USB 和 NFC 控制器，而不用担心 IC 损坏(见上图)？支持 NFC 的护照显然已经存在很长时间了，但我们无法为 USB 驱动器找到相同的功能。

不管有没有可能，我们都希望手中有一个！

编辑:我们的一位好心读者指出，这一活动实际上是失败的 indiegogo one 的重新推出，它提供了有关该技术的更多细节，并证实了我们的假设。