# 破解 D-Link DSP-W215 智能插头

> 原文：<https://hackaday.com/2014/05/17/hacking-the-d-link-dsp-w215-smart-plug/>

[![DSP-W215](img/faacc3a2dac01ace7af5f959f7f9c914.png)](http://hackaday.com/wp-content/uploads/2014/05/dspw215.jpg)

D-Link DSP-W215 智能插头，一种用于监测和控制电源插座的无线家庭自动化设备[刚刚被黑客攻击](http://www.devttys0.com/2014/05/hacking-the-d-link-dsp-w215-smart-plug/)。尽管还不能从亚马逊或百思买买到，但 D-Link 的网站上已经有了固件。这篇非常详细的文章解释了导致该漏洞产生的所有步骤。

首先，打开固件，检查文件系统内容。人们发现，智能插头没有正常的基于网络的界面，因为用户需要使用 D-Link 的 Android/iOS 应用程序来配置它。然而，这些应用程序似乎使用家庭网络管理协议(HNAP)来与运行 lighthttpd 服务器的智能插件对话。查看后者的配置文件可以发现，这些函数无需任何身份验证就可以调用。另一个发现，固件可以接受无限量的 POST 请求字节，这些字节在固定长度的缓冲区中复制，而不进行任何检查。我们将让我们的读者前往原始文章，看看作者从这一点去了哪里。