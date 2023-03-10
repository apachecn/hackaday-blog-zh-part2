# 利用 GPU 加速 Linux 内核

> 原文：<https://hackaday.com/2012/12/14/leveraging-the-gpu-to-accelerate-the-linux-kernel/>

如今，功能强大的显卡非常实惠。尽管我们很少在日常机器上玩高端游戏，但我们仍然有一台 GeForce 9800 GT。这对一台主要用于发布帖子和为微控制器编写代码的机器来说是浪费。但也许我们可以在编译时很好地利用 GPU。KGPU 包让你的显卡帮助内核做一些繁重的工作。

这并不适用于任何 GPU。该技术使用了 [CUDA](https://developer.nvidia.com/what-cuda) ，这是一个用于 NVIDIA 硬件的并行计算包。但是不要让硬件的缺乏阻止你检查它。[孙伟斌]是这项技术背后的研究人员之一。他在[的网站](http://www.cs.utah.edu/~wbsun/)上发布了[关于这个话题的白皮书](http://www.cs.utah.edu/~wbsun/kgpu.pdf) (PDF)。

将此添加到今天图形硬件的不断增长的[非图形应用](http://hackaday.com/2012/12/06/25-gpus-brute-force-348-billion-hashes-per-second-to-crack-your-passwords/)列表中。

**更新:**看来我们最终不会尝试这个了。你的 GPU 必须支持 CUDA 2.0 或更高版本。我们在[这个列表](https://developer.nvidia.com/cuda-gpus)中找到了我们的产品，它只支持 CUDA 1.0。

[谢谢约翰]