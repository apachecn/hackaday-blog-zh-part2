# 缓慢驱动无刷 DC 电机

> 原文：<https://hackaday.com/2015/04/20/driving-a-brushless-dc-motor-sloooooooowly/>

驱动无刷 DC(万向节)电机可能是一个痛苦的晶体管。[Ignas]写了一篇很好的文章,不仅解释了如何用 Arduino 做到这一点，还解释了这个过程是如何工作的。他使用了一个 [L6234](http://www.st.com/web/catalog/sense_power/FM142/CL851/SC1791/SS1157/LN1720/PF63243) 三相电机驱动器，但他指出还有其他方法来连接 BLDC 电机和 Arduino。

警告是必要的——这不适合胆小的人。如果不小心的话，你很容易毁坏你的微控制器。【Ignas】按照[应用笔记](http://www.st.com/st-web-ui/static/active/jp/resource/technical/document/application_note/CD00004062.pdf) (PDF 警告)中的建议，增加了几个限流电阻和电容，以确保安全。

高速运转时一切正常，但在低速运转时，发动机运转不稳定。[Ingus]通过改用正弦波驱动电机解决了这个谜题。他没有让 Arduino 计算波浪，而是使用了一个查找表。

请务必查看他的博客，获取完整的源代码和原理图。还有一个视频演示了他能让下面的马达移动得多慢。

[https://www.youtube.com/embed/667XSSxieXM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/667XSSxieXM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)