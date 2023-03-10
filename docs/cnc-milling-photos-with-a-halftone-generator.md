# 使用半色调生成器的 CNC 铣削照片

> 原文：<https://hackaday.com/2015/02/23/cnc-milling-photos-with-a-halftone-generator/>

正在寻找一种制作照片或图形的好方法吗？查看[Matt Venn]的[半色调代码生成器](http://www.mattvenn.net/2014/10/07/drill-pic-gcode-generator-updated/)，它可以从任何图像文件创建半色调 CNC 刀具路径。我们之前遇到过[的一些半色调生成器](http://hackaday.com/2011/09/14/making-better-cnc-halftone-pictures/)，但是【马特】的生成器有一些有趣的特性，可以产生一些非常独特的输出。

[Matt]最初用 Python 编写了一个简单的命令行程序，但只是用一个更加用户友好的 UI 重写了他的脚本，当您更改选项时，它会呈现输出的预览。UI 允许您更改参数，如钻孔深度、行数和步长，以调整输出。它甚至可以选择沿着正弦波绘制半色调点，产生如上图所示的有趣效果。

[Matt]的程序生成标准的 gcode，你可以用它来运行你的 CNC 机床。[Matt]建议铣削具有不同颜色层的材料，但您始终可以铣削实心材料，并用油漆或染料填充布线区域。想抓取脚本还是查看源代码？前往[Matt]的 [GitHub 库](https://github.com/mattvenn/cad/tree/master/tools/drillpic2)。

感谢提示，阿基斯。