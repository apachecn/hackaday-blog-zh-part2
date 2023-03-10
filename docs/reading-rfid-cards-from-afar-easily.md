# 从远处轻松读取 RFID 卡

> 原文：<https://hackaday.com/2012/05/27/reading-rfid-cards-from-afar-easily/>

RFID 黑客技术已经存在多年，但迄今为止，所有从某人钱包中嗅出数据的构建都太大、范围太小，或者对于一个随机的 Joe 在他的工作室中构建来说太复杂了。[【Adam】的 RFID 嗅探器](http://colligomentis.com/2012/05/16/hid-reader-arduino-rfid-card-catcher/)避开了所有这些问题，并提供了另一个销毁你信用卡中所有 RFID 芯片的理由。

这个项目的灵感来自于[这个版本](http://www.proxclone.com/Long_Range_Cloner.html),它采用了一个更大的 RFID 阅读器，并把它变成了一个嗅探器，能够从背包或公文包的安全处秘密读取借记卡和护照。[亚伦]的构建使用了一个[更小的现成 RFID 阅读器](http://www.hidglobal.com/prod_detail.php?prod_id=9)，但他仍然能够在大约一英尺远的地方读取 RFID 卡。

[Aaron]的构建非常简单，只包含一个 Arduino 和 SD 读卡器。[Aaron]能够从 RFID 卡中捕获所有数据，将这些数据写入 SD 卡，并使用他的[RFID 克隆器](http://colligomentis.com/2012/05/09/proxmark3-t55x7-cloning-standalone/)模拟一张卡。

这个版本真正令人印象深刻的是，[Aaron]说他不是程序员或电气工程师。他的建造日志充满了自我贬低，显示了(亚伦)是多么的卑微，以及任何拥有必备技能的人克隆你钱包里的银行卡是多么的容易。我们不知道你，但你可能想从现在开始用铝箔衬你的钱包。