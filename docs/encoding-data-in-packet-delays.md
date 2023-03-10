# 在数据包延迟中编码数据

> 原文：<https://hackaday.com/2015/05/28/encoding-data-in-packet-delays/>

如果你曾经参加过“夺旗黑客大赛”( CTF ),你可能会看到一些[隐写术](http://en.wikipedia.org/wiki/Steganography)的挑战。隐写术是一种在众目睽睽之下隐藏数据的艺术。过去，包括仅在特定光线下可见的秘密墨水在内的工具已被用于此目的。现代隐写术挑战通常要求您找到隐藏在图像或文件中的“标志”。

[Anfractuosus]想出了一种在网络流量流中隐藏数据包的方法[。“时移器”将数据编码为数据包之间的延迟。根据延迟的长度，每个数据包被解释为 1 或 0。](https://www.anfractuosity.com/projects/timeshifter/)

为此，C 程序使用 [libnetfilter_queue](http://www.netfilter.org/projects/libnetfilter_queue/) 来访问数据包。用户使用 [iptables](http://en.wikipedia.org/wiki/Iptables) 设置网络规则，将流量转发给 Timeshifter 程序。然后用它来发送和接收数据。

提供了所有的代码，如果您曾经想在 Linux 上进行底层联网，这是一个很好的例子。如果你对隐写术感兴趣，或者对 CTFs 感兴趣，看看这个[伟大的资源](https://github.com/ctfs/resources/tree/master/topics/steganography)。