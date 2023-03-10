# 邮递员到达时的邮箱通知文本

> 原文：<https://hackaday.com/2013/03/13/mailbox-notifier-texts-when-the-letter-carrier-arrives/>

![mailbox-notifier](img/c948f5ebaf24117ca8bb2e52f54fe636.png)

(菲利克斯·鲁苏的)邮箱在街的另一边，他有一个相当大的前院。这意味着检查邮件不仅仅是一种把头伸出门外的活动。这在冬天变得尤其明显，那时他必须穿得严严实实，在雪地里跋涉，看看他的邮递员是否已经到了。但是他通过建立一个为他监控邮箱的通知程序，让无意义的旅行成为过去。

他用的是 Moteino，这是他自己制作的 Arduino 克隆体。它很小，在电路板的底部有一个射频模块，负责与房屋内的基站通信。上面看到的模块将微控制器板与 9V 电池和霍尔效应传感器一起卷起，霍尔效应传感器可以判断邮箱门是开着还是关着。当 Arduino 检测到传感器的变化时，它会将一些数据推回基站，然后基站将这些信息转发给计算机或 Raspberry Pi，以便给他发送短信。所有这些都在休息后的视频中展示出来。

[https://www.youtube.com/embed/uh2-1NP3aR0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/uh2-1NP3aR0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)