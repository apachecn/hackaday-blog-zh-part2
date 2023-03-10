# GPU 编程实现简单快速的图像处理

> 原文：<https://hackaday.com/2012/05/30/gpu-programming-for-easy-fast-image-processing/>

![](img/36aa40ea5225479df0e590f2448aecb8.png "gpu")

如果你需要快速处理图像，或者只是想制作一些漂亮的分形图，[Reuben]正好满足你的需要。他开发了一个[简洁的命令行工具](http://reubenjcarter.github.com/GPU-Programming/)来将代码发送到显卡，并使用像素着色器生成图像。与用 CPU 制作这些图像不同，GPU 并行处理每个像素，使图像处理速度快得多。

所有的 GPU 编码都是通过在 [GLSL](http://en.wikipedia.org/wiki/GLSL) 中写一点代码来完成的。[Reuben]的命令行实用程序获取该代码，将其发送到显卡，并返回由 GPU 计算的图像。用这种方法制作漂亮的[曼德布洛特设定图像](https://github.com/ReubenJCarter/GPU-Programming/blob/master/Mandelbrot.jpg)和[正弦波干扰](https://github.com/ReubenJCarter/GPU-Programming/blob/master/SineWaves.jpg)非常简单，但是【鲁本】的项目能做的远不止这些。通过将图像发送到 GPU 并执行一些操作，[Reuben]可以对预先存在的图像进行非常快速的边缘检测和其他算法处理。

到目前为止，[Reuben]已经在 Windows 和 Linux 下用一些 NVIDIA 显卡测试了他的软件，尽管它应该可以与任何带像素着色器的显卡一起工作。

虽然[Reuben]正在向他的 GPU 发送代码，但它不完全在 [NVIDIA CUDA](http://www.nvidia.com/object/cuda_home_new.html) 并行计算平台的水平上；[鲁本]只研究图像。不过，巧妙编写的软件可以绕过这个问题。尽管如此，即使[Reuben]的项目只用于图像处理，它仍然比任何 CPU 绑定的方法快得多。

你可以在 GitHub 上下载一份[Reuben]的作品。