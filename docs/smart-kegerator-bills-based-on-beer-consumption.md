# 基于啤酒消费的智能啤酒账单

> 原文：<https://hackaday.com/2014/03/11/smart-kegerator-bills-based-on-beer-consumption/>

Kegerator 的所有权很棒，但也有不好的一面。如果没有罐子或瓶子来计数，很难跟踪谁喝了什么。[菲尔]正在寻找一个好办法来解决这个问题，当谈到与他的室友和朋友分享啤酒时，他刚刚完成了他的智能啤酒桶的第一次迭代。

他设计了一个基于树莓派的系统。他的软件可以识别拿啤酒的人的脸，并根据小桶的价格和倒的量在他们的账单上加上费用。该系统还跟踪 kegerator 内部当前和历史的温度和湿度值，一切都显示在一个 [Mimo 720S](http://www.amazon.com/Powered-Slide-out-Touch-Screen-Monitor/dp/B002QFP4Z8/ref=sr_1_1?ie=UTF8&qid=1394450430&sr=8-1&keywords=mimo+720s) 触摸屏上。

[Phil]在每个桶上都有一个[流量计](http://www.adafruit.com/products/828)来检测和监控倒酒。这将触发 Pi 摄像头模块运行面部识别。跳转后发现的遍历可能有点混乱；在录制的时候，这个装置只能进行面部*检测*。[Phil]用 QT 和 C++编写了 UI，并使用 Python 脚本处理流中断。他的未来迭代计划包括小桶下面的重量传感器，用于更准确的啤酒温度读数的液体探针温度计，用于弱光条件的 [NoIR Pi 相机模块](http://www.amazon.com/Raspberry-Pi-Camera-Filter-Vision/dp/B00G76YEU8/ref=sr_1_1?ie=UTF8&qid=1394450401&sr=8-1&keywords=raspberry+pi+noir)，以及你将在他的构建页面上看到的真正时髦的用户界面。

如果你没有 Pi，这里有一个 [Arduino-fied kegerator，它可以报告温度并控制啤酒冷却](http://hackaday.com/2013/12/13/over-engineered-kegerator-is-glorious/)。

[https://www.youtube.com/embed/9UmkgNAIu60?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/9UmkgNAIu60?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)