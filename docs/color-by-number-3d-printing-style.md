# 按数字显示颜色 3D 打印样式

> 原文：<https://hackaday.com/2015/08/19/color-by-number-3d-printing-style/>

还记得按数字上色工具吗？您的画布具有带编号区域的轮廓，您用相应编号的颜料绘制这些区域。当你完成后，你已经重新创造了蒙娜丽莎。[KurtH3]使用类似的技术从他的 3D 打印机中获得多色打印。

这种技术不是通用的，但它仍然是一种有趣的方式来为您通常的单色打印添加一些颜色。这个想法很简单:你找到一个按数字绘制的布局(显然，你可以通过谷歌搜索找到它们)。用你最喜欢的方法将轮廓输入 CAD 程序。[KurtH3]并没有真正深入这方面的细节，但一些 CAD 程序会直接导入图像。其他人会要求您在 Inkscape(或类似的程序)中进行描摹，并将其转换为 3D CAD 程序可以导入的矢量格式，如 DXF。

诀窍在于:不是将 2D 图像挤压成一片，而是将数字区域挤压到稍微不同的高度。假设你想印刷一面红、白、蓝三色的旗子，厚度约为 5 毫米，你用了 0.2 毫米的层。例如，您可以将白色部分挤压到 5 毫米。然后，红色部分可以挤压到 5.2 毫米(高一层)，蓝色部分可以挤压到 5.4 毫米。您可以扩展这个想法，做多层，尽管这将增加表面粗糙度。

[KurtH3]在层的末端暂停打印以改变灯丝，但是我们可能会编辑切片 g 代码以在正确的位置放置暂停(例如，Repetier Host 允许您在文件中放置@pause)。你也可以使用[软件来分割 g 代码](http://hackaday.com/2015/04/06/3d-printing-different-colors-with-a-single-extruder/),就像我们之前提到的那样。使用我们的示例，最终的打印结果将是自下而上的白色，但在顶部的正确位置会有薄薄的红色和蓝色层。白色表面与其他颜色之间几百微米的差异意味着你不会得到完美光滑的表面，但几百微米的差异不应该太明显。

停止打印机和更换灯丝并不是一个新的想法(例如，见下面的视频)。这里有趣的想法是从按数字绘制图像开始，并根据颜色进行挤压。

[https://www.youtube.com/embed/sk1aP6MQEhc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/sk1aP6MQEhc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)