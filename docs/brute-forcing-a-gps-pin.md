# 暴力破解 GPS 密码

> 原文：<https://hackaday.com/2013/01/05/brute-forcing-a-gps-pin/>

![pin](img/31269f66d731c05285d1398afad03818.png)

[JJ]最近在拍卖会上买了一个 Garmin Nuvi 780 GPS。[JJ]遇到的更令人沮丧的功能之一是它的个人识别码；这个 GPS 无法解锁，除非输入一个四位数的代码，或者被带到一个“安全的位置”。不想让他的拍卖横财白白浪费，[JJ]装配了一个自动暴力破解机器人来解锁这个 GPS。

这个机器人是围绕一个旧的惠普扫描仪和一个 DVD 驱动器滑板建造的，用来在 X 轴和 Y 轴上移动 GPS。一个由橡皮擦笔尖和伺服系统组成的聪明的小装置会敲出从 0000 到 9999 的每一个代码，然后等一会儿看这个装置是否解锁。[JJ]的机器人输入一个密码大约需要 8 秒钟，所以输入所有 10，000 个密码大约需要一天半的时间。

幸运的是，输入这些代码的人并不太关心他们的 GPS 设备的安全性。用来打开[JJ]全球定位系统的密码是 0248。机器人只花了几个小时就输入了正确的代码；我们认为这段时间花得值。

休息之后，你可以看看机器人的暴力行为。

[https://www.youtube.com/embed/sHp4px45uQY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/sHp4px45uQY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)