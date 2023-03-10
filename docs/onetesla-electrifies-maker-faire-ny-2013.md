# OneTesla 电气化制造商博览会纽约 2013

> 原文：<https://hackaday.com/2013/09/24/onetesla-electrifies-maker-faire-ny-2013/>

![onetesla](img/8d5a4a5f316ce8a6f27bbcf35e9ddd11.png)

在整个创客馆，可以听到音乐特斯拉线圈的警笛声。那些跟着耳朵走的人发现自己来到了 oneTesla 的展台。OneTesla 是一个业余爱好特斯拉线圈，增加了和弦 MIDI 输入的扭曲。

oneTesla 由三名麻省理工学院的学生发起，去年在 Kickstarter 上成功开展了一次活动。像许多 kickstarters 一样，他们在运输部门有点落后。他们正在向支持者运送第三批装备。该集团在展会上有少量 oneTesla 线圈出售，截至周日中午似乎已售罄。

用特斯拉线圈产生声音的实际过程非常有趣。所有特斯拉线圈都是高频共振。在 oneTesla 的例子中，这是 220kHz。人类的听觉在 20kHz 左右结束，所以这远远超出了感知范围。由于线圈被锁定在该频率，线圈的功率被调制到所需的声音频率。例如，演奏一个 A 音符意味着以 440 赫兹调制线圈。

在 OneTesla 中，所有这些都由 [MIDI 中断板](http://onetesla.com/index.php/products/kits/midi-interrupter-kit.html)处理。ATMega328 完成了所有调整线圈的繁重工作。更有趣的是，MIDI 中断器可以通过交错调制的音符来创建两个音符复调。想想视觉风格效果的持久性，但是用音频。断续器还充当线圈的总功率控制，消除了在交流侧使用自耦变压器来控制总线圈功率的需要。

[https://www.youtube.com/embed/VvyWSsEhs-k?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/VvyWSsEhs-k?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)