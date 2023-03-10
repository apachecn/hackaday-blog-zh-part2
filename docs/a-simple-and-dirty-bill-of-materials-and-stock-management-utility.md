# 一个简单(和肮脏)的物料清单和库存管理工具

> 原文：<https://hackaday.com/2014/01/09/a-simple-and-dirty-bill-of-materials-and-stock-management-utility/>

[![](img/97f712eb99ee7f4689f62c73c0f24211.png)](http://hackaday.com/wp-content/uploads/2014/01/bom.png)

正如许多读者可能已经知道的那样，当我没有展示你的项目或者[在 mooltipass](http://hackaday.com/tag/developed-on-hackaday/) 上工作的时候，我会试着做一些可能对电子爱好者有用的简单的东西。我的[最新创造是一个简单的物料清单生成工具](http://www.limpkin.fr/index.php?post/2014/01/09/The-Updated-Bill-of-Materials-and-Stock-Management-Tool)，它也可以做简单的库存管理。不幸的是，对于 Linux 用户来说，这个工具是使用 Excel 文件中的 Visual Basic 函数实现的。

它的工作相当简单:只需在 excel 表格中输入原理图的元件参考，以及相应的 Digikey 网页地址。点击“获取”按钮，脚本将自动从互联网上获取您的所有组件特性，并根据您想要制作的原型数量告诉您组件成本。然后点击“排序 BoM”按钮，您的 BoM 将自动按组件类型和值排序。另一个功能允许您检查 BoM 中的所有组件是否也存在于(非常简单的)Kicad 生成的组件中。最后，使用另一个包含您当前库存的 Excel 表，物料清单将让您知道您是否有足够的组件用于组装阶段。休息后嵌入了工具运行的视频，您可以在这里下载 BoM 模板(。XLSM 文件)和相应的股票文件[那里](http://www.limpkin.fr/public/BoM/Stock_file.xlsm)(。XLSM 文件)。

[https://www.youtube.com/embed/lPLJ8kMP0Uo?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/lPLJ8kMP0Uo?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)