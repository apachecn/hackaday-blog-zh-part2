# 由压电和麦克风构建的声纳

> 原文：<https://hackaday.com/2015/01/26/sonar-built-from-piezo-and-microphone/>

[Jason]继续开发他的声纳系统，最近展示了一个使用压电元件和麦克风的单基地主动声纳。普通读者会记得“一周失败”帖子中的[杰森的]实验，其中[关注的是他在更早的原型中的防水问题](http://hackaday.com/2014/10/02/fail-of-the-week-sonar-submersibility-sealing/)。

我们发现这种产品更有吸引力。他抛弃了那些实验中看到的超声波模块。新装置使用 27V 电源驱动压电元件。每个 ping 发出后，麦克风输入会立即被捕获，以检测声音的返回。[Jason]提到他在项目中使用的 TI Launchpad 对于这些实验来说足够快，但他可能会切换到 Teensy 3.1，以便使 RAM 加倍，从而增加他能够记录的样本大小。

当然，这是为了水下遥控潜水器，所以他的下一次迭代将涉及 DIY 水听器。我们迫不及待地想看到这一点，因为将这个测试设备转换成水下工作的过程避开了我们。如果你对这个话题有什么建议，请在评论中告诉我们。

[https://player.vimeo.com/video/117110029](https://player.vimeo.com/video/117110029)

[via [危险原型](http://dangerousprototypes.com/2015/01/21/audible-frequency-chirp-sonar-with-the-stellaris-launchpad/)