# 设计我的第二版名片

> 原文：<https://hackaday.com/2014/06/17/designing-the-second-version-of-my-business-card/>

这个月底，我和现在雇主的合同(不，不是黑客日)将会结束。随着面试开始排队，我因此认为这将是一个很好的机会来设计你可以在上图中看到的 [PCB 名片](http://www.limpkin.fr/index.php?post/2014/06/16/My-business-card-v2)。

它是由两个 PCB 焊接在一起，底部的一个包含 SMD 元件，而顶部的一个只有孔，让大部分通过。该设计主要受我们已经在 Hackaday 上展示的第一个版本的启发，尽管微控制器被更改为(昂贵的)ATMega32u4，并且顶部 PCB 被轻微打磨，以便 led 可以透过 FR4 发光。led 以 2 个为一组(总共 8 组)连接到 PWM 通道，隐藏的闪存允许使用 LUFA 库将卡识别为外部 2MB 存储。所有源文件都可以在我的网站上下载。