# 一个 8 节点的 Raspberry Pi 集群 Web 服务器能经受住黑客攻击吗？

> 原文：<https://hackaday.com/2013/11/05/can-an-8-node-raspberry-pi-cluster-web-server-survive-hackaday/>

许多人已经将他们的树莓 Pi 用作网络服务器。[Steve]然而，这是我们遇到的第一个[8 节点负载平衡的 pi 集群](http://raspberrywebserver.com/)服务器。[虽然我们在](http://hackaday.com/2013/05/21/33-node-beowulf-cluster-built-with-raspberry-pi/)之前已经看到过 pi 集群，但它们从未作为面向公众的 web 服务器投入使用。[Steve]已经创建了一个非常好的关于 Raspberry Pi 和 Linux 的信息网站。随着页面浏览量的增加，[他不得不在服务器上添加节点](http://raspberrywebserver.com/raspberrypicluster/adding-more-nodes-to-the-cluster.html)。目前[史蒂夫]每月有大约 45，000 的页面浏览量。

乍一看，负载平衡系统似乎是链条中的薄弱环节。然而，[史蒂夫]确实意识到，他需要的不仅仅是一个私家侦探来完成这项任务。他使用一台具有 512MB 内存和 2.7GHz x86 CPU 的旧 PC 构建了负载平衡器。关于平衡器最重要的是双网络接口，一边面向互联网，另一边面向 Pi 集群。不过，平衡器不是路由器。仅转发 HTTP 请求。Pi 节点本身存在于它们自己的子网中。史蒂夫已经运行了一些基本的围攻测试，但是没有什么能打败现实世界的测试。我们认为来自 Hackaday 的几个链接足以对系统进行酸性测试。