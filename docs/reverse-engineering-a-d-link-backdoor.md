# 逆向工程 D-Link 后门

> 原文：<https://hackaday.com/2013/10/14/reverse-engineering-a-d-link-backdoor/>

这里有一个真正的黑客 ( [谷歌缓存链接](http://webcache.googleusercontent.com/search?q=cache:http://www.devttys0.com/2013/10/reverse-engineering-a-d-link-backdoor/))给我们亲爱的黑客读者。在一个周六的晚上，由于[Craig]没有其他事情可做，他决定下载一台旧的 D-Link DIR-100 路由器的固件(因为谁不会呢？).他的目标是看看他能在里面找到什么有趣的东西。他启动 [binwalk](https://code.google.com/p/binwalk/) 来提取 SquashFS 文件系统，然后在多处理器反汇编器/调试器 [IDA](https://www.hex-rays.com/products/ida/index.shtml) 上打开路由器 web 服务器。[Craig]发现 web 服务器实际上是 thttpd 的修改版本，为路由器提供管理接口。正如你在上面的图片中看到的，似乎是 alpha networks(D-Link 的一个分支)进行了修改。

对 Craig 来说幸运的是，Alphanetworks 的人很善良，在他们的许多自定义函数名前加上了字符串“alpha”。查看 http 标识函数的反汇编，可以发现固件上实施了后门。如果一个恶意用户将字符串“xmlset _**roodkcab**leoj 28840 Yb tide”作为他的浏览器用户代理，则不需要认证就可以访问路由器。reddit 帖子上[的一条评论指出，读取该字符串会导致:“由(04882) joel backdoor 编辑”。](http://www.reddit.com/r/programming/comments/1ocghn/reverse_engineering_a_dlink_backdoor_lots_of/)