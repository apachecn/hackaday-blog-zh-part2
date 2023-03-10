# 深入探究 8085 处理器的寄存器是如何设计的

> 原文：<https://hackaday.com/2013/03/05/digging-deep-into-how-the-8085-processors-registers-were-designed/>

硬件设计爱好者看到这张图片应该已经垂涎三尺了。但是[Ken shir riff]关于[8085 处理器的寄存器是如何设计的](http://www.righto.com/2013/03/register-file-8085.html)的文章会让你进入硅逆向工程的天堂。他设法找到了设计者用来使寄存器访问尽可能高效的技巧，比如在它们的路径上通过 ALU 路由一些寄存器。

我们当然不是像上面看到的那样研究死亡的专家。幸运的是[Ken]在放大重要部分方面做得很好，然后通过将硅树脂图像表示为功能流程图来剖析它们是如何工作的。我们发现最有趣的部分之一是 WZ 临时登记册。这是一组程序员无法访问的内部寄存器。它们仅供芯片内部使用。它们充当多操作数函数的临时存储器，也保存少量指令(JMP、CALL、RST 等)的寄存器地址。).

如果你对这些芯片的图像是如何获得的更感兴趣，你应该在 Hackaday 上做一些搜索。就在上周[我们在一篇链接文章](http://hackaday.com/2013/02/28/hackaday-links-february-28th-2013/)中介绍了一个这样的项目。

[via [Reddit](http://www.reddit.com/r/ECE/comments/19l699/ken_shirriffs_blog_the_8085s_register_file/)