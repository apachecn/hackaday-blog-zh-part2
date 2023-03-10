# 安卓应用回顾:ADSdroid 给你所有的数据表

> 原文：<https://hackaday.com/2012/04/18/android-app-review-adsdroid-gives-you-every-datasheet-ever/>

![](img/825dfe2eea2c82f3f59e21b5b4b6314b.png "ADS")

几个月前，当我评论 Android 电子参考应用程序 [ElectroDroid](http://hackaday.com/2012/02/10/electrodroid-your-android-electronic-reference-app/) 时，我随口说了一句话，alldatasheet.com 的[的前端应用程序将是一个杀手级的移动电子参考应用程序。[András Veres-Szentkirályi]接受了我的挑战，](http://www.alldatasheet.com/)[开发了 ADSdroid](http://techblog.vsza.hu/posts/Unofficial_Android_app_for_alldatasheet.com.html) ，这是 alldatasheet.com 的非官方安卓应用。休息之后你可以看看我的完整评论。

在我开始这篇评论之前，我想指出[安德拉什]免费赠送 ADSdroid 是因为他认为他的工作存在于道德灰色地带。ADSdroid 只是解析在 alldatasheet.com 上搜索生成的 HTML，去掉广告，然后提供. pdf。这和在你的浏览器中打开所有数据表没有什么不同。不过，alldatasheet 的工作人员靠广告生存，所以我们同意安德拉斯不把他的应用放在 Android market 上的选择可能是正确的决定。

#### 好人

[![](img/679e36f6eaa4d537bf0f203a900071a9.png "atbegin")](http://hackaday.com/wp-content/uploads/2012/04/atbegin.png)

第一次启动 ADSdroid 后，会出现一个简单的文本框，询问您想要搜索哪个部分。像 alldatasheet.com 上的搜索工具一样，你的搜索词可以*包含在*零件名称中，*与*零件名称完全匹配，或者让返回的条目以你的搜索词开始或*结束*。没有像 alldatasheet.com 那样的“按描述搜索”，但我想这个功能不会用得很多。

当 ADSdroid 返回您的搜索结果时，您会看到一个匹配零件的列表。老实说，ATtiny25 可能是我为演示这款应用而进行的最糟糕的搜索之一；alldatasheet.com 为 ATtiny25 微控制器返回两页条目。这些条目只是针对不同电压、速度和不同封装的相同芯片。

![](img/c6a9a4632e0aa630e5fd3d746aa40de8.png "ATTINY25")

点击其中一个条目后，ADSdroid 下载链接的。PDF 并在我的屏幕上显示:

![](img/9adf2e812027eeda1c533a5ddebae4c3.png "atmel")

当然，找到 ATtiny25 的数据手册非常容易。我决定给 ADSdroid 一些更难找到的东西。ADSdroid 可以在 alldatasheet.com 上找到任何东西，拥有一个可移植的参考更有利于用户遇到更深奥的组件。在翻遍我的零件抽屉寻找最奇怪的零件来对抗 ADSdroid 后，我最终选定了东芝公司生产的线性 CCD，零件编号 TCD143D:

![](img/77d41cfef880366a0c1a67ef2beb0fd5.png "linearCCD")

ADSdroid 怎么样？恐怕不太好。ADSdroid 仅仅是 alldatasheet.com 的一个前端，所以任何不是由 alldatasheet 托管的东西都不会被找到。ADSdroid 确实找到了我的线性 CCD 芯片的两个近亲；可能好到足以得到引脚，但除此之外没有太多。

![](img/73204a71b747813d5c5f0efa6174dcb6.png "TCD")

#### 这还是很好的

尽管 ADSdroid 无法准确找到我需要的东西，但它的能力取决于它背后的数据库。Alldatasheet.com 没有每一个电子元件的信息，但 ADSdroid 很好地完成了它的工作。

有几个功能/缺陷，我相信有些人会抱怨:首先，没有内置的 PDF 浏览器。ADSdroid 依赖于手机上默认的 PDF 查看器。虽然这是一个很好的软件设计选择，但如果您没有安装 PDF 查看器，您将无法查看数据表。

其次，ADSdroid 默认将 pdf 保存到内部 SD 卡。同样，这是一个很好的设计选择，但我发现当我用 [MyPhoneExplorer](http://www.fjsoft.at/en/) 记录截图时，为什么下载总是失败，这让我非常困惑。没什么大不了的，我只是需要一个让 cyanogenmod 给我原生屏幕捕捉支持的方法。

最后，还有一个问题是会返回几十个名称相似或相同的组件，我在搜索“ATtiny25”时就遇到过这种情况。对于 ADSdroid 的用户界面来说，给用户一个看似相同的项目列表供选择是一个可怕的问题，但这个问题可以很容易地解决，但对于每个唯一的搜索结果只返回一个结果就不那么容易了。(见下面 vsza 的评论)

我知道这是一个过于苛刻的评论。ADSdroid 是一个非凡的工具，现在就在我手机上的 ElectroDroid 旁边。它确实是一个很棒的应用程序，如果它能在安卓市场上买到，我会很乐意花一美元买它。

因为安德拉斯对他的应用程序有一些道德问题，他还没有把它放在 Android Market(或 Google Play)上。相反，他提供了。apk [在他的网站](http://techblog.vsza.hu/posts/Unofficial_Android_app_for_alldatasheet.com.html)和来源[在 github](http://techblog.vsza.hu/posts/Unofficial_Android_app_for_alldatasheet.com.html) 上。只需下载。apk，把你的手机连上 USB 线，转到 SD 卡上。一个非常简单的安装，如果你知道你在做什么。如果你甚至在考虑用一个应用程序来下载数据手册，你可能有安装 ADSdroid 的技术技能。

总之 ADSdroid 就是我一直在等的 app。根据一位用户的评论，当前的 Android 数据表应用程序比书签好不了多少，因此[András]应用程序填补了移动电子参考类别的一个巨大空白。尽量不用太多就好；我们不知道 alldatasheet.com 的人们是否会对服务感到满意。没有广告收入的 pdf。