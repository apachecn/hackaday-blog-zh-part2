# qtled test–评估有机发光二极管显示器的软件

> 原文：<https://hackaday.com/2014/01/02/qtledtest-software-to-evaluate-oled-displays/>

[![](img/e5ce5e533b62842804df1a74a557fc4b.png)](http://hackaday.com/wp-content/uploads/2014/01/qtledtest_screenshot.png)

几天前，我们特别推出了 USB pass T1，这是一款由很少组件组成的离线密码管理器。在我们文章的最后，我们提到[Josh]已经在开发他的硬件的另一个版本，包括在平台上增加一个有机发光二极管屏幕。为了帮助他选择一个，他[创造了 QtLedTest](http://sroz.net/projects/qtledtest) ，一个基于 Qt 的工具，模拟不同的有机发光二极管显示和 GUI 布局。内部 QtLedTest 由 [QLedMatrix](http://qt-apps.org/content/show.php/QLedMatrix?content=101193) (一个模拟 LED 矩阵的小部件)、一个 SSD1306 有机发光二极管控制器模拟器、一个简单的图形绘制库和一些在模拟屏幕上绘制文本的函数组成。[Josh]使用了 [Fontbuilder](https://github.com/andryblack/fontbuilder) 和他制作的一个程序，以便将他在互联网上找到的字体转换成 C 文件。所有[Josh]制作的源代码都可以在 Github 上找到，应该会在未来几周内更新，因为最终的程序渲染模拟屏幕有点慢。