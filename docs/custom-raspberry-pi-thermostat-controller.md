# 定制树莓 Pi 恒温控制器

> 原文：<https://hackaday.com/2014/11/26/custom-raspberry-pi-thermostat-controller/>

恒温器可能是一种痛苦。在一个多房间的家里，他们通常只查看一个传感器，然后根据这个传感器来设置温度。结果是一个房间很舒服，而其他房间不舒服。另外，你通常不得不离开沙发来改变温度。在这个时代，谁想这么做？你可以购买现成的解决方案，但有时自己动手定制硬件更有趣。

[redditseph]正是这样做的，他把家里的恒温器[改成由树莓皮控制。温度由运行在 Pi 上的简单 web 界面控制。通过这种方式，[redditseph]可以使用电脑或智能手机在家中的任何房间改变温度。他还在设计中内置了多传感器功能。这意味着 Pi 可以从家中的多个房间获取读数，并使用这些数据来做出关于如何改变温度的更智能的决定。](http://imgur.com/gallery/YxElS "RasPi Thermostat")

Pi 需要一种方法来真正与恒温器对话。[redditseph]用一个中继模块完成了这项工作。Pi 翻转继电器的一侧，然后继电器依次切换内置在恒温器中的按钮。Pi 基本上只是模仿人类按下按钮。他的恒温器内部有接线端子，所以[redditseph]不必冒险焊接任何东西来损坏它。最终的结果是一个功能性的设计，有一种赛博朋克的外观。

[via [Reddit](http://www.reddit.com/r/raspberry_pi/comments/2nc4z5/my_homemade_raspberry_pi_smart_thermostat/ "Reddit.com")