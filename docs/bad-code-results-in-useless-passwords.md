# 糟糕的代码导致无用的密码

> 原文：<https://hackaday.com/2014/12/07/bad-code-results-in-useless-passwords/>

[HeadlessZeke]很高兴尝试他的新美国电话电报公司无线电缆盒，但很快就被捆绑在一起的所需无线接入点所困扰。显然，为了使用有线电视盒，您还需要启用这个接入点。他不是一个盲目地将未知设备放入网络的人，[HeadlessZeke] [做了一些调查](http://goto.fail/blog/2014/11/25/at-and-t-u-verse-vap2500-the-passwords-they-do-nothing/ "The passwords they do nothing")。

无线接入点是 Arris VAP2500。乍一看，事情似乎很好。它使用 WPA2 加密法，使用一个看似随机的长密钥。然而，更多的挖掘揭示了大量的安全问题。

[HeadlessZeke]很快就找到了 web 管理门户。当然，这需要认证，他不知道凭证。[HeadlessZeke]尝试连接尽可能多的页面，但它们都需要用户验证。除了一个。在 web 服务器的根目录下有一个名为“admin.conf”的纯文本文件。它包含用户名和散列密码的列表。这是这个装置的第一个特点。

[HeadlessZeke]本可以尝试[破解密码](http://www.hackaday.com/2011/06/01/gpu-password-cracking-made-easy/ "cracking passwords")，但他决定在这个兔子洞里走得更远。他从固件中取出源代码，查看了认证机制。系统检查用户名和密码，然后设置一个 cookie，让系统知道用户已经过身份验证。这听起来不错，但是经过进一步检查，发现 cookie 中的数据只是用户名的 MD5 散列。这听起来可能不错，但这意味着您要进行身份验证所要做的就是用您想要使用的任何用户的 MD5 散列手动创建您自己的 cookie。系统会看到这个 cookie，并假设您已经通过了身份验证。你甚至不需要密码！第二击。

现在[HeadlessZeke]已经登录到管理站点，他能够访问更多的功能。一个页面实际上允许用户从下拉框中选择一个命令，然后应用一个文本参数来执行该命令。然后，该命令在设备的外壳中运行。结果是文本参数根本没有被净化。这意味着[HeadlessZeke]可以将额外的命令添加到初始命令中，并运行他想要的任何 shell 命令。那是三振出局。三振出局！

[HeadlessZeke]向 Arris 报告了这些漏洞，它们现在已经在最新的固件版本中得到修补。不过，有些东西告诉我们，这个设备可能还有更多漏洞。

[via [Reddit](http://www.reddit.com/r/netsec/comments/2nenn4/att_uverse_vap2500_the_passwords_they_do_nothing/ "Reddit.com")