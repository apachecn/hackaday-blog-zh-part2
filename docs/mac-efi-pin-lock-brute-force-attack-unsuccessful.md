# Mac EFI PIN 锁暴力攻击(不成功)

> 原文：<https://hackaday.com/2013/02/26/mac-efi-pin-lock-brute-force-attack-unsuccessful/>

[Oliver]在另一台机器上使用“dd”命令擦除 Macbook Pro 的硬盘。这做了一个伟大的工作，让一切从驱动器上，但他仍然面临着 EFI PIN 锁保护，当他试图把它放回 Mac。您过去可以清除 NVRAM 来绕过这个问题，但是这个漏洞现在已经被修补了。所以[Oliver]开始使用微控制器强行破解 EFI 引脚。

你可以通过上面的链接阅读他的背景故事。在格式化之前，他有机会输入一个 4 位数的 pin。现在他已经清除了硬盘，密码至少有 6 个字符长，这就有更多的可能性了(至少只有数字字符！).为了使这个过程自动化，他设计了这个小小的板来尝试每一种可能的组合。它在文本编辑器上工作得很好，但有时字符或 enter 命令不会注册。他猜测这是某种针对自动攻击者的保护措施。为了解决这个问题，他在按键之间和输入每个代码之间增加了不同的延迟。这解决了这个问题，你可以在休息后的视频中看到。不幸的是，经过两次 48 小时的运行，尝试了每一个代码，他仍然没有获得访问权！

[https://www.youtube.com/embed/xXMiX-Bybsw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/xXMiX-Bybsw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)