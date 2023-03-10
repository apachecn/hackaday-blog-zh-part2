# 构建网状网络会议徽章

> 原文：<https://hackaday.com/2014/04/16/building-a-mesh-networked-conference-badge/>

[![](img/527151c84652b25d044029b5672240b9.png)](http://hackaday.com/wp-content/uploads/2014/04/conf.png)

[Andrew]刚刚完成他的文章，描述了他为一个自由的南非安全会议制作的电子会议徽章( [part1](http://andrewmohawk.com/2014/01/18/zacon-v-badge-12-build-time/) ， [part2](http://andrewmohawk.com/2014/04/14/zacon-v-badge-22-how-they-work/) )。上面显示的终端平台基于 ATMega328、诺基亚 5110 LCD、433MHz AM/OOK TX/RX 模块、几个 led 和按钮。

徽章形成网状网络来发送信息。这允许跟踪不同与会者之间的对话。最终成本是这次冒险中的主要制约因素，这也是为什么选择从易贝和阿里巴巴购买这些特殊组件的原因。

第一个 PCB 原型是 CNC 铣削的。PCB 铣削完成后，还有大量的焊接工作要做。幸运的是，安德鲁的朋友们加入了焊接 77 块最后的电路板。他还在记录他建立的协议方面做得很好，这是使用~~开源~~工具 [Maltego](https://www.paterva.com/web6/products/maltego.php) 验证的。点击休息时间，观看系统运行的两个视频。

[https://www.youtube.com/embed/5M51PI5m3-0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/5M51PI5m3-0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[https://www.youtube.com/embed/frp9m3uGWAA?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/frp9m3uGWAA?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)