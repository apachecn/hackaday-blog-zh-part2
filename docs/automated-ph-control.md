# 自动化 PH 控制

> 原文：<https://hackaday.com/2013/02/23/automated-ph-control/>

[![pH Controller](img/06344919deb2ddf2419ab07f37e3431d.png)](http://hackaday.com/2013/02/23/automated-ph-control/phcontrol/)

控制溶液的 pH 值通常是一项繁琐的任务。向溶液中添加酸或碱会改变 pH 值，但手动监控水平并添加正确的量并不好玩。[Reza]安装了一个自动 pH 控制器来保持溶液的 pH 值稳定。

这个建筑使用了一个 Arduino，它带有一个 LCD 屏蔽、螺丝端子屏蔽和[Reza]自己的 pH 屏蔽。[蠕动泵](http://en.wikipedia.org/wiki/Peristaltic_pump "Peristaltic Pump")用于将 pH 值降低的酸泵入溶液。这种类型的泵将流体与泵部件隔离，防止溶液污染。该泵由电源开关尾部控制，允许 Arduino 控制液体的流量。

Omega pH 探针用于读取 pH 值。[Reza]的开源固件支持校准探头，以确保读数准确。设置完成后，屏幕会显示 pH 值和系统的当前状态。当 pH 值超出所需范围时，泵将启用。

休息之后，请观看设备的视频演示。

[https://www.youtube.com/embed/Y9XbZL0CMaY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/Y9XbZL0CMaY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)