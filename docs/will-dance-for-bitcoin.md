# 会为比特币起舞

> 原文：<https://hackaday.com/2013/12/07/will-dance-for-bitcoin/>

现在的新闻似乎都是比特币，但[比特币机器人](http://sync.heatsynclabs.org/special/bitcoin_bot.html "Bitcoin Bot")可能是第一个会为比特币跳舞的机器人。

亚利桑那州梅萨市的 HeatSync 实验室(HeatSync Labs)的[Ryan]是加密货币的粉丝，他决定开发一些东西来接受加密货币。他发现比特币基地，一个流行的托管比特币钱包服务，有一个[回调 API](https://coinbase.com/docs/merchant_tools/callbacks "Coinbase Callback API") 。这使得比特币基地在钱包收到交易时获取指定的 URL，并在请求中提供交易信息。Python 脚本处理这些请求，并更新发送到机器人钱包的 BTC 余额的运行计数。

在硬件方面，带有以太网屏蔽的 Arduino 检查平衡。如果它已经改变了，它调用舞蹈函数和 luau 女孩跳舞。

该机器人位于黑客空间的窗口，因此任何路过的人都可以阅读比特币并进行捐赠。源代码在 [Github](https://github.com/blhack/hsl_bitcoin "Bitcoin Bot on Github") 上，休息之后是一段视频。

[https://www.youtube.com/embed/eAdKmcUyp9s?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/eAdKmcUyp9s?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)