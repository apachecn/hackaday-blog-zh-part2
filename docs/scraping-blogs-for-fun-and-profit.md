# 为了乐趣和利益而抓取博客

> 原文：<https://hackaday.com/2012/06/13/scraping-blogs-for-fun-and-profit/>

![](img/242184118cc6f77d25a7a2635d439874.png "py")

有时当你在解决一个问题时，一个解决方案就摆在你面前。几天前，我们在整理 Hackaday 的新复古版时，发现自己正处于这种情况；我们需要一种随机选择一篇黑客文章的方法，codepanel.net 的亚历山大·范·特灵根给了我们解决方案。

为了抓取每个 Hackaday URL，[Alex]使用 [Beautiful Soup](http://www.crummy.com/software/BeautifulSoup/) 屏幕抓取库编写了一个小 Python 脚本。该程序从 Hackaday 的主页开始，在进入下一页之前，抓取 Hackaday 帖子的每个链接。这并不是一个非常复杂的构建，但是我们惊讶于我们正在处理的问题的解决方案会神奇地出现在我们的收件箱中。

多亏了[Alex]，编写一个 cron 作业来自动更新我们的[新复古版](http://retro.hackaday.com/)变得简单多了。如果你想查看有史以来(或者至少是两天前)所有黑客帖子的列表，你可以在这里找到 10693 行文本文件[。](http://retro.hackaday.com/assets/hackaday.com.txt)