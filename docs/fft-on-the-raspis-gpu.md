# Raspi 的 GPU 上的 FFT

> 原文：<https://hackaday.com/2014/01/31/fft-on-the-raspis-gpu/>

![fft](img/098cd9f989ea11f08ff630871b3e1f7c.png)

Raspberry Pi 已经出现两年了，但硬件黑客实际上仍然无法利用集成的 GPU 做什么。这种情况正在改变，因为 Raspberry Pi 基金会刚刚发布了一个使用 GPU 进行傅里叶变换的库[。](http://www.raspberrypi.org/archives/5934)

对于那些还没有上过 DSP 课程的人来说，傅立叶变换采用一个函数(或音频信号、无线电信号等)并输出基频。它对从软件定义的无线电到吉他踏板的一切都非常有用，新的 GPU_FFT 库在这项任务上比 Raspi 的 CPU 快十倍。

您可以通过在您的 pi 上运行 rpi-update 来获得 GPU_FFT 库的副本。如果你碰巧制作了什么有趣的东西——软件定义的无线电或者甚至是吉他踏板——非常欢迎你将[发送到 Hackaday tips line](http://hackaday.com/contact-hack-a-day/) 。我们很想知道你在做什么。