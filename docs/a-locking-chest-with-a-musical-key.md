# 带音乐钥匙的锁柜

> 原文：<https://hackaday.com/2012/04/17/a-locking-chest-with-a-musical-key/>

![music-detecting-box](img/741ed7068a554c424a8d359d5bf62453.png "music-detecting-box")

[Basil Shikin]正在考虑不同类型的锁，并试图提出一个他尚未看到的锁定解决方案。他意识到自己从来没有遇到过由音乐触发的锁，所以他开始着手建造一把自己的锁。

他在网上订购了一个木制的箱子，然后开始组装锁机制和音乐检测逻辑所需的电子设备。使用与驻极体麦克风配对的 Atmega328P，他的系统监听要播放的特定曲调(时间陶笛发出的光的前奏)，这触发了一个微小的伺服系统来解开闩锁。为了做到这一点，他在 Arduino 上实现了 Goertzel 算法的一个版本，使他能够根据频率准确地检测出神奇的曲调，不管它是在什么乐器上演奏的。

一定要看看下面的视频，看看他的音乐锁在行动。

[https://www.youtube.com/embed/EpMhZ3Fbm5g?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/EpMhZ3Fbm5g?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)