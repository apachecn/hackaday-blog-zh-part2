# Beverly-Crusher，音效最伟大的名字

> 原文：<https://hackaday.com/2014/10/10/beverly-crusher-the-greatest-name-for-an-audio-effect/>

[![Image is © aliceazzo [http://aliceazzo.deviantart.com/].](img/aa339c8cd523146c064bb034cb9cb73c.png)](http://aliceazzo.deviantart.com/) 

图片 Alice azzo[http://Alice azzo . deviantart . com/]。

说到音频效果，你有你的延迟，混响，合唱，相位，以及其他来自严格的模拟过程。与传统的做事方式相比，数字音频相对较新，新的流程和效果仍有未开发的潜力。其中之一是比特粉碎机，一种将 8 位或 16 位音频变成糊状的效果。[Electronoob]想试验一下比特粉碎，找不到想要的。他毫不气馁，建造了自己的 T8。

有两个主要的影响完全是在数字领域。第一个是采样率降低装置。这有一些有趣的应用。因为[香农]和[奈奎斯特]说我们只能再现低于一半采样率的音频信号；如果你让一些音频通过一个设置为 1kHz 的采样率降低装置，听起来会像废话，但你也只会得到低音。

bitcrusher 有点不同。一位 bitcrusher 只记录一个值(开或关),而不是记录 8 位音频的 256 个值或 16 位音频的约 65000 个值的样本。通过扬声器以合适的采样率播放，你仍然可以听到。这听起来像一个机器人的噩梦，但它仍然存在。

[Electronoob]纯粹用软件创建了他的 bitcrusher，将生成的 bitcrushed 和小得多的文件发送到 Arduino 进行播放。有趣的是，他还包括了降采样音频的能力，以一个的价格为 is project 提供了纯数字效果。1 位音频听起来有点粗糙，但 2 位、3 位和 4 位音频开始听起来很酷，在一些音乐流派中会感觉很舒服。

[https://www.youtube.com/embed/U2mQjJXUQ4k?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/U2mQjJXUQ4k?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)