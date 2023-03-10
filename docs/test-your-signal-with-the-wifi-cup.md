# 用 WiFi 杯测试你的信号

> 原文：<https://hackaday.com/2014/11/11/test-your-signal-with-the-wifi-cup/>

[CNLohr]想测试他家的 WiFi 范围。看了一眼他室友的杯子，一个非正统的想法诞生了。[WiFi 杯](https://github.com/cnlohr/ws2812esp8266)用一个 ESP8266 连接到他的家庭网络。为了输出，[CNLohr]还在杯子上增加了一个 WS2812 LED 灯带。ESP8266 被编程为向[CNLohr 的]笔记本电脑发送 UDP 数据包。当笔记本电脑回应时，ESP8266 打开 led，照亮杯子。杯子对信号强度的反应非常快——大约一秒钟。

[CNLohr]拿着 WiFi 杯在家里转悠。他惊讶地发现在他没有预料到的角落里的联系；事实上，信号一点也没有减弱！他带着它走到外面，希望看到信号强度减弱。作为他室友强大路由器的证明，杯子只是闪烁了一下。为了进行更好的测试，[CNLohr]将路由器换成了更便宜、天线更短的 TP-Link。虽然最初的 ping 测试显示响应时间较慢，但 cup 检测到房子周围的 WiFi 没有问题。当它被放在一个金属桶里时，它只摇摆了一会儿。我们不得不怀疑[CNLohr 的]墙到底有多薄。我们家的 WiFi 从来没这么好用过！

[https://www.youtube.com/embed/3LiMAG4viWA?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/3LiMAG4viWA?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)