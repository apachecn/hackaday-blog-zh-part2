# sharemail 试图扰乱美国国家安全局的电子邮件监控

> 原文：<https://hackaday.com/2013/11/28/scaremail-tries-to-disrupt-nsa-email-surveillance/>

![scaremail](img/c9babb50ca8b65d8bfe78dac44478a80.png)

你在国家安全局的电子邮件监控名单上吗？你想成为吗？这个项目名为 [ScareMail](http://bengrosser.com/projects/scaremail/) ，旨在扰乱美国国家安全局的电子邮件监控项目。

[Benjamin Grosser]将它作为许多流行的网络浏览器的插件编写，它使用一种算法在你的电子邮件签名中生成一个聪明但最终无用的叙述，尽可能多地使用可能的 NSA 搜索词。这背后的想法是，如果有足够多的人使用它，它将使国家安全局的搜索结果超载，最终使他们的电子邮件关键词跟踪无用。

那么它是如何工作的呢？该算法从自然语言处理(NLP)和一个原始文本源开始——他选择了雷·布雷德伯里的 *华氏 451 度。使用处理器，它识别原始文本中的所有名词和动词，并用适当格式和共轭的“可怕”单词替换它们，这些单词是他从假设的 NSA 关键字列表中索引的。为了确保每个签名都是唯一的，他利用一条 [马尔可夫链](http://en.wikipedia.org/wiki/Markov_chain) 来生成每次都完全不同的新文本。结果是一个有点连贯的段落，没有任何实际意义。*

但是等等！像这样的监视是不好的，但假设它可以工作！嗯，也许吧。但重点是:

> ScareMail 揭示了美国国家安全局监视工作的一个主要缺陷:言不由衷。

休息后留下来看看本自己对 ScareMail 的视频解释。

[https://player.vimeo.com/video/75828491](https://player.vimeo.com/video/75828491)

喜欢这个项目？他还制作了一个有趣的 [【脸书·德米特里克特】](http://hackaday.com/2012/10/23/hacking-facebook-to-remove-the-social-value-facade/) ，从每个人都喜欢的网站上去掉了社会价值的外表。