# 用你的思想在潘多拉上点赞歌曲

> 原文：<https://hackaday.com/2014/02/07/thumbs-down-songs-on-pandora-with-your-mind/>

史蒂文喜欢音乐。像我们许多人一样，他使用潘多拉来享受熟悉的音乐，并发现新的音乐。潘多拉的本意是好的，但她有时会弄错。[Steven]有一个 Mindwave 移动脑电图耳机已经有一段时间了，他决定好好利用它。借助树莓派和蓝牙模块，[他建造了脑波控制的潘多拉轨道推进系统](http://stevenhickson.blogspot.com/2014/02/controlling-music-with-your-mind.html)。

这个想法是基于你的脑电波来识别你不喜欢一首歌。[脑波](http://store.neurosky.com/products/mindwave-mobile)给出了许多不同脑波的数据，以及近似你的注意力和冥想水平。由于[Steven]并不精通 brainwavery，他使用贝叶斯估计生成了两个多元高斯模型。一个代表好音乐，一个代表烂音乐。产生的算法大约有 70%的准确率，所以【史蒂文】的 Python 脚本在推进音轨之前会连续等待四次“坏音乐”的估计。

【Steven】通过 [pianobar](http://6xq.net/projects/pianobar/) 传输 Pandora，并在[他的 GitHub repo](https://github.com/StevenHickson/MusicEEGControl) 中有一个控制-pianobar 脚本的修改版本。如果耳机没有很好地接触皮肤，他的脚本也会提醒你，这是一个 Mindwave 报告的变量，范围是 0 到 200。

留下来观看[史蒂文]用意念控制潘多拉的演示。如果你没有脑电图耳机，你仍然可以用 Pi，pianobar 和一些漂亮的按钮来控制 Pandora。

[https://www.youtube.com/embed/KogQT437Xe8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/KogQT437Xe8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)