# 滑翔飞机用变程计

> 原文：<https://hackaday.com/2012/11/15/variometer-build-for-gliding-aircraft/>

![](img/7df1324ca5173281ae9c34eca0e4a4a2.png "variometer-for-hang-gliding")

如果你在一个没有动力的交通工具中在空中飞行，你的下降率是你想要保持的。考虑到这一点，[阿德里安]决定[设计他自己的变仪](http://villamany.blogspot.com.es/2012/11/tinyvar-un-vario-medida.html) ( [翻译](http://translate.google.com/translate?sl=auto&tl=en&js=n&prev=_t&hl=en&ie=UTF-8&layout=2&eotf=1&u=http%3A%2F%2Fvillamany.blogspot.com.es%2F2012%2F11%2Ftinyvar-un-vario-medida.html))，它将在驾驶舱中其他仪器旁边占有一席之地。它发出一种音调，其频率由高度增减的速率决定。

他用 PIC 24FJ64 微控制器来驱动这个装置。它从 MS5611 气压传感器读取数据。这测量了与高度变化相关的气压变化。作为用户界面，他选择了 SparkFun 的诺基亚 5110 液晶屏分线板。他还带了一个升压转换器，可以只用一个电池为设备供电。表壳本身是用数控铣床从几层塑料上切割下来的。

在广告之后的视频中，你可以看到这个设备是多么的敏感。只要上下移动几英尺，就会对声音和显示的数据产生直接影响。

[https://www.youtube.com/embed/-3N-Qq-q5Jw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/-3N-Qq-q5Jw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)