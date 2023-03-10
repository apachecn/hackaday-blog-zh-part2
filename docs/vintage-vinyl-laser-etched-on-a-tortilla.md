# 老式乙烯基激光蚀刻在玉米饼上

> 原文：<https://hackaday.com/2015/07/14/vintage-vinyl-laser-etched-on-a-tortilla/>

[UpgradeTech]有一个概念验证的难题需要解决:用激光切割机将玉米饼制作成可播放的唱片。这个想法源于 YouTube 上一段愚蠢的“[玉米饼黑胶](https://www.youtube.com/watch?v=U1SiveWVIIo)”视频。

使用未煮过的玉米粉圆饼。当煮熟的玉米饼在电唱机上被切碎时，玉米饼太多块了。为了将录音放到玉米粉圆饼上，Audacity 被用来修改立体声 WAV 文件。使用 [RIAA 均衡标准](https://en.wikipedia.org/wiki/RIAA_equalization)是一个很好的选择，因为它最初是用来防止唱针穿过时唱片凹槽的过度磨损。Python 脚本为激光切割机生成了文件，创建了一个包含声音数据的文本文件，该文件随后被处理为凹槽的矢量 PDF。对于每张唱片，激光切割机需要 30 分钟才能将一张简单的玉米粉圆饼变成各种音乐。

每个玉米粉圆饼可以在 45 或 78 转/分钟的转速下播放 30-40 秒的音乐，但一旦变干，它们就会开始翘曲。是时候在电唱机周围建一个雪茄盒了！有背景噪音，可以使某些歌曲更难听到，但有无可争议的听得见的音乐。有足够的空间来优化声音文件、音乐套路和切割。我们希望这个项目能激励其他人制作他们自己的音乐玉米饼。玩你的食物有了全新的意义！

[https://www.youtube.com/embed/rdzCv_9eaoM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&start=43&wmode=transparent](https://www.youtube.com/embed/rdzCv_9eaoM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&start=43&wmode=transparent)