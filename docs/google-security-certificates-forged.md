# 伪造的谷歌安全证书

> 原文：<https://hackaday.com/2013/12/09/google-security-certificates-forged/>

最近，谷歌发现一个认证机构(CA) [为谷歌域名](http://googleonlinesecurity.blogspot.com/2013/12/further-improving-digital-certificate.html)颁发了伪造的证书。这损害了传输层安全性(TLS)和安全 HTTP (HTTPS)提供的信任，允许伪造证书的持有者执行[中间人](http://en.wikipedia.org/wiki/Man-in-the-middle_attack)攻击。

为了验证您正在访问的网站确实是他们所声称的那个网站，您的浏览器会确保您正在访问的服务器所提供的证书是由受信任的 CA 签名的。当有人向 CA 请求证书时，他们应该验证请求者的身份。您的浏览器和操作系统有一组最终受信任的 ca(称为根 ca)。如果证书是由他们之一或他们信任的中间 CA 颁发的，您将信任该连接。整个信任结构被称为[信任链](http://en.wikipedia.org/wiki/Chain_of_trust)。

有了伪造的证书，您可以说服客户您的服务器实际上是[http://www.google.com](http://www.google.com)。你可以用这个坐在一个客户端的连接和实际的谷歌服务器之间，窃听他们的会话。

在这种情况下，中间 CA 就是这样做的。这很可怕，因为它破坏了我们每天在互联网上安全交易所依赖的安全性。[证书锁定](https://www.owasp.org/index.php/Certificate_and_Public_Key_Pinning)是一种可以用来抵御这种攻击的工具。它通过将主机与特定证书相关联来工作。如果它发生变化，该连接将不被信任。

如果你不信任权威机构，TLS 的集中特性就不起作用。不幸的是，我们不能。