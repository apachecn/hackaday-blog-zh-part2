# 笔记本电脑触摸板和 MIDI 控制器

> 原文：<https://hackaday.com/2013/10/26/laptop-trackpads-and-midi-controllers/>

![pads](img/63004d080436b3c9fee72ab81614c9ef.png)

一堆连接到 MIDI 输出端口的焊盘和 Akai MPC 一样古老。创造一个自制版本是很棒的，但是[【斯科特】把他的版本向前推进了一步](http://scottmetoyer.com/radix16-laptop-touchpad-matrix-midi-controller)。他使用旧的笔记本电脑触控板来控制每个触控板被点击时的音符开和音符关命令，还添加了触摸压力以及 x 轴和 y 轴位置的 MIDI CC 值。

触控板是相同的型号，每个都有自己的 PS/2 输出。制造了几个带状电缆到 8 针接头适配器，整个套装被包装在一个奇妙的枫木和铝制外壳中。

电子设备基于 Arduino Mega，每个触摸板有 16 个时钟和数据点，占用了“duino”上 54 个可用引脚中的 32 个。PS/2 协议是有据可查的，但是运行 16 个独立的 PS/2 id 肯定不行。[Scott]最终编写了自己的异步 PS/2 通信库，将他的 midi 设备的延迟降低到大约 50 毫秒。

这是一个令人惊叹的套件，相对便宜，因为[斯科特]现在有一个 16 通道的 Kaoss pad。该设备的视频连接到下面的一个微型机器人。

[https://www.youtube.com/embed/X0AUrA_6aCM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/X0AUrA_6aCM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)