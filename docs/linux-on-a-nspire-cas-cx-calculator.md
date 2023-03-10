# Nspire CAS CX 计算器上的 Linux

> 原文：<https://hackaday.com/2012/11/12/linux-on-a-nspire-cas-cx-calculator/>

[![](img/f8b77d4dd8cc9b8bf5292bb4afb93c05.png "Linux on Nspire CAS CX")](http://hackaday.com/2012/11/12/linux-on-a-nspire-cas-cx-calculator/ti-linux/)

很高兴看到 Linux 以一种从未想过的方式在一台设备上运行。[tangers]已经在基于 ARM 的 Nspire CAS CX 图形计算器上成功运行了一个 [Linux 内核。他开发了一个就地引导加载程序，允许从普通的 Nspire 操作系统中加载内核。它还允许偷看和戳内存进行调试。](http://www.omnimaga.org/index.php?topic=14534.0 "Linux on Nspire CAS CX")

[tangers]还设法让 USB 主机模式在计算器上工作。这允许连接 USB 键盘和 Wifi 加密狗。此时，计算器可以[连接到互联网](http://www.omnimaga.org/index.php?topic=14762.0 "Internet on Nspire CAS CX")并使用基于文本的浏览器进行浏览:链接。计算器运行 SSH 服务器进行远程访问，图形浏览正在进行中。

看起来这个计算器正在成为手持 Linux 设备。内核和引导加载程序的所有源代码都可以在[tangrs]的[Github](https://github.com/tangrs/ "[tangrs]'s Github")和他的[博客](http://blog.tangrs.id.au/ "tangrs")上获得。休息之后，看看使用全键盘进行文本浏览的视频。

[https://www.youtube.com/embed/hET3g3CWLlg?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/hET3g3CWLlg?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)