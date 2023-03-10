# [Jeri]展示了一个德尔塔适马 ADC

> 原文：<https://hackaday.com/2012/11/05/jeri-shows-off-a-delta-sigma-adc/>

![](img/d4c55e7d0882ab0d93d0399837bd8d55.png "DeltaSigma")

[Jeri]升级到 Valve 软件经历了一段时间，但是电子显微镜安全地放在她的车库里。)而她的电子实验室也在慢慢成型。由于她无法拿出她正在制作的现实生活中的重力枪，她决定[展示一个一位 ADC](https://www.youtube.com/watch?v=DTCtx9eNHXE) ，它只使用一个触发器将模拟波形采样成数字数据。

通过切换 74xx74(或任何触发器)的时钟输入，并将互补输出反馈到数据输入，[Jeri]可以获得一个占空比为 50%的输出，输入到芯片的输入端。向此数据输入添加一个音频输入，并在此反馈环路中添加 10k pot，将导致占空比相对于模拟输入发生变化，从而形成一位 ADC。

和任何电子捷径一样，也有一些缺点:输入触发器的时钟周期必须非常快；如果采样音频，至少需要几十千赫。尽管如此，如果你没有空闲的 ADC 引脚，或者你只是想建立一个破碎的吉他踏板，这是一个非常简单(和便宜)的方式将模拟变成数字微。

[https://www.youtube.com/embed/DTCtx9eNHXE?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/DTCtx9eNHXE?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)