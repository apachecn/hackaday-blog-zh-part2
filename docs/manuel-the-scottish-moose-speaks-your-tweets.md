# 苏格兰驼鹿曼纽尔说你的推文

> 原文：<https://hackaday.com/2012/12/19/manuel-the-scottish-moose-speaks-your-tweets/>

![tod1](img/339bfc8e09b934f57619ae216ddb76ee.png)

火炬箱的人今年需要一张圣诞卡。以前，最受欢迎的节日贺卡是一个网页，让访问者有机会激活“造雪机”并向随机的员工喷洒五彩纸屑，所有这些都是在线播放的。他们想在今年复制虚拟和现实生活互动之间的这座桥梁，于是会说话的麋鹿曼纽尔诞生了。

曼纽尔需要一种个性，需要与互联网上随机的人互动，所以火炬箱团队决定让假驼鹿头在树莓派的帮助下实时发布推文。运行在 Raspi 上的代码获取带有#tbxmoose hashtag 的 tweets，通过 node.js 脚本发送，最后发送到 [Festival 语音合成系统](http://www.cstr.ed.ac.uk/projects/festival/)。

在 Manuel 出现在互联网上之前，需要对他进行一些修改。他的下巴被砍成两半，一个伺服和电子控制器被添加进来，以便在 Torchbox 的《曼纽尔的随想之流》中进行适当的演示。