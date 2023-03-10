# 踩高跷节拍音频 ReCAPTCHA

> 原文：<https://hackaday.com/2012/06/15/stiltwalker-beat-audio-recaptcha/>

![](img/6421001e7986767ec8d4057faba3b0f8.png "defeating-audio-recaptcha")

这个来自 2012 LayerOne 会议的演讲概述了团队如何构建高跷，[一个可以击败音频 reCAPTCHA](http://www.dc949.org/projects/stiltwalker/) 的包。我们都熟悉为了确认你是人类而需要输入的模糊的单词图像(事实上，有一个猫捉老鼠的游戏来[破解那个视觉版本](http://hackaday.com/2009/04/29/times-poll-hacked/))。但是你可能没有注意到让别人给你读单词的选项。第二个选项是踩高跷者的努力目标，当时团队达到了 99%的准确率。我们想提醒读者，音频是很重要的，因为只有视觉的确认是视觉障碍用户的一个祸根。

这都是过去式了。事实上，在演讲前大约一个小时(休息后嵌入)，谷歌升级了系统，使其更加复杂，并打破了这些人已经完成的东西。但是听到他们的功绩还是很有趣的。系统中只使用了 58 个单词。该团队发现有一种方法可以利用这些单词的条目，只需拼错足够多的单词，就可以验证它们是多达三个不同单词中的任何一个。机器学习被用来提高解析音频的准确性，但在它可靠地独立运行之前，它仍然需要数万次人工验证。

[https://www.youtube.com/embed/rfgGNsPPAfU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/rfgGNsPPAfU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[via [Reddit](http://www.reddit.com/r/programming/comments/v1ogp/stiltwalker_is_a_proof_of_concept_tool_that/)