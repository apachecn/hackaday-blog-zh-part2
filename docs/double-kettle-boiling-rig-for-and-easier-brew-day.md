# 双壶煮沸设备，更容易酿造一天

> 原文：<https://hackaday.com/2012/11/09/double-kettle-boiling-rig-for-and-easier-brew-day/>

![](img/6178cef8ae3f04695eccd48568c3e595.png "double-kettle-electric-boiling-system")

[戴夫]制造了一个控制器，让他在酿造啤酒时同时煮两壶啤酒。该装置在每个水壶中使用电加热元件。我们更喜欢用煤气，因为它更容易控制温度。但是像这样的电力系统可以在冬季室内使用，而丙烷则被转移到室外。我马上想到的另一件事是部分糖化食谱，需要浸泡在一个壶中，然后用不同温度的水喷射(冲洗谷物)。这种事情很容易，因为这两个是由控制箱前面的微调按钮单独控制的。

里面有两个 220 伏固态继电器。盒子本身插在他地下室的 220 伏插座上，这个插座通常被他的干衣机电线占用。为了不烧断保险丝，MSP430 芯片驱动继电器在它们之间来回切换，而不是同时打开两个继电器。该系统完全采用手动控制，但如果需要，添加热电偶和 PID 算法应该很容易。

休息过后，[Dave]在一个视频剪辑中展示了该系统。

[https://www.youtube.com/embed/eHrI0EKLxtk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/eHrI0EKLxtk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)