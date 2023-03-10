# 入侵 KVM:教键盘开关监视

> 原文：<https://hackaday.com/2015/08/08/hacking-a-kvm-teach-a-keyboard-switch-to-spy/>

说到大型系统，计算机的数量远远超过维护它们的人数。这没什么大不了的，因为您可以简单地使用 KVM 将一个键盘/视频/鼠标终端连接到所有这些终端，在每个盒子之间简单无缝地切换。副作用是，现在 KVM 可以像轻抚键盘的人一样访问所有这些系统。[Yaniv Balmas]和[Lior Oppenheim]花了一些时间对其中一个设备的固件进行逆向工程，并展示了可疑的固件如何能够 pwn 这些系统，即使有些系统本身与互联网没有任何联系。这是他们第一次 DEF CON 演讲，他们很好地解释了如何破解这些设备。

## 历史

KVM 的起步非常简单，但他们并没有就此止步。在 20 世纪 90 年代早期，你可以得到一个 4 端口 KVM，它比 AV 风格的开关好不了多少。键盘向 USB 的转变带来了 KVM 硬件的大升级。2000 年，具有 16 端口和完整 USB 堆栈的交换机出现了。十年后，你可以找到支持 1024 台或更多机器的矩阵 KVM。这些与早期的交换机相去甚远，它们是成熟的计算机，旨在简化对装满机器的服务器机架的访问。

## 查找固件

![DSC_0422](img/c8a990f82bc177559985d48f8e2b8be4.png)关键是固件，拥有它，你就拥有了设备。在这次演讲中展示的设备的未公开制造商非常好，在包含固件更新实用程序和`firmware.bin`文件的盒子中包含了一张 CD。固件实用程序将这个二进制文件解包并存储在内存中，这样可以很容易地访问它。

不幸的是，通过 Binwalk 运行倾倒的 blob 对研究人员没有任何帮助。64 千字节的数据不包含一个字符串和零可用的结果，这显然是混淆。下一个测试是嗅探通过设备附带的更新电缆传输的数据。除了正常的串行开销和纠错之外，通过电缆传输的内容与 blob 完全相同。他们需要找到破解密码的方法。

## 解码固件

[![](img/5181ef90e3e1b313c0bceca0b29a19dd.png)](https://hackaday.com/wp-content/uploads/2015/08/dsc_0429.jpg) 在查看 KVM 的电路板时，破解固件 blob 的真正关键出现了。有两个大芯片，上面印有设备制造商的名称；可能是 ASICs。此外，还有一个 8052 处理器和一个外部 RAM 芯片。通过 8051 组件(是的，这是一个 8052，但组件与' 51 变体相同)的镜头来看固件是什么为他们做了。

它没有立即找到任何线索，但查看固件的最后八个字节，一种模式开始出现。匹配在固件的几个变体中发现的频繁使用的值，研究人员开始将其作为固件版本的标识符。这些是基本的数值，但是代表每个数字的四位隐藏在每个字节中，占据了位置[6..3].通过将字节向右旋转三次，每个字节都变成一个数字的 ASCII 值，这些值与固件的版本号对齐。

他们快到了。看着这些字符串，他们发现了一个字母表，但是顺序错了。进一步的研究表明，这些字母被分成三组，每组都以同样的方式洗牌。这个字符串是解开其余二进制文件的关键。找到了，废弃的代码！移动固件的所有字节使 Binwalk 能够解析文件，并产生字符串、函数和阅读程序所需的一切。

## 展示漏洞

当然，读取固件只是第一步，你需要展示一些有用的(阴险的)东西可以用它来完成。在谈话中，两人演示了他们的定制固件切换到不同的系统，“键入”密码(当人类键入密码时，密码会被记录)，并回显一个二进制文件，然后执行该文件以将恶意软件加载到系统中。

是的，您需要实际接触到通话中使用的 KVM 来执行此攻击。但是一些 KVM 允许通过 IP 进行固件更新，并且其中许多都有用于配置的 web 界面。这里有许多可用的媒介，知道了这一点，讨论就转向预防。击键统计是防止这种攻击的一种方法。通过记录字符输入的速度、节奏的紧密程度以及退格键的使用等其他人类特征，可以大大降低这种攻击的有效性。

 [![DSC_0412](img/9f7df81719be5de29a1eed632b921417.png "DSC_0412")](https://hackaday.com/2015/08/08/hacking-a-kvm-teach-a-keyboard-switch-to-spy/dsc_0412/)  [![DSC_0417](img/97f58b9c4f86120c62d5c9beb18bde9f.png "DSC_0417")](https://hackaday.com/2015/08/08/hacking-a-kvm-teach-a-keyboard-switch-to-spy/dsc_0417/)  [![DSC_0418](img/539cef15b5cd8656156cf45d73b35341.png "DSC_0418")](https://hackaday.com/2015/08/08/hacking-a-kvm-teach-a-keyboard-switch-to-spy/dsc_0418/)  [![DSC_0419](img/a07ae8b56aafbe6e38645bc155b5de92.png "DSC_0419")](https://hackaday.com/2015/08/08/hacking-a-kvm-teach-a-keyboard-switch-to-spy/dsc_0419/)  [![DSC_0422](img/5942131a4ff092c35016ac5bb3b29b00.png "DSC_0422")](https://hackaday.com/2015/08/08/hacking-a-kvm-teach-a-keyboard-switch-to-spy/dsc_0422/)  [![DSC_0420](img/e7e26aad230d010f8b3db0e55bf9e4c4.png "DSC_0420")](https://hackaday.com/2015/08/08/hacking-a-kvm-teach-a-keyboard-switch-to-spy/dsc_0420/)  [![DSC_0428](img/dff637cdc14bb54183918c392d23d183.png "DSC_0428")](https://hackaday.com/2015/08/08/hacking-a-kvm-teach-a-keyboard-switch-to-spy/dsc_0428/)  [![DSC_0430](img/47bc802f67d8eacdc480c8a4b5064e48.png "DSC_0430")](https://hackaday.com/2015/08/08/hacking-a-kvm-teach-a-keyboard-switch-to-spy/dsc_0430/)