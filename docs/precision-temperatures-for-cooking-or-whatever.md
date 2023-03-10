# 烹饪或其他的精确温度

> 原文：<https://hackaday.com/2014/06/26/precision-temperatures-for-cooking-or-whatever/>

![sous-vide temp controller](img/ef91acbdaf69da5978547febe608a17d.png)

如果你没有听说过真空烹饪法，你并不孤单。这种方法使用低温水浴来烹饪密封塑料袋中的食物。因为温度比正常情况低得多，烹饪时间必须长得多，实际温度非常关键。优点是食物受热均匀，不会过度烹饪外部。由于食物是袋装的，它也保留了水分。

[Brian]组装了一个[真空控制系统](http://www.instructables.com/id/Sous-Vide-Oven-Controller/?ALLSTEPS)来自动保持电饭煲的正确温度。一个温度控制装置是从易贝购买的，价格约为 15 美元。考虑到它有一个 LED 显示屏，控制按钮，内置继电器和温度计输入，这是一个不错的交易。控制单元安装在一个带有一些其他部件的项目箱内。120 伏交流线进入接线盒，零线和地线连接到控制单元和标准插座。热线直接连接到控制单元，控制单元通过使用其内置继电器来确定热线是否连接到插座。

![sous-vide temp controller](img/ca162d26ebd593ca28c438f5bed2fcf5.png)

一个 3.5 毫米耳机插孔也安装在项目盒中，以便连接温度计。看看[Brain]是如何防止温度计接触电饭锅的，他把它安装在一个搅拌器里。让温度计远离电饭锅内表面可以确保准确读取水温，而不是加热元件的温度。基于从温度计接收的信号，控制单元确定是否打开电饭煲。

因为这个项目使用一个标准插座作为它与炊具的接口，它可以用于任何依赖于环境温度的东西。如果太热，它可以打开空调，或者控制 3D 打印机的[加热外壳](http://hackaday.com/2014/03/19/heated-build-chambers-dont-have-to-be-that-complex/)。

[ [通过 24 小时工程师](http://24hourengineer.blogspot.com/2014/06/2014-06-24-tu-sous-vide-oven.html)