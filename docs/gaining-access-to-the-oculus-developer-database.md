# 进入 Oculus 开发者数据库

> 原文：<https://hackaday.com/2014/09/01/gaining-access-to-the-oculus-developer-database/>

Bitquark [的一名黑客在 Oculus 开发者门户](https://bitquark.co.uk/blog/2014/08/31/popping_a_shell_on_the_oculus_developer_portal)上打开了一个外壳，让他完全控制里面的特殊管理面板。如果他愿意的话，这允许他编辑用户、修改项目、添加新闻文章、编辑仪表板、上传 SDK 文件和各种其他好东西。

这个过程从使用一个名为 BSQLi 的 SQL 注入器测试参数、cookies 和头开始。注入头显示，Oculus 团队成员将 [X-Forwarded-For](https://en.wikipedia.org/wiki/X-Forwarded-For) 头直接插入数据库，没有适当的转义格式。这为他打开了大门，在 sqlmap 的帮助下，对数据库进行了枚举，并识别出了一个模式。存储在数据库中的 Oculus 密码被大量散列。但是，用户会话变量仍然不受保护。一个 SQL 查询被快速构建，最新的管理会话被迅速提取，然后信息被插入，从而允许访问门户。进一步的调查发现，AJAX eval()预览脚本没有受到一个 [CSRF 令牌](https://en.wikipedia.org/wiki/Cross-site_request_forgery)的保护，这个令牌很容易被恶意黑客利用。

这些发现后来变成了脸书，他为第一个漏洞和特权提升攻击支付了 15000 美元。随后，每发现一个管理账户接管漏洞，SQL 注入就会获得 5000 美元的奖励，这是这个家伙一周工作的丰厚回报。