# 更新:麦克的自我闪光钻机

> 原文：<https://hackaday.com/2013/09/17/update-mchcks-self-flashing-rig/>

[![](img/d91bbb5f880dad952b9c505fd23ac1b3.png)](http://hackaday.com/wp-content/uploads/2013/09/9729390425_2649ff8c0f_h.jpg)

几周前，我们特别介绍了 McHck 项目(发音为 McHack)，这是一个基于 Cortex M4 的 5 美元平台，可以直接插入个人电脑。最近，[西蒙]宣布他制作了一个固件，允许一个 mch CK[像一个 SWD 适配器](https://mchck.org/blog/2013-08-13-self_hosted_toolchain_the_mc_hck_as_swd_adapter/)一样工作，并且还详细介绍了他的[闪存装备](https://mchck.org/blog/2013-09-12-mc_hck_flashing_rig/)。

因此，那些想要构建自己的 McHck 的人只需要借用一次 SWD 程序员就可以开始了。当第一个平台已经用 SWD 固件编程时，它可以用来在第二个 McHck 上刷新和调试应用程序。因此，微控制器 flash rig[Simon]设计(如上图所示)就是基于此。几个核心元件是一个 TQFP48 ZIF 编程插座，一个按钮和两个 led。只需将 Kinetis 推入编程插座，关闭并按下按钮。两个 led 表示操作成功。【西蒙】用 [Ragel 状态机编译器](http://www.complang.org/ragel/)生成他的 flashing 程序，他做的所有代码都可以从他的 [github](https://github.com/mchck/mchck) 下载。

如果你错过了最初的 McHck 帖子,现在你有机会回去看看到底是怎么回事。