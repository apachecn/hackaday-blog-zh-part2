# 用磁头读取信用卡

> 原文：<https://hackaday.com/2012/04/18/reading-credit-cards-with-a-tape-head/>

一家名为 Square 的公司正在发放免费的信用卡读卡器，可以将任何 iPhone 或 iPad 变成销售终端。[史蒂夫]拿起一个微型外设，做了任何正常人都会做的事情:[拆开它，了解它是如何工作的](http://cosmodro.me/blog/2011/mar/25/rhombus-square-iskewedi/)。这个硬件有点不起眼；这并不奇怪，因为 Square [正在把他们送走](https://squareup.com/)。随着简单性而来的是容易理解，并且[史蒂夫]能够成功地用这个小小的免费信用卡阅读器读取他自己的信用卡。

[Steve]解码信用卡数据的工作建立在[Count Zero]在 bbs 上发表的文章[的基础上。基本上，每张信用卡都有两到三个音轨。第三磁道大部分未被使用，而第一磁道包含持卡人姓名、账号、](http://stripesnoop.sourceforge.net/devel/phrack37.txt) [cvc 代码](http://en.wikipedia.org/wiki/Card_Verification_Value#CVC_.2F_CVV)和其他辅助数据。轨道二只包含信用卡号和有效期。

方形读卡器中仅有的组件是磁带放音机的磁头和 1/8”麦克风插孔。方形读卡器中的磁头定位成只能读取磁道二。通过一个小垫片，可以重新调整磁头，从第一磁道获取数据。在录制了他将卡片滑过方形阅读器的音频文件后，[史蒂夫]观察了波形从正到负翻转的次数。由此，他能够获得卡上的 1 和 0，并使用 6 位 ANSI/ISO alpha 格式将它们转换为字母数字。

[Steve]还不打算分享他为 Android 写的代码，但是用他用过的 [Android 教程](http://eurodev.blogspot.com/2009/09/raw-audio-manipulation-in-android.html)复制他的工作应该相对容易。另外，*是的*，我们确实在几个小时前提出了这些方形信用卡读卡器如何工作的问题[。做得好，史蒂夫。向[鲍比]、[叶小开]、[德里克]和其他我们可能漏掉的人致敬。](http://hackaday.com/2012/04/18/hackaday-links-april-18-2012/)

编辑:[Stephen]在这篇文章发布后几分钟就发来了他的评论。黑客读者在这方面太快了。