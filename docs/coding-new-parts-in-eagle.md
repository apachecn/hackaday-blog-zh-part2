# 在 Eagle 中编码新零件

> 原文：<https://hackaday.com/2013/03/31/coding-new-parts-in-eagle/>

![chip](img/dd9d61efa880bd867fbe5182b3c2fa35.png)

在 Eagle CAD 中制作新零件并不是世界上最容易的事情，尤其是当您处理的包不在默认库中时。通常，制作一个新零件意味着要翻出一个数据表，并在 Eagle 中绘制一个新零件。更好的解决方案是用代码生成新的部件——定义焊盘的数量、焊盘的形状、芯片的对称性等等。[【Joost】的 madparts](https://github.com/andete/madparts/wiki) 就是这么做的，允许任何人通过输入数字而不是画线在 Eagle 中创建新零件。

madparts 背后的想法是用 Coffeescript 编写 Eagle 库中的新条目。它对您正在设计的零件有即时的图形反馈，并且能够从 Eagle 库导入和导出到 Eagle 库。一个支持 KiCAD 的版本即将发布，但在此之前，madparts 看起来是一个在 Eagle 的怪异包中创建自己的部件的好方法。