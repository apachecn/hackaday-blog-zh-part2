# 不到 40 美元的黑板数字化

> 原文：<https://hackaday.com/2015/02/17/blackboard-digitization-for-under-40/>

数字白/黑板或“智能板”在现代教室中非常有用，但其高昂的成本往往很难说服管理员放松他们的钱包。Cooper Union 在纽约举办的第二届年度 HackCooper 活动希望学生设计和构建既能解决实际问题又能激发想象力的硬件和软件项目。在 24 小时黑客马拉松上，[harrison]、[david]和[caleb]的团队决定将[一个低成本、简单的解决方案整合到一起，以数字化课堂黑板内容](https://www.hackerleague.org/hackathons/hackcooper-2015/hacks/string2string)。

粉笔夹系在两根绳子上，每根绳子通过滑轮与重物相连。重物在黑板两侧的 PVC 管内滑动。每个试管底部的超声波传感器测量到砝码的距离。重物处于静态平衡，所以它们的作用是保持琴弦绷紧，而不会对书写者产生负面影响。

通过几个校准点来测量每个砝码的位移程度，可以确定板材宽度，从而轻松适应不同尺寸的板材。一旦被校准，系统就可以根据一些三角计算来确定粉笔在黑板上的位置。由于他们只有 24 小时的时间一起破解系统，他们不得不使用一个带有几个按钮的手动无线电来提供用户控制。按下“写入”按钮开始将粉笔运动传输到数字屏幕。无线电遥控器上的第二个按钮用于“擦除”数字屏幕。在收到粉笔位置数据后，他们必须做大量的处理，以消除噪音并平滑数字屏幕上的书写。

服务器允许全班实时接收黑板数据。在每次“擦除”命令后，粉笔板状态被保存并记录在服务器上，从而允许查看或下载以前的内容。如果只书写文本，可以使用光学字符识别来进一步数字化内容。

这个项目真正有用的地方是成本低。传感器的价格是一美元。其他部件——PVC 管、重物/滑轮、Arduino 和无线电遥控钥匙——都是以不到 40 美元的价格购买的。如果多花一些钱(对他们来说可能需要更多的时间)，他们可以自动检测粉笔何时真正在写字。团队在 Github 上发布了他们的[代码。对于成本谱另一端的粉笔板，](https://github.com/harrisonzhao/string2string)[看看这个](http://hackaday.com/2013/11/22/building-a-crystal-clear-whiteboard/)。下面视频。

[https://www.youtube.com/embed/y1aw0IiamFM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/y1aw0IiamFM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[via [Reddit](https://www.reddit.com/r/somethingimade/comments/2w4ab1/digitally_encoding_a_chalkboard_with_strings/)