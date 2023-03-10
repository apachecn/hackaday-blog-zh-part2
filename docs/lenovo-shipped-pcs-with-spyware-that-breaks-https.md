# 联想发货的个人电脑带有间谍软件，攻破 HTTPS

> 原文：<https://hackaday.com/2015/02/19/lenovo-shipped-pcs-with-spyware-that-breaks-https/>

如果你曾经买过新电脑，那么你可能对预装的大量膨胀软件很熟悉。通常有系统工具、杀毒软件试用版和一大堆我们大多数人一开始就不想要的东西。现在我们可以把超级鱼间谍软件添加到列表中了。

你可能想知道是什么让这个案例如此特别。许多个人电脑都预装了为制造商收集使用统计数据的软件。超级鱼是这方面的一个极端例子。该软件实际上安装了一个自签名的根 HTTPS 证书。然后，该软件为用户打开的每个 HTTPS 会话使用自己的证书。例如，如果您访问您的网上银行门户，您实际上不会从您的银行获得证书。相反，你会收到一份由 Superfish 签名的证书。你的电脑会信任它，因为它已经安装了根证书。这实质上是由联想安装的软件执行的中间人攻击。Superfish 使用这种能力对你的加密连接做一些事情，包括收集数据和注入广告。

如果这还不够糟糕，他们的证书实际上使用了一个废弃的 SHA-1 证书，该证书使用 1024 位 RSA 加密。这种级别的加密很脆弱，容易受到攻击。事实上，[有报道称](http://arstechnica.com/security/2015/02/lenovo-pcs-ship-with-man-in-the-middle-adware-that-breaks-https-connections/ "Arstechnica article")Errata Security 的 CEO【Rob Graham】已经破解了证书并泄露了私钥。有了公开的私钥，攻击者可以很容易地伪造任何 HTTPS 证书，感染了 Superfish 的系统就会信任它。用户将不知道他们正在访问一个假冒的网络钓鱼网站。

自从这一发现被发现后，联想[发布了一份声明](http://news.lenovo.com/article_display.cfm?article_id=1929 "Lenovo statement"),称 Superfish 被安装在 2014 年 9 月至 12 月发货的一些系统上。他们声称服务器端的交互从一月份开始就被禁用了，这就禁用了 Superfish。他们没有计划在任何新系统中预装 Superfish。