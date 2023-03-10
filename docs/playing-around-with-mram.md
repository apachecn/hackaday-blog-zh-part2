# 和 MRAM 一起玩耍

> 原文：<https://hackaday.com/2012/10/10/playing-around-with-mram/>

![](img/63b8d31e089f0fe0d1ac4e1c35395a05.png "MRAM")

很长一段时间以来，硬件修补者只能摆弄两种类型的内存。RAM，包括静态 RAM 和动态 RAM，速度非常快，但是易失性，断电时会丢失数据。EPROMS、EEPROMS 和 Flash 存储器等非易失性存储器在断电后仍保持其状态，但这些格式稍慢。

总有一些相互竞争的技术试图结合这些类型记忆的最佳特性，但爱好者并不经常能得到它们。[Majenko]得到了一些 MRAM 芯片——磁阻 RAM—[,决定看看它们能做些什么。](http://digital-diy.com/general-blog/511-mram-joy.html)

磁阻 RAM 使用微小的磁板对来读写 1 和 0。[Majenko]收到了一个带有 SPI 总线的四个 MRAM 芯片的样品(它可能是[这个芯片](http://au.mouser.com/ProductDetail/Everspin-Technologies/MR25H40CDC/?qs=sGAEpiMZZMvaNBfR%2fsmQGz8qy96p9VdiyOb3yG94yeE%3d)，4 兆位，售价 20 美元，尽管更小容量的芯片[也有售](http://www.digikey.com/product-detail/en/MR25H256CDC/819-1015-ND/2504973?WT.z_cid=ref_octopart_dkc_buynow&cur=USD)，售价约为 6 美元)。在将这些芯片连接到自制的分线板上后，[Majenko]拥有了 16 兆的非易失性存储器，能够以 40 MHz 的速度运行。

结果正如数据手册所说:读写速度非常快，并且能够切断电源。不像 EEPROMS 会被反复读写破坏，MRAM 有无限的写周期。

虽然 MRAM 现在可能是一项非常年轻的技术，但它是未来事物的美好预兆。在 20 年(或 30 年，或 40 年)内，任何计算机，从最大的服务器到最小的微控制器，都很难实现磁盘空间和内存的人工分离。今天，任何硬件黑客都能够使用这项技术，这一事实有些令人惊讶，我们期待将来有更多的版本使用 MRAM。