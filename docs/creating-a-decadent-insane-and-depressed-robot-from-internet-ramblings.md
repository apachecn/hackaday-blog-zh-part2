# 从网络漫谈中创造了一个颓废、疯狂、抑郁的机器人

> 原文：<https://hackaday.com/2012/07/15/creating-a-decadent-insane-and-depressed-robot-from-internet-ramblings/>

![](img/77f68668f734e09d0d6e6302b4202b13.png "robots")

你有没有想过一个精神病机器人写的 Tumblr 会是什么样子？不要再想了，因为[拉斯]已经想通了。

几年前，[Lars]偶然发现了 lowbrow.com(现已不存在，但在这里有镜像)，这是一个在线忏悔和浴室墙，旨在匿名展示人们最隐私的想法和行为。[Lars]写了一个脚本，每分钟拉下一个随机的低俗帖子，并将每个唯一的结果放入数据库。

在大约 50 页真实性可疑的最堕落和令人沮丧的帖子中，[Lars]训练了一个[马尔可夫链](http://en.wikipedia.org/wiki/Markov_chain)算法来产生模仿低级作者风格的段落。这给了[Lars]几页计算机生成的文本，描述了最颓废、最压抑、最疯狂、最空洞、但却是最具人性的经历。来自[输出](http://retro.hackaday.com/assets/out.txt)的几个选择报价是:

> 美洲驼:大自然的随机数发生器。
> 
> 超过 7000 瓦的老巴里抱怨他的屁股脸颊，以减轻打击。
> 
> 整个上学期间，我都被拉到当地的圣本笃会修道院后面，我害怕我不知道我想的是创始人从关于 homestarrunner.com 的讨论中退缩了

虽然[Lars]的脚本无法通过图灵测试，但我们遇到过做不到这一点的人。至于创造一个现实生活版本的快乐主义机器人，哈尔和马文从搭便车的指南，我们认为[拉尔斯]击中了目标。

休息过后，你可以看看 Lars 从电脑生成的文本中收集的图片。你也可以抓取[完整的低级语料库](http://retro.hackaday.com/assets/lowbrow_dump.txt.gz)和[ruby 脚本](http://retro.hackaday.com/assets/markov.rb)来构建你的机器人【凯鲁亚克】。

[![](img/e09f9cf26204a88fee479a289002faae.png)](https://hackaday.com/wp-content/uploads/2012/07/panel_1.jpg)[![](img/a98a64a10a03da7e6950a40c9205134a.png)](https://hackaday.com/wp-content/uploads/2012/07/panel_2.jpg)[![](img/1165416b1be243d49e44c4ce5d4ace26.png)](https://hackaday.com/wp-content/uploads/2012/07/panel_3.jpg)[![](img/b7da83940f004c2c6885545cd98653b9.png)](https://hackaday.com/wp-content/uploads/2012/07/panel_4.jpg)