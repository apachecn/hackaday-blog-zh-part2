# 现实生活字幕眼镜

> 原文：<https://hackaday.com/2012/07/23/real-life-subtitle-glasses/>

[![](img/3ddfb2a11ecdb678b5d727e5af8b5cb1.png "reallifesub_072212")](http://hackaday.com/2012/07/23/real-life-subtitle-glasses/reallifesub_072212/)

[威尔·鲍威尔]发来了他的[实时字幕眼镜项目](http://www.willpowell.co.uk/blog/?p=219)。受到非常酷的谷歌眼镜项目的启发，他决定尝试自己的版本。

他使用了两个运行 Debian squeeze 的 Raspberry Pi、vuzix 眼镜、麦克风、一台电视、ipad 和 iphone 作为硬件组件。这个项目中的数据流有点奇怪。音频首先被蓝牙麦克风接收，然后通过智能设备传输到网络上的服务器。一旦上传到服务器上，就会通过微软的翻译 API 进行解析。之后，翻译后的信息被发送回 Raspberry Pi，并在眼镜上显示为字幕。

当然，这与《星际迷航》中看到的通用翻译设备相去甚远。被翻译的人必须对着麦克风清楚地说话，这是一个巨大的复杂性。不过，就技术演示而言，这很酷，你可以看到他在休息后使用该系统下棋。

[https://www.youtube.com/embed/vw6dJDMmnlw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/vw6dJDMmnlw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)