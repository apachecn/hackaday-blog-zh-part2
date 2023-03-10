# 简单的真空黑客

> 原文：<https://hackaday.com/2012/05/16/a-simpler-sous-vide-hack/>

![](img/e66a0501379b22f50ad3ce970d1fe0ba.png "sous-vide-with-simple-hardware")

这里是 Nerdkits 的一个真空项目的控制模块。[Humberto]和工作人员继续做好工作，将项目集中在一个目标上，然后解释实现目标所需的步骤。在这种情况下，他们希望打造自己的廉价储物电器，并且不需要用户处理电源电压。我们喜欢它，因为大部分零件可以在五金店和大盒子店里找到。

他从一个慢炖锅开始，[这是非常标准的](http://hackaday.com/2011/08/09/sous-vide-crock-pot-controller/)。接下来，他需要一种方法来切换设备的电源。他没有使用固态继电器，而是使用了标准的调光开关。它内置在一个双组电气盒中，控制着该盒中第二个位置的插座。现在，慢炖锅的电流受到调光器位置的限制。下一个任务是添加一个纸板框架，将伺服电机连接到调光器的旋钮上。

有了控制方案，Humberto 需要一个反馈传感器。他用收缩管覆盖 LM34 温度传感器，并密封两端，制成了自己的防水温度探头。在烹饪用水中只有一个探头是不太可靠的，所以他在慢炖锅的底座和陶瓷容器之间增加了第二个探头，以提高 PID 算法的性能。休息过后，他在视频中详细介绍了这一点。

[https://www.youtube.com/embed/16aLzIRHycw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/16aLzIRHycw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)