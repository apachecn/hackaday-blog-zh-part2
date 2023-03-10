# 密码学——了解它的全部内容

> 原文：<https://hackaday.com/2012/09/25/cryptography-learn-what-its-all-about/>

![](img/cc05b350b1bb66d6245619650061d4f6.png "from-0-to-cryptography-diffie-hellman-key-exchange")

密码学的概念每天都会触及我们的生活很多次，这可能是一个保守的估计。我们已经对它的工作原理有了很好的了解，已经处理了像远程 git 存储库或无密码 ssh 隧道这样的事情的公钥加密。但是我们仍然喜欢阅读[提比略·巴尔布的]关于这个主题的初级读本，他称之为从 0 到密码学的[](http://techblog.rosedu.org/from-0-to-cryptography.html)*。*

 *他从术语的定义开始讨论，但很快转移到密钥分发的主题。如果你用一个密钥来解密数据，你怎么能保证那个密钥只给你想读数据的人呢？一种方法是使用 Diffie-Hellman 密钥交换。上面的图表说明了交易，它使用一个商定的值(在这个例子中是颜色)作为一个共同的起点，然后从那里开始。在完成了密钥交换场景之后，[Tiberiu]接着运行其他选项的 gammut，包括公钥、RSA、散列、数字证书和其他一些选项。考虑到它涵盖了多少主题，这篇文章并不算长。如果你今天没有时间，一定要留到周末。

[via [Reddit](http://www.reddit.com/r/programming/comments/10celr/from_0_to_cryptography/)*