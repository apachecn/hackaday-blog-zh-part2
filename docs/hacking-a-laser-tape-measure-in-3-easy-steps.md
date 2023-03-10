# 通过三个简单的步骤破解激光卷尺

> 原文：<https://hackaday.com/2014/03/29/hacking-a-laser-tape-measure-in-3-easy-steps/>

![uni-t-laser-distance](img/1d8003c1f85cffcd311aa16b34b9143b.png)

[Andrew]在朋友的帮助下黑了一个激光测距仪。使用激光测距仪作为传感器是黑客的一大追求——理由很充分。精确的距离读数对于包括机器人、打印机和制造业在内的应用来说是无价的。我们已经看到有人[在](http://hackaday.com/2013/09/26/fail-of-the-week-capturing-data-from-a-laser-rangefinder/)之前尝试破解类似的单元，但失败了，而其他人[则从零开始建造自己的单元](http://hackaday.com/2014/02/28/homebrew-phase-laser-rangefinder/)。[Andrew]开始试验 UNI-T 390B，这是一种来自中国的相对便宜的设备(60 美元)。他发现 390B 有一个串行端口，可以通过电池盒访问。更好的是，串行端口仍然启用并输出距离数据。虽然可以读取数据，但[Andrew]无法命令 390B 开始测量。唯一的选择似乎是使用 Arduino 来模拟 390B 前面板上的按钮按压。

在他最初的博客的[更新中，他描述了一个 Arduino 草图，可以解码距离测量。这时[洞穴狂人]发现 Uni-T 会响应“*xxxxx#”形式的命令。有了这些信息，【安德鲁】](http://blog.qartis.com/parsing-laser-distance-meter-serial-output/)[发布了第二个更新](http://blog.qartis.com/laser-distance-meter-update-serial-commands-timing-measurements/)，给出了基本的命令分解。命令*00004#将进行单次测量，并通过串行输出数据。命令*00002#将进行 3 次测量，并以 C 风格的数组格式输出。还有其他几个命令输出调试信息和存储的测量转储。虽然他没有探究数据输出的每个细微差别，但[Andrew]现在已经有足够的信息来启动测量并读取结果。干得好！

【谢谢詹姆斯！]