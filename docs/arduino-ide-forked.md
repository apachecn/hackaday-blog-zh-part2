# Arduino IDE 分叉

> 原文：<https://hackaday.com/2015/04/06/arduino-ide-forked/>

好像这些天在 Arduino 世界中还不够混乱，现在我们将不得不处理 IDE 的冲突版本号。是的，它被分叉了。Arduino LLC 正在 arduino.cc 上提供最近更新的版本 1 . 6 . 3(T1 ),但是在 arduino.cc，Arduino SRL 已经将 T2 的版本号提升到 1 . 7 . 0(T3)。命名和版本的冲突[并没有被忽视](https://github.com/arduino-org/Arduino/issues/2)。

对于那些最近一直生活在岩石下的人来说，开发 Arduino 的公司(Arduino LLC)和制造大部分硬件的公司(Smart Projects SRL，现在的 Arduino SRL)已经[停止合作](http://hackaday.com/2015/03/28/arduino-srl-to-distributors-were-the-real-arduino/) , [提起一系列诉讼](http://hackaday.com/2015/03/12/arduino-v-arduino-part-ii/)，现在[维持着单独的网站](http://hackaday.com/2015/02/25/arduino-v-arduino/)。

根据[这篇文章](http://www.golem.de/news/arduino-vs-arduino-kampf-um-die-arduino-ide-1504-113322.html)(谷歌翻译[这里](https://translate.google.com/translate?sl=auto&tl=en&js=y&prev=_t&hl=en&ie=UTF-8&u=http%3A%2F%2Fwww.golem.de%2Fnews%2Farduino-vs-arduino-kampf-um-die-arduino-ide-1504-113322.html&edit-text=&act=url))版本没有太大的不同，1.7.0 IDE 甚至可能比 1.6.3 倒退了一步。在我们看来，Arduino 项目中大多数活跃的开发人员都坚持使用[Massimo Banzi]和 Arduino LLC 阵营。当然，一切都是开源的，没有什么能阻止 Arduino SRL 将有价值的 IDE 更改移植到他们的代码库版本中。

不需要千里眼就能感觉到这可能是对“官方”1.6.1 版本中包含的[关于非授权板](https://github.com/arduino/Arduino/commit/39d1dfc9995e75e858fa238c7c8881ee2d7679c6)的警告的回应。也不需要通灵师来预见未来混乱的时代。

如果你有兴趣做一些代码调查，看看这两个版本，并在下面留下评论，让我们知道你发现的任何实质性差异。

感谢【凯】，以及 via【golem . de】。