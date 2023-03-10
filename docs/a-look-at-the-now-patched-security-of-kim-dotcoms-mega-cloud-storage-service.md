# 看看(金·多特康姆的)大型云存储服务的安全性(现在已经打了补丁)

> 原文：<https://hackaday.com/2013/01/29/a-look-at-the-now-patched-security-of-kim-dotcoms-mega-cloud-storage-service/>

![mega-cloud-storage-security](img/957a5839ed42155a12054bc9ccc68c1b.png)

MEGA 是一个新的加密云存储系统，由 MegaUpload fame 的[金·多特康姆]创建。他们在出售隐私，因为该公司没有办法解密其服务用户存储的数据。与任何软件项目一样，他们的开发人员正在快速改进用户界面和安全基础。但是，当我们对可能的安全问题有所了解时，这很有趣。听起来[Marcan]写的问题已经解决了，但是我们仍然很开心地阅读了他的文章。

本文主要关注网站使用一些 JavaScript 来验证从非 SSL 来源获取的数据的散列。这些不安全的来源是 CDN，因此这种类型的验证是必要的，以确保第三方网络没有作为对大型网站的攻击的一部分而受到损害。当使用 [CBC-MAC](http://en.wikipedia.org/wiki/CBC-MAC) 生成散列时，出现了特殊的安全问题。[Marcan]断言该协议不适用于其应用程序，并继续发布了一个概念证明，说明如何在保留验证真实性的哈希的同时伪造消息。

[谢谢基督教]