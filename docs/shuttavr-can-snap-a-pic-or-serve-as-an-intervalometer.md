# ShuttAVR 可以拍摄照片，也可以用作间歇拍摄仪

> 原文：<https://hackaday.com/2013/03/14/shuttavr-can-snap-a-pic-or-serve-as-an-intervalometer/>

![shuttAVR-intervalometer-hack](img/c65bb77b3d91bb74647b29b3fe1c1a73.png)

这个项目开始时是作为一个简单的微控制器的替代品，安装在这个红外摄像机的遥控印刷电路板上。但是焊接工作对 Balthamos 来说相当糟糕，所以他改变了现状，设计了自己的简单 AVR 遥控快门和间隔计。

大部分腿向后弯曲的 DIP 芯片是使系统工作的 ATtiny25。它与电池连接、按钮(在电路板的另一面)和他用左手捏着的红外 LED 的迹线相连。把它对准一架大炮相机，按下按钮就可以拍照了。但是正如你在休息后的视频中看到的，它也可以作为一个时间间隔计；让他拍摄多张照片，每张照片之间有用户定义的暂停。首先按住按钮选择该模式。一旦释放，芯片等待第二次按钮按下登记的延迟。只要稍加改动，新电路仍然适合原来的情况。

[https://www.youtube.com/embed/AxuifhkwKsE?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/AxuifhkwKsE?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)