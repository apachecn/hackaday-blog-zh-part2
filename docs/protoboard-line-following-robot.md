# 原板循线机器人

> 原文：<https://hackaday.com/2013/08/03/protoboard-line-following-robot/>

![dspic-line-follower](img/839c24c1adfd7d0011c077b02f420fd6.png)

我们喜欢[一个好的循线机器人项目](http://dangerousprototypes.com/forum/viewtopic.php?f=56&t=4052#p40526),这真的很棒。它有锋利的边缘，大量的焊料桥接，看看那些跳线！尽管外表如此，它的表现不会让人失望。

它使用 dsPIC33 来读取电路板底部的六个模拟传感器。我们不太熟悉芯片的功能，但[Exapod]说它有一个自动扫描功能，他用它来读取传感器。这使他能够以约 30 kHz 的频率对所有六个器件进行 12 位分辨率采样。难怪这个东西在下面的演示视频中反应如此迅速。他使用的轨道只是一些白色打印纸，上面有一圈黑色的电工胶带，有点弯曲。

这也是一个有趣的玩具挑战。这里有一个[让一个六足动物沿着线](http://hackaday.com/2012/11/12/turning-the-hexbug-spider-into-a-line-following-robot/)前进。

[https://www.youtube.com/embed/B0XdQ6GRexo?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/B0XdQ6GRexo?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[via [危险原型](http://dangerousprototypes.com/2013/07/30/line-follower-robot-project/)