# 秘密阁楼图书馆的门

> 原文：<https://hackaday.com/2014/12/25/secret-attic-library-door/>

我们有一个很好的猜测:[Krizbleen]在哪里为他的家人藏了任何季节性礼物:在他闪亮的新秘密图书馆门后面。作为一名经验丰富的木工，【Krizbleen】在装修家中阁楼的过程中，他决定利用烟囱在他即将成立的办公室前的恼人位置。他在中央烟囱障碍物前建造了一堵假墙，并在墙中间(烟囱正前方)放置了一台电视，两侧各有一个书架。

然而，如果你触摸秘密书或敲出秘密序列，右边的书架会轻轻滑出，露出[克里兹布林的]家庭办公室。在幕后，一个重型线性致动器根据需要推或拉门，[Krizbleen]熟练地将书柜安装在上面，带有一些 2 英寸的脚轮。致动器期望+24V 或-24V 将它发送到两个方向中的一个方向，因此 Arduino Uno 需要几个继电器来处理电压差。

这里花费了巨大的努力，但结果是天衣无缝的。在借用了一个敲门探测脚本并在一本书里挂了一个二级访问按钮后，[Krizbleen]有了他一直想要的秘密之门:尽管打开和关闭可能有点慢。你可以在下面看到它的操作视频。

[https://www.youtube.com/embed/saLP7EKy3VM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/saLP7EKy3VM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)