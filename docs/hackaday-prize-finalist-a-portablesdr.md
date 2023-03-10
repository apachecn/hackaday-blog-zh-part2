# Hackaday 奖决赛选手:便携式 SDR

> 原文：<https://hackaday.com/2014/11/05/hackaday-prize-finalist-a-portablesdr/>

除了迈克尔·科尔顿的便携式电脑之外，没有其他项目能让人们把钱砸向电脑屏幕，希望会有什么事情发生。这是一款软件定义的无线电，设计覆盖范围高达 30MHz。世界各地的业余无线电运营商都对这个项目感兴趣，甚至称之为第一个宝丰 UV-5R 杀手。那可是*极其*的高度赞扬。

[迈克尔]非常友好地坐下来，回答了几个关于他如何进入 Hackaday 奖的问题。你可以看看下面，以及该项目的最后一轮视频。任何想要拥有自己的便携式电脑的人都可以通过参加这个调查来真正帮助迈克尔。

[https://www.youtube.com/embed/Yb5tmzy5dFs?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/Yb5tmzy5dFs?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

```
*What was the inspiration for this? Was it just a desire to build
the radio you wanted, and doing something with SDR, or was it 
something deeper?*
```

这不是一个真正的灵感时刻，我不知道它有多深。它进化了。我第一次了解 SDR 收音机是在阅读 Gerald Youngblood 的这篇文章时。我被这种事情的存在震惊了！一台基本上无所不能的收音机！？我想有一个，但负担不起，我需要建立自己的。因此，我重读了几遍文章，研究了原理图，直到我非常明白每个部分是如何工作的。他没有提供材料清单，所以我重新做了一份。我当时也不知道怎么布局 PCB，就开始学了一点 Eagle。但是生活变得繁忙，其他事情发生了，我再也没有重建他的收音机。随着我技能的提高，特别是在使用微控制器方面做得更好，我开始想我可以简化他的一些设计(他有一整板的移位寄存器，允许 PC 并行端口控制一切)。大约一年前，我开始接触内置 DAC 和 DSP 库的 ARM 芯片。我开始认为这些芯片中的一个可以做所有的事情。所以现在我可以把电脑拿出来，如果可以的话，我可以把它变得便携，突然之间，它对我来说比以前更有吸引力了！将所有这些与我对超轻背包和人体工程学的兴趣结合起来，这就是 PortableSDR 概念的形成。

此时，我已经掌握了[一定程度的 PCB 布局技能](http://hackaday.com/2014/09/07/thp-hacker-bio-michael-r-colton)，并开始在设计上取得进展。当我看到这个的时候，我还没有做太多[，我的一部分说，“我已经想做这个很多年了，他只是在几天内就做出了这么酷的东西！？我给他看看！”事实上，我和里奇有一段时间互通了电子邮件。然后 Hackaday 奖宣布了，我正式得到了我需要的东西。虽然我不喜欢截止日期，但它真的很有帮助。对于 PSDR1，有一段时间我决定“必须制作 PCB，这个版本中不包含任何其他内容。”同样的事情也发生在 PSDR2 上，“这是我得到的所有东西，其他的都必须放在下一个里。”它迫使我去构建一些东西，而不是无休止地争论这部分或那部分是否会完全正确地工作。这也让我有理由花掉我一直存着的一点钱。](http://hackaday.com/2014/04/25/building-a-software-defined-radio-with-a-teensy)

```
*You have a GPS module, and doing CTRL+F 'APRS' reveals nothing on 
your project logs. What's the timeline for that?*
```

你说得对，全球定位系统还没做多少工作。它最初不包括 APRS，它是为了获得像 JT65 这样的低功耗数字传输模式的准确时间。我不知道有 HF APRS 这种东西。将它用于紧急定位的想法也是后来才有的。我以前在另一个项目中使用过这个模块，所以我并不担心它的工作，但让其他功能工作似乎是更优先的事情，所以 GPS 的东西一直被搁置。虽然我或多或少移植了 TinyGPS 库。我可能很快就会有时间和地点的工作。现在，编写编码和解码这些模式的代码已经远远超出了我目前的舒适水平。我会实现的，但是考虑到我从社区得到的巨大的积极响应，我想有人可能会抢先我一步。我需要更多的硬件。

```
*A number of people have called the PortableSDR the first Baofeng UV-R5
killer, a very impressive compliment given that's everyone's go-bag 
apocalypse radio. You're producing kits, but are there any plans to move 
to full-scale manufacturing? Is that going to require a redesign, or are
you been designing for manufacturing the whole time?*
```

哇！那确实是高度赞扬！宝丰收音机最大的优点之一就是它的价格，你怎么能不买呢！在这方面我肯定无法竞争。另一方面，在真正的天启中(我听说犹他州是僵尸天启的可能起点之一，顺便说一句)，我认为像 PortableSDR 这样的高频无线电的范围将更有用，它方便的显示将使从少数分散的幸存者那里找到信号更容易。说到这里，我希望这个东西很坚固，适合背包旅行，但也因为我不喜欢一次性电子产品。我希望 PortableSDR 能在社会完全崩溃后，仍能支撑并正常工作数年。

事实上，我还没有真正开始销售套件。我把所有的 PSDR1 板都发给了我项目的热心追随者。其中至少有两个已经建好了(感谢 John Laur 和 Nricciar)！我计划对额外的 PSDR2 板做同样的事情，但还没有得到它。我将在我的项目页面上发起一个投票。我想知道有多少人想要套件还是组装单元。有多少人想要住房？金属的还是塑料的？如果我做套件，人们真的愿意焊接其中一些零件吗？一些人要求一套安装了硬部件的套件，这很公平。有多少人想要原样的 PSDR2，又有多少人会等待 PSDR3(可能要等一段时间)？我几乎可以立即开始制作套件(可能在接下来的一两周内开始计划)，但组装电路板和外壳将是更多的工作。我确实为制造设计了电路板和外壳，我的大部分设计经验来自工作，所以这是一种习惯，但我从来没有让制造发生，选择组装室等。令人望而生畏。此外，似乎 100 单位的最低订单是正常的(至少在我看来。嘿 Hackaday 蜂巢思维，有什么建议吗？！)因此，我可能要花 20-30，000 美元来启动 PSDR 的第一次生产运行，这还不包括住房或 FCC 认证！我想我会建一个 Kickstarter，这样我就可以看看是否有足够的需求来支付成本。我很想在野外看到这些！我真的很想看看人们是否会参与进来，并帮助它变得令人惊叹，就像我认为它有潜力一样。这整个过程很吓人，但是很刺激！

```
*Hypothetical, and we’re not going to hold you to whatever answer you give.*
*You win the grand prize, a trip to space or about $200,000 USD. Which one*
*to you take, and what is your reasoning for doing so?*
```

这个问题我想了很多，尽管我努力不去想它。我真的很想去太空，错过这个机会会让我心碎，但这笔钱会对我的生活和家庭产生更大、更持久的影响。大部分会花在无聊的东西上，税收(我想人们忘记或者不知道税收是对奖品征收的！虽然我确实看到太空旅行对此有一些津贴，这是可怕的和慷慨的！)、什一税、抵押、储蓄等。

很大一部分将用于继续开发(实验室玩具！)和 PSDR 的制作。还有，我想我会带我的妻子去日本和台湾。这很奇怪，但是我有一个清单，上面列出了我可能会花在哪些事情上，按照利弊排序。

如果是轨道的，会有什么不同吗？我也想过这个问题。我不得不承认，例如，在国际空间站呆上一周可能比我能忍受的更有诱惑力。但话说回来，有人评论说，到达并停留在国际空间站将花费大约 5000 万美元。那样的话，我还是得拿钱！

```
*Anything else?*
```

我有一些激烈的竞争！我一直在关注其他四个，我真的很喜欢他们！当我看他们的视频时，我不禁感到矛盾，我希望我是获胜的一方，但他们的东西太棒了！他们都很努力，做了惊人的工作，他们中的任何一个都应该获胜。我真的很感谢 Hackaday 和邪恶的超载把这个放在上面，它刺激了一些惊人的项目，并一直是一个有趣的吨。我希望 Hackaday 继续展示竞赛中产生的其他项目。感谢所有在我的博客、youtube、reddit 甚至其他博客上鼓励我的项目的人！它帮助我在整个过程中保持动力和兴奋！我会给你做很酷的东西！*