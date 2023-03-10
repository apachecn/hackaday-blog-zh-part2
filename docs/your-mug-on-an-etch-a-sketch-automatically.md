# 你的杯子会自动蚀刻出草图

> 原文：<https://hackaday.com/2012/05/14/your-mug-on-an-etch-a-sketch-automatically/>

![](img/8128f0b7a811f7aca9486a431a8647f8.png "your-candidate-on-an-etch-a-sketch-mitt")

[吉姆]对他蚀刻素描很认真。他不辞辛苦地建造了一个能够像蚀刻素描一样自动渲染照片的装置。你能认出这幅图中的美国政治人物吗？当重新组装的身体准备挂在墙上时，他实际上把这些打开，并移除所有的内部构件来保存艺术品。但是我们喜欢他使用的黑客友好的界面技术。

他用一对步进电机移动旋钮。它们的附着得益于他模拟的一对 3D 打印齿轮，齿轮越过枪托旋钮，并用四个固定螺钉固定。他说，他可以在五分钟内使用这些设备以及支撑机身和电机的 MDF 夹具进行打印。

他将照片转换成 1 位图像，然后通过 ImageMagick 将它们转换成文本文件。Python 脚本解析该文本，向驱动电机的 Arduino 发送适当的命令。图像绘制得很像扫描 CRT 监视器。手写笔一次跟踪一条水平线，如果像素应该是黑色的，就画一条曲线，如果像素应该是白色的，就跳过这条曲线。

我们希望有打印过程的视频。既然没找到，休息之后还有一个和这个无关的加分项目。这是一个蚀刻素描钟。

[https://www.youtube.com/embed/NBbNn8Tkb6I?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/NBbNn8Tkb6I?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)