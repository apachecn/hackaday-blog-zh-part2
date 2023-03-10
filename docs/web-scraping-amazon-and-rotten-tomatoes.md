# 亚马逊和烂番茄的网络抓取

> 原文：<https://hackaday.com/2013/01/23/web-scraping-amazon-and-rotten-tomatoes/>

![web-scraping-amazon-and-rotten-tomatos](img/47f4b9f9afac157a9403fc82f8dfdbee.png)

[Rajesh]充分利用网络搜集来收集对他来说重要的信息。他就此发表了两篇文章。一个人每天浏览亚马逊网站，看看他想读的书是否达到了一定的价格门槛。[另一个刮烂番茄](http://rawdust.com/rotten/rotten-tomatoes-audience-scores.htm)为了显示收视率最高的出租电影的评论分数旁边的观众分数。

Web 抓取使用脚本以编程方式从 HTML 中收集信息，而不是使用 API 来访问数据。我们最近推出了主题为的概念教程[，甚至遇到了](http://hackaday.com/2012/12/10/web-scraping-tutorial/)[一个抓取了我们所有帖子](http://hackaday.com/2012/06/13/scraping-blogs-for-fun-and-profit/)的黑客。[拉杰什的]技术是非常相同的。

他使用 Python 脚本和漂亮的 Soup 模块来解析 DOM 树以获得他想要的信息。在亚马逊脚本的例子中，他为他正在寻找的某本书设定了一个目标价格，并会在该书到达时自动收到一封电子邮件。在考虑一部电影时，烂番茄有时喜欢看观众评分，但你无法在网站的列表中找到它；你必须点击进入每部电影。他的脚本保存了一个数据库，这样就不会不断地抓取相同的信息。如上所示，收集的数据显示在评论家得分旁边。