# 在 Hackaday 上开发:许可证不兼容和项目状态

> 原文：<https://hackaday.com/2014/05/13/developed-on-hackaday-license-incompatibilities-and-project-state/>

[![mooltipass top pcb](img/4bd742a700eeb5c0b9c33d6b60d059e2.png)](http://hackaday.com/wp-content/uploads/2014/05/top_pcb.png)

自从我们写了一篇关于我们正在进行的离线密码管理员项目(又称 Mooltipass)的文章已经有一段时间了。我们的上一篇文章是请我们亲爱的读者为他们最喜欢的[卡片艺术](http://hackaday.com/2014/04/21/developed-on-hackaday-vote-for-your-favorite-card-art/)投票，那么从那以后我们一直在做什么呢？

在过去的几周里，我们一直在改进现有的 PCB 和外壳设计，以使生产过程顺利进行。上面显示的最终顶部 PCB 已经过调整，以提高他的电容触摸感应能力，你甚至可以在 hackaday.io 上的 Mooltipass 项目日志[中看到系统运行的视频。我们还花了一些时间来完善两个最受欢迎的卡片艺术设计，以便我们的制造商可以正确地打印它们。我们将很快将更新的 USB 代码(允许 Mooltipass 被检测为复合 HID 键盘/ HID generic)集成到主解决方案中，这将允许我们在浏览器插件上工作。](http://hackaday.io/project/86-Mooltipass)

有趣的是，我们最近决定停止使用 GPL 许可的 avrcryptolib。我们目前的项目是 [CDDL 授权](http://en.wikipedia.org/wiki/Common_Development_and_Distribution_License)，允许感兴趣的各方在他们自己的项目中使用我们的代码，而不强迫他们发布他们创建的所有剩余代码。GPL 许可证执行相反的规定，因此我们选择了[另一个 AES 加密/解密实现](https://github.com/limpkin/mooltipass/blob/master/source_code/src/AES/aes.c)。这次迁移由我们的专职撰稿人[Miguel]执行和检查，因此他在不到一天的时间内运行了 AES [NESSIE](http://en.wikipedia.org/wiki/NESSIE) / CTR 测试并检查了它们的输出。

我们即将向我们的积极贡献者和顾问发送第一批 Mooltipass 原型。几周后，在我们展示(在 Hackaday 上)最终产品之后，我们将正式召集测试人员。不要犹豫，在评论区提出你的任何问题，你也可以通过专门的 [Mooltipass Google group](https://groups.google.com/forum/#!forum/mooltipass) 联系我们。