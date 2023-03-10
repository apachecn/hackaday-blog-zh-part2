# 无线鼠标的速射模式

> 原文：<https://hackaday.com/2014/08/30/rapid-fire-mod-for-a-wireless-mouse/>

![Rapid Fire Wireless Mouse](img/0426cc72c3ce19d142423674634b3219.png)

有时更换电脑鼠标会让你不舒服一段时间，直到你习惯了更换。可能还需要一些时间来适应新的功能或新鼠标缺乏的功能。[Jon]买了一个他非常喜欢的超棒的无线鼠标，但是它缺少一个关键的功能:游戏的快速射击。他之前改装了他的老式有线鼠标，用 555 定时器设置了一个快速发射按钮。这在鼠标耗尽 USB 的 5 伏电压时工作正常，这是 555 定时器需要的电压。新的无线鼠标有 1.5 伏电池，不支持 555 定时器。[游戏玩家做什么](http://tsjwang.blogspot.com/2013/10/wireless-555-timer-mouse-modification.html)？

[乔恩]搜索了整个网络，但没有找到任何无线速射模块。最终，他找到了一种叫做 LMC555 的低压变体，并为他的项目订购了一些。新的无线鼠标被拆开，以了解鼠标按钮是如何工作的。在这种情况下，当按下鼠标按钮时，信号引脚被拉低。现在我们知道了鼠标按钮是如何工作的，只需要几个电阻、一个电容、一个 NPN 晶体管和一个按钮开关就可以完成这个模块了。当按下按钮时，LMC555 定时器激活晶体管，以便将鼠标按钮信号引脚接地。这种情况每分钟发生 1236 次！那是大量的快速射击。

几个组件被整齐地焊接在一起，装进了鼠标内部有限的备用区域。鼠标外壳侧面钻有一个孔，将新的快速发射按钮固定在符合人体工程学的位置。

早些时候，我们提到过[Jon]以前在有线鼠标上做过这个模型。他在 Hackaday 上了解到这个项目。如果你的有线鼠标渴望一个快速发射按钮，看看吧。

休息后的视频…

[https://www.youtube.com/embed/mfyascZjakI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/mfyascZjakI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)