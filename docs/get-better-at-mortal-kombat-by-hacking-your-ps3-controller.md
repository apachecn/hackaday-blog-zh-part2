# 黑客入侵你的 PS3 控制器，在真人快打玩得更好

> 原文：<https://hackaday.com/2015/01/24/get-better-at-mortal-kombat-by-hacking-your-ps3-controller/>

像真人快打这样的格斗游戏为你提供了各种不同的招式。包括踢、打、抓等。它们通常还包括你能完成的各种组合动作。这些连击动作需要你以正确的顺序按下正确的按钮，还需要你正确的计时。[Egzola]意识到他可以黑掉他的控制器来模拟按键。这绕过了学习曲线，让他只需按下一个按钮就能完成更复杂的组合。

[Egzola]从拆开他的 Playstation 3 控制器开始。有两个 PCB 的内部通过带状电缆连接。幸运的是，这种电缆的每个衬垫都标有相应的控制器按钮。这使得破解控制器变得极其简单。[Egzola]把他自己的电线焊接到每个焊盘上。每根电线都是不同的颜色。然后，电线进入两个不同的连接器，使它们更容易挂在面包板上。

然后在试验板上断开每根电线。来自每个按钮的信号通过 4n25 [光隔离器](http://hackaday.com/2014/10/10/macgyvered-optoisolator-is-a-great-introduction/ "Optoisolator")传输。从那里，信号返回到各个 Arduino 引脚。4n25 芯片将控制器电路与 Arduino 的电路隔离开来。Arduino 还连接了两个按钮。这些按钮安装在 PS3 控制器上。

现在，当[Egzola]按下其中一个按钮时，Arduino 会感应到按钮的按下，并按照预编程的顺序模拟按下各种控制器按钮。结果是一个毁灭性的组合动作，通常需要练习和重复才能记住。你可能会说[艾佐拉]可以把时间花在学习动作上，但这不是重点，不是吗？请观看下面的视频进行演示。

[https://www.youtube.com/embed/ZMxE_EeapMI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/ZMxE_EeapMI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)