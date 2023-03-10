# 黑客日复古版:300 波特的黑客日

> 原文：<https://hackaday.com/2014/04/27/hackaday-retro-edition-hackadaying-at-300-baud/>

![SONY DSC](img/eae5b1777b94e662d7ff3a5b04a1ceb9.png)

对于像我们的复古版这样的底层网站[，几乎没有理由需要快速的互联网连接。即使是世界上最快的人也只能打出 300 波特。低速连接的问题在于开销，正如【Pierre】在](http://retro.hackaday.com/)[找出一个 80 年代的声学调制解调器](http://www.journaldulapin.com/2014/04/23/connecting-to-the-net-at-300-bauds-with-an-acoustic-modem/)并加载到我们的复古网站时发现的那样。

虽然这不是有史以来第一个调制解调器——那是 20 世纪 60 年代的技术——但它确实以同样的速度运行——每秒 300 比特，或者比你读这句话的速度还慢。[Pierre]将一部台式电话插入调制解调器的杯子，将其插入电话线模拟器，并连接到配备了另一个调制解调器的 Raspberry Pi。从那以后，建立一个 300 波特的终端是相当容易的。

然而，串行连接不是到互联网的连接，在 300 波特的速度下，PPP 几乎是不可能的。封装数据包的开销就是这么高。SLIP 是通过慢速串行连接发送 IP 数据包的更好选择，但是[Pierre]的 mac 没有合适的工具。

[Pierre]最终使用了他的 Mac 和 Raspi 与 Zterm 之间的串行连接。从那以后，Lynx 和 Bob 就是你的叔叔了。

不出所料，下面有一个很长的[Pierre]加载复古网站的视频，以及一个很长的 speedtest.net 以 56k 跑的视频。

[https://www.youtube.com/embed/JgMYSPp0WdM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/JgMYSPp0WdM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[https://www.youtube.com/embed/qG1A24lSb6c?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/qG1A24lSb6c?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)