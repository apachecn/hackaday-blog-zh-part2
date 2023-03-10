# 两种浏览器 PCB 工具的故事

> 原文：<https://hackaday.com/2015/08/21/a-tale-of-two-browser-pcb-tools/>

我们生活在一个免费电子设计自动化(EDA)工具的黄金时代。不久前，工程工作站还是一种运行非常昂贵的软件的昂贵硬件，通常需要缴纳年费。现在，你可以去当地的电子商店买一台让旧工作站相形见绌的电脑，并下载大量软件来设计原理图、模拟电路、编程器件和布局 PCB。

许多这种免费软件的唯一问题是它在 Windows 上运行。我有时会运行 Windows，但我最常用的是 Linux，所以在 Web 浏览器中运行的新型工具有一定的吸引力。特别是，我想简单地看一下两个基于网络的 EDA 工具: [EasyEDA](http://www.easyeda.com) 和 [MeowCAD](https://hackaday.io/project/7229-meowcad) 。两者都提供类似的功能:绘制原理图、填充 PCB 和下载制造文件(即 Gerber 文件)。EasyEDA 还提供 SPICE 模拟。

这有很多好处:软件总是最新的。你可以在任何地方使用它，访问你的文件。当然，也有一些缺点:许多人不相信他们的设计在一些外星服务器的手中。还有一个问题是，如果基于网络的服务拔掉插头会发生什么。

最后一个是一个特殊的问题。人们已经证明他们对付费访问网站的容忍度很低。然而，运营一个网站是要花钱的，那么这个工具如何维持下去呢？每个工具对这个问题都有不同的答案。EasyEDA 承诺，如果他们关闭，他们将开放源代码，并提供足够的时间下载文件。当然，好的意图总是会出错，但是如果它们真的关闭了，并且可以按照这个计划来做，你至少可以自己安装软件并继续运行。

另一方面，MeowCAD 已经是开源的了。这意味着你现在可以自己托管它，这将避免你担心他们离开，也可能减轻一些隐私问题。

所以选择很容易，对吧？用 MeowCAD(尽管名字很傻，猫咪主题也有点烦人)。嗯，没那么快。如果你两者都尝试过，你会很快发现 EasyEDA 是更精致的产品。即使没有愚蠢的猫主题，EasyEDA 的工作最像一个传统的包。SPICE 模拟并没有引起我太大的兴趣(很难击败 LTSpice，即使我必须在 Wine 中运行它)。但是在我看来，软件包的其余部分、文档和系统的整体外观都优于 MeowCAD。

当然，在任何一种情况下，您都可以导出 Gerber 文件和示意图，这样您就有了一些设计记录。EasyEDA 将为您提供电路板(价格也非常低)。他们计划通过生产电路板的利润来维持网站。但是，它们不会阻止您下载将您的设计带给任何您喜欢的主板制造商所需的所有文件。

我可以对这两个包中的任何一个做一个回顾，并且我可能会在将来的某个时候这样做。然而，由于两者都是免费的，所以你可以很容易地亲自尝试一下。如果你不能忍受在这两个网站上创建一个免费帐户，这两个网站都有视频演练(见下文)。

[![easyeda](img/0b4220bbb28845928a1a822758f38591.png) ](https://hackaday.com/wp-content/uploads/2015/08/easyeda.png) EasyEDA(左)外观和感觉都像桌面应用。它支持多层板，并具有简单的设计规则检查。它可以生成电路板布局的 2D 模型。有一个新的符号向导(以及一个编辑器)。导航功能使您能够处理复杂的电路板，甚至是跨越多个原理图的电路板。

我唯一的抱怨是，在一个小屏幕上，属性编辑器面板是隐藏的，我花时间试图记住，我必须弹出它来完成某些任务。另一个小问题是，它似乎没有办法使导线具有某种属性，然后从整体上设置它们的属性。例如，最好将所有电源线标记为电源类，然后使该类的所有网络为 12 密耳宽。平心而论，您可以访问该工具的 XML 表示，因此您可以使用自定义的外部工具做类似的事情。

[![meowcad](img/d57dc6b578992846eef9b4c965a9cf0b.png) ](https://hackaday.com/wp-content/uploads/2015/08/meowcad.png) MeowCAD 的工作区还好，虽然菜单和工具栏并不总是那么明显(而且大多看起来像猫)。在我的显示器上很难阅读组件库。总的来说，该应用程序感觉更像一个网页，而不像一个桌面应用程序。如果有一个简单的方法来添加自定义符号到程序中，我找不到它。不要误解我的意思，MeowCAD 拥有它所拥有的特性是令人印象深刻的。然而，如果你把它和 EasyEDA 相比，它远没有那么完美和实用。

[![heart](img/390742adb26445636735cc5428648f4f.png)](https://hackaday.com/wp-content/uploads/2015/08/heart.png)

我还没有用 MeowCAD 制作过电路板，但它似乎足以胜任这项任务。他们的心形轮廓样板(见左图)看起来不错。不过，我已经让 easy 给我做了些板子。这些板(见下文)看起来很棒，而且非常便宜(25 块板，大约 22 美元，外加适度的运费)。诚然，这是一个小板，但如果你报价更大的板，定价似乎是合理的。一些大约 Arduino 大小的双层板 25 块 33 美元。请注意，这些不是每块板的价格，而是总价格(不包括运费)。您可以订购少至 5 块的主板，尽管像往常一样，每块主板的价格会上涨(5 块较大的主板价格为 18 美元，所以价格不到两倍，但数量是原来的五倍)。

[![pcb1](img/95cd828d09115be919ad46b815f1cc91.png)](https://hackaday.com/wp-content/uploads/2015/08/pcb1.jpg)

当然，如果你想要完全免费的设计软件，KiCAD 是一个不错的选择(这两个工具都借用了 KiCAD 组件库；MeowCAD 甚至可以导出到 KiCAD)。如果你能坚持使用 Windows 或者如果你只是想要示意图，还有许多其他的免费选项。然而，今天，我想坚持使用基于浏览器的工具。

尽管我认为 EasyEDA 更加完善，但这两个工具都是可用的，我为 MeowCAD 以源代码形式提供而喝彩。即使您选择使用该网站，如果有必要，您也可以设置自己的安装程序。我确信 EasyEDA 打算留下来，也打算兑现它的承诺，如果有必要，它将如何关闭。然而，我知道如果事情真的变坏了，尽管有良好的意愿，也很难信守承诺。但是现在，我将坚持使用 EasyEDA 来完成一些不太重要的简单项目。工作流程很好，点击一个订购按钮，电路板就会出现在邮件中，这种便利让人难以拒绝。

[https://www.youtube.com/embed/MWll14sQI-A?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/MWll14sQI-A?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[https://www.youtube.com/embed/fhGYMZgFtho?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/fhGYMZgFtho?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)