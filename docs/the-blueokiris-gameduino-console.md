# BlueOkiris Gameduino 控制台

> 原文：<https://hackaday.com/2014/08/01/the-blueokiris-gameduino-console/>

![3011851406903369314](img/dee77f6ff2bbea8d60446fd77aafdc05.png)

[迪伦]用 Arduino Uno、一个临时按钮、一个模拟棒和一个 TFT LCD 触摸屏屏蔽创造了一个易于制作的游戏控制台。另外，他用胶带做了一个简单的纽扣。

到目前为止，他已经做了 2 场比赛。一个是臭名昭著的 Pong。另一种是“猜数字”式的体验。整个项目在代码中运行，不像使用 [2boots](https://github.com/thseiler/embedded/tree/master/avr/2boots) 或常规 [Gameduino 适配器](http://excamera.com/sphinx/gameduino/)那样直接访问引导加载程序。

构建说明可以在[Dylan]的 hackaday.io 项目页面上找到(上面有链接)。本质上，所有需要的是收集电源，然后拿起按钮和模拟棒，完成一个电路，将明线安装到数字引脚 9 的插槽中。将导线焊接到位，并将地与地、5v 与 5v、x 与 A4、y 与 A5 相连。加 TFT 盾，插个 micro SD 卡，上传个游戏。

要查看它的运行情况，请在休息后观看视频:

[https://www.youtube.com/embed/wNBl15fcvTI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/wNBl15fcvTI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

这就对了。一台 Arduino 游戏机。

其他类似的项目包括信用卡大小的游戏机和 UnoJoy，这使得你的 T2 Arduino 可以很好地与 Xbox 360 或 PS3 配合使用。