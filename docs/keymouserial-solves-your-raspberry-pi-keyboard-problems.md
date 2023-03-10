# KeyMouSerial 解决你的树莓 Pi 键盘问题

> 原文：<https://hackaday.com/2015/06/27/keymouserial-solves-your-raspberry-pi-keyboard-problems/>

所有的笔记本电脑都有内置的键盘和鼠标，唯一的问题是你不能在没有这些工具的电脑上使用它们。至少，直到现在。[Peter]创造了[key mouse rial，以便在他的 Raspberry Pi](http://peterburk.herokuapp.com/keymouserial/)上使用他笔记本电脑的键盘和鼠标作为物理设备，最终解除了束缚我们笔记本电脑人机界面设备的束缚。

KeyMouSerial 的软件复制击键和鼠标信息，并通过他的笔记本电脑上的串行端口发送出去(使用 USB 转串行适配器)。从那里，Arduino 将信息翻译成 HID 命令，通过 USB 发送到目标计算机，在这种情况下是 Raspberry Pi。对于携带笨重的键盘和鼠标来说，这是一个非常优雅的解决方案，只是为了一个 Raspberry Pi，或者对于任何可能无法访问网络和 SSH 的计算机。

[Peter]也一直在使用他的 iPod 作为串行到 USB 的转换器，所以如果你是 Rockbox 开发人员，想帮他一把，就给他写封短信吧。所有的软件都是可用的(适用于 Windows、Mac 或 Linux ),包括 Arduino sketch，如果你想亲自试用这个软件的话。而且，如果你不想把电脑变成键盘，而想反其道而行之，把[键盘变成电脑](http://hackaday.com/2015/03/21/rasppikeyboard-project-called-kiiboard-still-pronounced-keyboard/)，那[也是一个选择](http://hackaday.com/2012/08/14/turning-a-keyboard-into-a-computer-with-a-raspberry-pi/)。