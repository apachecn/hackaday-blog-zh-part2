# 采访:发明 Unix“sudo”命令

> 原文：<https://hackaday.com/2014/05/28/interview-inventing-the-unix-sudo-command/>

这只是其中的一个夜晚。我们坐在奥尼尔的圣马特奥酒吧，在漫长的一天的制造商集会后休息一下。Hackaday 正在举办一场非正式的酒会，源源不断的各色人物刚刚开始涌入。就在那时，我们遇到了[罗伯特·科格舍尔]。

![XKCD comic #149](img/fb540e92483fd5415334408dcdd787aa.png)

[ [xkcd，149](//xkcd.com/149/) ]

一开始是一个普通的讨论——他经营[小批量组装](http://hackaday.com/2014/03/21/hackaday-visits-nova-labs-and-small-batch-assembly/)，在创客空间做了很多有趣的事情。然后他提到了一个有趣的细节——“哦，你知道我在 80 年代也参与发明了数独吗？"

如果您曾经接触过 Unix 系统，您就会知道这是一件大事。更令人惊讶的是，首先必须“发明”出像 sudo 这样的东西。当想到 base Unix toolkit 时，总有这样一种感觉，它是从贝尔实验室深处的一些原始思想中产生的，由[Ken Thompson]和其他人的无限智慧赋予了生命。事实证明并非总是如此。我们不能错过对[鲍勃]的采访，他告诉我们这一切是如何发生的…

##### 黑客

[https://www.youtube.com/embed/LaAwl3HN5ds?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/LaAwl3HN5ds?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

这个故事本身是一个相当普通的故事——它以一个问题开始，以一次黑客攻击结束。[鲍勃]和他的同事[克里夫·斯潘塞]当时在[SUNY/布法罗](http://suny.buffalostate.edu/)工作，[鲍勃]负责他们 Unix 基础设施的管理。因为 Unix 从一开始就是一个多用户系统，所以作为一名系统管理员意味着要以超级用户的身份执行大量的命令。这样做的标准方法是使用“su”命令，该命令使用户能够切换到超级用户模式。虽然这通常会成功，但它为人为错误提供了很多机会——人们太容易忘记自己处于“根”模式，最终导致系统意外损坏。[Bob]和[Cliff]想到了一个更好的方法——与其不停地切换，为什么不简单地创建一个工具，以超级用户的身份执行单独的命令，而不改变 shell 中的实际用户 id。为了实现这样的功能，他们很快就设计了一个组合了两个标准 Posix 系统调用——*setuid()*和 *execvp()* 的黑客。这个命令被命名为“ **sudo** ”，是超级用户 do 的缩写([Bob]坚持认为正确的发音是/ˈsuːduː/，而不是/ˈsuːdoʊ/).

##### 走向开源

在证明了 sudo 是 SUNY 系统管理员不可或缺的工具之后，它开始慢慢进入其他研究小组，并于 1985 年正式“开源”。在那些日子里，开源还没有风靡一时(理查德·斯托尔曼在同一年刚刚发表了他的 GNU 宣言)，所以“开源”的行为实质上意味着在新闻组上发布源代码。1985 年 12 月 15 日，他们就这么做了。[Bob]帮助我们追踪了发布到 [*网上的*](https://groups.google.com/forum/message/raw?msg=net.sources/rdwIP38fbCo/1L3R9K9zbEYJ)*[原始消息。来源](https://groups.google.com/forum/message/raw?msg=net.sources/rdwIP38fbCo/1L3R9K9zbEYJ)*集团。

##### 有巨魔

另一个有趣的历史文物可以在[原始帖子](https://groups.google.com/forum/#!searchin/net.sources/sudo.c/net.sources/rdwIP38fbCo/1L3R9K9zbEYJ)后面的帖子中找到，这是互联网巨魔物种的早期例子:

```

--
isn't this the same as saying:
su -f root -c "some commands here"

why reinvent the wheel? plus this doens't have to be recompiled when
there is a new root passwd.

i find that most unix programs get written again and again and again,
when the one you wanted was already there in the first place.

tom
--

```

虽然 sudo 确实没有发明任何全新的东西，但它做得更好——它为实际问题提供了有效的解决方案。因为[Bob]和[Cliff]足够关心与世界分享它，其他人高兴地采用它并继续改进。今天，sudo 有 9944 行代码(比最初版本的 153 行有所增加)，由[Todd C. Miller]维护。超过 30 年的历史，它仍然继续接受代码贡献，并定期发布新版本。