# 廉价万用表测量嵌入式空闲时间

> 原文：<https://hackaday.com/2014/09/25/cheap-multimeter-gauges-embedded-idle-time/>

你的微控制器实际上多久做一次事情？你可以通过测量空闲时间来找出答案，但是你具体是怎么做的呢？[Jack Ganssle]表明，简单的嵌入式应用可以在空闲时触发一个引脚，然后对其进行测量。更复杂的应用程序，比如那些使用实时操作系统的应用程序，也可以通过使用 idle 钩子来完成同样的任务。但是，如何才能让这种切换引脚反馈真正有意义呢？

他的解决方案是[重新使用模拟万用表](http://www.ganssle.com/video/episode12-measuring-idle-time.html)。仪表与肘节销连接，trimpot 校准指针。这样，指针在处理器忙的时候跳，空闲的时候归零。这是一个很好的技巧，可以获得关于黑色塑料 ic 封装内部情况的更多反馈。从 Hackaday 奖评委之一的[那里找到这样一个聪明的黑客并不奇怪。](http://hackaday.io/prize/judges#Ganssle)

当你在模拟万用表的过道上时，你可能想为[多选择几个额外的数据显示](http://hackaday.com/2010/06/24/multi-multimeter-clock/)。

[https://www.youtube.com/embed/f8KGatsPTNo?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/f8KGatsPTNo?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)