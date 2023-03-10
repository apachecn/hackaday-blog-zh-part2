# 更新:口哨平台升级为简单的单词识别

> 原文：<https://hackaday.com/2013/08/22/update-whistled-platform-upgraded-for-simple-word-recognition/>

有些人可能还记得我[limpkin]不久前设计的口哨平台，它可以识别不同的口哨来控制你的灯光。最近，我设计了一个固件，可以将电路板转换成一个[文字识别设备](http://www.limpkin.fr/index.php?post/2013/06/30/The-whistled%3A-from-whistle-to-sound-recognition)，因为 50MHz ARM Cortex M4 的处理能力足够好，可以做到这一点。

简单算法的工作原理是将放大麦克风输出的连续快速傅立叶变换(FFT)与先前存储在存储器中的模板字的 FFT 相关联。只需将口哨连接到你的电源，说出你想让它识别的单词，你就可以开始了。

正如您将在休息后嵌入的视频中看到的那样(抱歉有口音……)，我简要解释了关于单词/声音识别的基本原理，以及您可以做些什么来提高您的算法性能。源文件可以下载，还有我的哨声检测算法的[代码，我们第一次看这个项目](http://www.limpkin.fr/index.php?post/2013/04/26/The-whistled%3A-how-to-remake-a-dozen-years-old-project-the-right-way)的时候[没有这个代码。](http://hackaday.com/2013/05/18/just-put-your-lips-together-to-turn-on-a-lamp/)

[https://www.youtube.com/embed/s4OKan-Szqw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/s4OKan-Szqw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)