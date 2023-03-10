# 声学脉冲标记器用铅笔跟踪声音

> 原文：<https://hackaday.com/2014/10/07/acoustic-impulse-marker-tracks-sounds-with-a-pencil/>

![Acoustic Impulse Marker (aiming device)](img/3dec3ce80449117e5d6edd1e3bf2f2e6.png)

康奈尔大学的两名学生组装了一个相当奇怪的声音跟踪设备，称为[声脉冲标记器。](http://people.ece.cornell.edu/land/courses/ece4760/FinalProjects/f2013/agw39_mag338/agw39_mag338/agw39_mag338/agw39_mag338.html)

[亚当·弗罗贝尔]和[迈克尔·格里桑蒂]研究电气和计算机科学，在他们最后的微控制器课上，他们决定用古老的 ATmega 1284p 制造这个设备。

该系统使用三个麦克风阵列来精确定位尖锐噪声，精确度在 5 度以内。微控制器检测麦克风之间的“声学延迟”,从而识别声源矢量的位置。它使用 8 级模拟系统将每个麦克风的声音转换为二进制信号，从而识别每个麦克风何时听到噪音。然后比较产生的 3 个二进制信号的时间延迟，选择两个最近的麦克风，然后根据每个麦克风的大小进行简单的角度计算，以确定声音的位置。

当声音被识别时，它的位置被发送到一个 180 度的伺服系统，该系统以 1:2 的比例与铅笔“指针”相匹配，这使它具有 360 度的指向能力。

该系统最适合尖锐的声音，但偶尔也会拾取语音。

[https://www.youtube.com/embed/hxsMbl1AFXw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/hxsMbl1AFXw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[via [被黑的小工具](http://hackedgadgets.com/2014/10/07/acoustic-impulse-marker/)