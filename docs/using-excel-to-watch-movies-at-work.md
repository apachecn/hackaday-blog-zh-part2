# 工作时使用 Excel 看电影

> 原文：<https://hackaday.com/2014/10/24/using-excel-to-watch-movies-at-work/>

本周早些时候，当 redditor [AyrA_ch]分享了他的自定义电子表格，允许他在锁定的工作电脑上播放视频文件时，Excel subreddit 爆炸了。如何锁定？由于无法访问 Windows Media Player，IE7 是唯一的浏览器(所有插件都被禁用，没有 HTML5)，Excel 成为了治愈 3 小时无聊任务的不太可能的英雄。

在矩形层叠的背后，在 Excel 宏的土地上，[AyrA_ch]利用程序的[VBA](http://en.wikipedia.org/wiki/Visual_Basic_for_Applications)(Visual Basic for Applications)函数来规避计算机的限制。虽然 VBA 通常提供比通常更复杂的宏，但它也可以调用一些 Windows API 命令，其中一个命令调用 Windows Media Player。Excel 文件包括一个工作播放列表和一些基本的控件:播放、暂停、停止等。以及一个灵感饼图倒计时定时器。

尽管这种方法很聪明，但最好的特点要微妙得多:欺骗内部老大哥。[AyrA_ch]的计算机运行一个应用程序来监控进程使用情况，但通过电子表格播放的任何视频都被归入 Excel，以确保进程使用情况符合目标。你可以在 GitHub 上下载。