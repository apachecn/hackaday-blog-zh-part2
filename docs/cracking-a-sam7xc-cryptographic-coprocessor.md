# 破解 SAM7XC 密码协处理器

> 原文：<https://hackaday.com/2013/02/11/cracking-a-sam7xc-cryptographic-coprocessor/>

![attacking-RFID-crypto-coprocessor](img/26c7e432a71d6bc49999fbec8b2445c7.png)

【Adam Laurie】花时间[撕裂 Atmel 生产的 SAM7XC 芯片](http://oamajormal.blogspot.co.uk/2013/02/atmel-sam7xc-crypto-co-processor-key.html)的安全性。即使他没有发现一些明显的安全漏洞，阅读他的方法也是值得的。

该芯片用于安全 RFID 系统。芯片被添加到组合中，以完成使用加密时所需的繁重工作。[Adam]找了几个开源库进行测试。固件被锁得很紧，但他对 RAM 内容的探索产生了一个位的宝库。在研究了该芯片的样本代码后，他震惊地了解到它使用 RAM 来存储密钥。在他余下的旅程中，他不断地转储数据，筛选数据，直到找到“多样化万能钥匙”。那是个大人物，他可以解密任何使用过的标签。

2011 年 9 月，他向 Atmel 报告了他的发现。他们的回答是，他们没有办法保护 RAM 不被利用。[Adam]断言问题在于示例软件在设计时没有考虑到 RAM 的脆弱性。密钥永远不应该存储在那里，因为它很容易从正在运行的系统中被转储。