# Snapchat 个人验证在不到 100 行代码中失败

> 原文：<https://hackaday.com/2014/01/22/snapchat-person-verification-defeated-in-100-lines-of-code/>

![out](img/7d2c18b9ad7be185d0fa81c92e8e2cba.png)

[史蒂文·希克森]今天早上醒来，看到一篇关于 Snapchat 实施的新个人验证系统的文章。三十分钟后[他用不到 100 行代码(](http://stevenhickson.blogspot.ca/2014/01/hacking-snapchats-people-verification.html) [GitHub](https://github.com/StevenHickson/FindTheGhost) )破解了这个问题，由计算机来解决。

先说一点背景。大约一个月前，460 万 Snapchat 用户的信息被一个安全漏洞泄露。为了提高安全性，Snapchat 实施了[一种新的个人验证方法](http://news.cnet.com/8301-1023_3-57617592-93/snapchat-now-makes-sure-youre-a-real-person/)，以确保新账户不是由电脑创建的。

方法？从一系列九幅图像中挑出一个白色幽灵。有点像可爱的，不那么讨厌的验证码。问题？这是证明你是一个人的可怕方式。史蒂文只用了 30 分钟就编写了一个程序，使用简单的阈值、冲浪关键点和 FLANN 匹配来找到鬼魂。在他的测试中，他 100%准确地找到了鬼魂。他还沉思着有一种更有效的方法来做这件事，他只是懒得去做。

不错的尝试 Snapchat。