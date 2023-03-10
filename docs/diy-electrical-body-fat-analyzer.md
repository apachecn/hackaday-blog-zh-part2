# DIY 电子体脂分析仪

> 原文：<https://hackaday.com/2015/01/10/diy-electrical-body-fat-analyzer/>

无论你是想减掉一些脂肪还是增加一些肌肉，追踪进展都是很重要的。追踪你的体重很容易，但是体重并不能说明全部。你可能在燃烧脂肪的同时也在锻炼肌肉，这会让你看起来好像根本没有减肥。一个更有用的数字是体脂百分比。康奈尔大学的学生开发了他们自己版本的[电子身体脂肪分析仪](http://people.ece.cornell.edu/land/courses/ece4760/FinalProjects/f2014/smb435_pkl25/webpage/index.html "Electrical Body Fat Analyzer")来帮助跟踪身体脂肪百分比。

无脂肪的身体主要含有水分，而脂肪含有很少的水分。这意味着，如果你让电流通过身体，总的生物电阻抗将根据脂肪或水的多少而变化。这不是一个完美的系统，但它可以以相对简单的方式给出一个粗略的近似值。

学生的系统将一个电极放在一只手上，另一只放在另一只脚上。这提供了人体内可能的最长的电路径，以允许可能的最精确的测量。ATMega1284P 用于产生 50kHz 方波信号。为了用户安全，该信号[被光隔离](http://hackaday.com/2014/10/10/macgyvered-optoisolator-is-a-great-introduction/ "Optoisolater")。然后，电路的另一级使用该源信号产生 50kHz 的 10ua 电流源。这是通过人体，并反馈给微控制器进行分析。

电压读数通过串口发送到 MATLAB 脚本。用户还必须输入他们的体重和年龄。MATLAB 脚本使用这些数字结合电压读数来估计身体脂肪百分比。为了校准系统，学生们用体脂卡尺测量了 12 名同龄人的体脂。他们承认他们的样本量太小了。所有的样本对象都大约 21 岁，并且具有相似的体脂百分比。这意味着他们的系统目前对这个范围的人来说非常准确，但对其他人来说可能不太准确。

[https://www.youtube.com/embed/pShGg8_L1D4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/pShGg8_L1D4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)