# 混沌通信营 2015:从第一天开始派遣

> 原文：<https://hackaday.com/2015/08/14/chaos-communication-camp-2015-dispatch-from-day-one/>

在四年一度的黑客户外会议[混沌交流营](https://events.ccc.de/camp/2015/wiki/Main_Page)这里有太多的事情要做。在会谈、项目和研讨会之间，几乎没有一分钟时间坐下来写总结。尽管如此，我还是旁听了一些讲座。下面是第一天发生的一些事情的快速概述，以及一个 5000 人黑客营工作的幕后情况。

## 政治

混沌计算机俱乐部从一开始就在政治上很活跃，第一天就反映了这一传统。有一个关于美国国家安全局和黑客可以做什么的谈话(用德语),政治上的[和技术上的](http://media.ccc.de/browse/conferences/camp2015/camp2015-6857-nsa-untersuchungsausschuss_-_wer_kontrolliert_wen.html)[来保护他们自己免受大规模间谍活动。](http://media.ccc.de/browse/conferences/camp2015/camp2015-6733-privacy_badger.html)

[![shot0001](img/5cd3e23e33042f6d48a77c9d85002f6a.png)](https://hackaday.com/wp-content/uploads/2015/08/shot00012.jpg) 也不是说德国现在没有自己的[国内监控丑闻](http://www.spiegel.de/politik/deutschland/harald-range-in-der-netzpolitik-affaere-ranges-rebellion-a-1046704.html) ( [谷歌翻译](https://translate.google.com/translate?sl=auto&tl=en&js=y&prev=_t&hl=en&ie=UTF-8&u=http%3A%2F%2Fwww.spiegel.de%2Fpolitik%2Fdeutschland%2Fnetzpolitik-affaere-gebt-die-akten-frei-kommentar-a-1048024.html&edit-text=&act=url))。在过去的几个月里，Netzpolitk.org 的两名博客写手被控叛国罪，因为他们披露了 BND(德国联邦调查局/中央情报局)用于国内监控的部分预算，而[他们在这里](http://media.ccc.de/browse/conferences/camp2015/camp2015-7043-kontrolle_ist_gut_landesverrat_ist_besser.html)讲述了他们令人毛骨悚然但充满希望的故事。

就在案件公开后，人们走上街头示威，要求新闻自由，政治家们与这一决定保持距离，因为很明显，国家检察官超越了他的界限，新闻自由的价值超过了对国内间谍能力造成的微小损害。检察官丢了工作，最后国家甚至帮助博客作者进行辩护，并帮助支付他们的一些法律费用，这是一件相当体面的事情。

## 拉德 10:谈话

[![rad10_hackaday](img/69d6e4dc2ff16e580145b58312ad1889.png)](https://hackaday.com/wp-content/uploads/2015/08/rad10_hackaday.jpg) 慕尼黑营地花了一整天的时间研究与 [rad1o 徽章](http://rad1o.de)相关的硬件、固件和软件:消除 bug、扩展功能，并帮助人们将额外的 WS2812 LEDs 焊接到徽章上。从昨晚到今晚，已经发放了 3500 多枚徽章，还有足够多的留给落后者。但是尽管表面平静有序，从想法到巨大的徽章努力的道路并不完全平坦。

我们最喜欢的硬件恐怖故事是在 6 月发现，在 2 月发布的制造商数据表中有一个勘误表，显示 BGA 封装是错误的。(谁会下载最新版本的数据手册，只是为了在您布置电路板时仔细检查是否有错误？我们现在会的。)的修复？用 0.25 毫米的钻头从电路板的另一侧钻出引脚。那还不到一根头发宽。

这个由慕尼黑团队进行的演讲，还有一个额外的嘉宾环节，主讲人不是别人，正是 Michael Ossmann，他是 HackRF board 的开发者，徽章以此为灵感和模板。Michael 做了一个感人的演讲，讲述了他开发 HackRF 的过程，以及他如何错过了在美国 [Toor 或【Camp 分发该工具的最后期限，粉碎了他让 100 名黑客在帐篷里玩 SDR 的梦想。通过开源硬件的魔力，以及芯片制造商 Maxim 和恩智浦的一些甜蜜赠品，他在社区中看到了 4000 多种(类似的)SDR 工具。](http://toorcamp.toorcon.net/)

虽然演讲很棒，但黑客们不会等着演讲才开始工作。随着徽章在人们手中不到 24 小时，固件错误被粉碎，大量带有(大部分)有趣动画的拉请求被发布。现在，整个营地的人都有了徽章，我们希望这种情况继续下去，并希望得到一些甜蜜的射频黑客。

## SatNOGS

【2014 年 Hackaday 奖获得者 SatNOGS 发表了一篇关于他们分布式卫星监控项目的演讲。该讲座基本上是对整个系统的概述，并再次呼吁参与该项目。特别是，他们最近[推出了他们的开放数据库](https://satnogs.org/2015/07/satnogs-db/)，以配合他们的开源硬件卫星跟踪项目。现在，当您构建您的跟踪器时，您可以将数据提交到全局项目中。好样的，色鬼！

(哦对了，你获得 2015 年[大奖](https://hackaday.io/prize)的时间不多了。Gogogo！)

## 幕后:沟通

混沌通信阵营:通信是它的中间名。在这个网站上，这些谈话正在通过 DVB-T 进行本地广播。拿一台普通的(数字)电视来看，你就可以收听并观看。如果你不在这里，你可以在家看。

有一个营地电话网有 42(！)基站，使用 [DECT 电话](https://en.wikipedia.org/wiki/Digital_Enhanced_Cordless_Telecommunications)，任何携带(或借用)电话的人都可以在本地系统上获得一个四位数的电话号码。自然，这些也与外部世界联系在一起。由于 DECT 的手机已经有点旧了，如果你有一张营地 SIM 卡，营地还提供 GSM 服务。GSM 网络目前由商用 SDR(当然是带放大器的)供电，但 POC 团队正在将其转换为在 camp badge 上运行，你猜对了。现在这是一个黑客。

没有提到数据厕所，任何来自营地的报道都是不完整的。如果你参加过黑客危机，有两个问题可以给出答案“Datenklo”:“你把一个声学调制解调器叫做什么，因为它的马桶座圈像密封圈一样？”或者“什么是防水、通风良好的外壳，可以方便地安装在装满千兆网络交换机的服务器机架上？”在营地里，你通过一根以太网电缆从你的帐篷连接到 Datenklo，通过一个专门的志愿者团队的“魔法”,你可以获得比在家里更好的连接:在你的帐篷里。那是黑客露营。

当然，Datenklo 还配有闪光灯。自从 2011 年的最后一次露营以来，达滕克洛人已经升级了速度和灯光。他们现在有一串串 WS2812 LEDs 显示全彩色动画。技术进步从不睡觉！

## 这仅仅是开始

我花了大部分时间和慕尼黑的工作人员一起玩徽章，所以毫无疑问我们错过了很多。好在露营的日子里有 21 个醒着的小时，从早上 7 点左右开始，一天到晚，直到凌晨 4 点左右。即便如此，我们确信我们已经错过了很多。如果你在营地看到这篇文章，请在评论中大声喊出来，让我们知道我们从第一天起还错过了什么。