# 在 Hackaday 上开发的:来造点硬件吧！

> 原文：<https://hackaday.com/2013/12/06/developed-on-hackaday-lets-build-some-hardware/>

我们很确定你们大多数人已经知道几个月前 Hackaday 被 SupplyFrame 收购了，他因此成为了我们新的邪恶霸主。我们真的希望你已经注意到他们实际上很好，出于他们神圣的善良，他们最近批准了在 Hackaday 上开发的这个名为*的系列。*

一个新的项目将由 Hackaday 员工和社区完成，并有望进入消费者市场。对于那些没有时间/经验参与这一冒险的人，我们希望展示和记录将一个想法带到可销售产品阶段所需要的东西。对于其他人，我们希望您尽可能多地参与设计/开发过程。显然，这个项目将是开源的硬件/软件。这一次，硬件将主要由你们真正开发。你可能已经从[口哨平台](http://hackaday.com/2013/05/18/just-put-your-lips-together-to-turn-on-a-lamp/)(目前在 Tindie 上出售)或者从[我的网站](http://www.limpkin.fr)上描述的所有不同项目中认识了我，这使得这次新的冒险远不是我的第一次竞技。

对贡献者有什么好处？在这个项目的所有步骤中，我们将提供许多奖励以及手工焊接设备的第一个原型，以便您可以开始玩/测试它。没有什么是一成不变的，所以每个建议都是受欢迎的。如果我们要像 Kickstarter 一样发起一场运动来制造最终产品，我们只会在我们的原型最终成型、我们的合作伙伴被选定、生产流程的所有细节都已确定并得到确认的情况下才会这么做。在这种情况下，我们只需要收集所需的资金，使设备成为现实。我们要建造什么？请继续阅读，寻找答案。

那么这个新设备怎么样呢？经过与作者的多次讨论，我们决定为黑客读者做些有用的东西。我们想要一些简单的东西来简化用户的生活，因此选定了一个安全的离线密码管理器。请记住，下面的描述只是一个草稿，所以欢迎您在评论部分提出意见。请保持建设性，因为评论的格式对于这种讨论来说不是最佳的(我们目前正在努力)。

该产品背后的概念是最大限度地减少密码泄露的方式，同时为您日常使用的不同网站生成长而复杂的随机密码。顺便说一句，你可能已经知道大多数人通常不使用安全密码，除了 T2 红发女人 T3。假设，通过读取计算机 RAM 上的密钥+加密密码，可以绕过密码保存软件。理想情况下，产品应该非常简单，我的祖母可以使用它(我会让你想象她的电子邮件密码……)。它会尽可能的小，这样就可以放进你的口袋里。只需访问一个网站，当您需要登录时，设备会要求您确认输入您的凭据。

硬件呢？我们认为一个好的解决方案是让成为一个使用智能卡的设备，通过 USB 连接到你的电脑(以保持低成本)。该设备将存储您的 AES-256 加密密码，智能卡将保存您的 AES-256 密钥(以及其他一些密码)。智能卡将是(为简单起见)一个读保护的 EEPROM，需要 PIN 码来解锁其内容。与您的信用卡一样，尝试次数过多会永久锁定智能卡。因此，该项目的主要组件将是:一个智能卡连接器，一个微控制器(兼容 Arduino？)，一个有机发光二极管屏幕及其触摸屏面板。有机发光二极管屏幕将提供良好的对比度，因此能见度更好。在软件方面，我们“只”需要写一个简单的脚本在用户的浏览器上运行。浏览器脚本会将当前网站 URL 发送到设备(通过 HID 报告)。

出于几个原因，我们更喜欢基于接触的智能卡。它们更容易获得，更便宜，而且不易被察觉。我们希望这是一个开放的项目，将确保任何未来的问题得到处理。我们还希望这款设备尽可能具有可攻击性，一款兼容 Arduino、带有触摸感应有机发光二极管屏幕和 USB 连接的设备肯定会引起初学者的兴趣。

那么下一步是什么？我们需要一个项目名称，所以请在评论区给我们一些反馈。你也可以直接联系我:mathieu[at]hackaday[dot]com，如果你想投稿(我们需要设计师、编码员、网站管理员……)，成为测试团队的一员，或者你已经知道这个项目的潜在合作伙伴。我们期待您的评论！

[ [智能卡图像源](http://commons.wikimedia.org/wiki/File:Differentsmartcardpadlayouts.jpg)–[CC-BY-SA](http://creativecommons.org/licenses/by-sa/3.0/deed.en)