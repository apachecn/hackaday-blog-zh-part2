# 把多氯联苯变成艺术

> 原文：<https://hackaday.com/2013/03/27/turning-pcbs-into-art/>

设计一个电路，设计一个电路板，然后把它送去制造是如此简单，任何人都可以做到。事实上，很多人都是这样，使用 KiCAD 和 Eagle 等传统工具，很多不同的电路板看起来非常非常相似。你总是可以在你的电路板上添加一些很酷的丝网印刷图形，让它脱颖而出，但[Saar]有一个更好的解决方案:它被称为 [PCBmodE](http://boldport.blogspot.com/2013/01/introducing-pcbmode.html) ，它允许你艺术地绘制电路，而不是我们已经习惯的 45 度角。

PCBmodE 获取存储在 JSON 文件中的电路板的零件、焊盘、信号和过孔，并将其转换为 SVG 表示。然后，文件被传送(手动传送，但[Saar]正在进行自动传送)和栅格化，以便可以发送到生产部门。

你可以在 bitbucket 上下载 PCBmodE [,但是现在它仍然是一个非常早期的版本。](https://bitbucket.org/boldport/pcbmode/overview)[通孔和倒铜正在工作](http://boldport.blogspot.com/2013/03/pcbmode-update-copper-pours-and-stuff.html)，但是【萨尔】到目前为止只制造了[这块板](http://boldport.blogspot.com/2013/02/first-look-at-pieceof.html)。