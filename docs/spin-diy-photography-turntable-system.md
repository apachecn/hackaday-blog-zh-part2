# 旋转 DIY 摄影转盘系统

> 原文：<https://hackaday.com/2015/05/24/spin-diy-photography-turntable-system/>

电动转盘在拍摄产品照片、创建动画 GIF 或漫游视图时非常方便。[ [Tiffany Tseng](http://web.mit.edu/ttseng/www/) ]建立了 [Spin，这是一个 DIY 摄影转盘系统](http://spin.media.mit.edu/)，用于捕捉 DIY 项目如何随着时间的推移而聚集在一起。它旨在通过创建 GIF 和视频来帮助人们以一种引人入胜的方式分享他们的项目，这些 GIF 和视频将很容易在 Twitter 和脸书等社交网络上发布。

该装置是一个由步进电机驱动的[转盘](http://www.mcmaster.com/#lazy-susans/=xakgk1)，步进电机由 Arduino 和[简易驱动电机驱动罩](http://www.schmalzhaus.com/EasyDriver/)控制。Spin 系统利用[软调制解调器](https://code.google.com/p/arms22/)库将信号从 iPhone 发送到 Arduino。这将通过手机上的音频插座将 Arduino 连接到 iPhone。Spin iOS 应用程序目前处于测试阶段，只接受邀请。在你建造了自己的旋转转盘之后，给它拍张照，然后[请求应用](http://spin.media.mit.edu/request)。当然，有许多不同的方法来控制电机，所以如果你方便，你可以建立自己的控制器。但[蒂芙尼]的 iOS 应用程序提供了一种方法，可以将各种图像拼接成动画 GIF，然后轻松分享。如果您从 [github repo](https://github.com/ttseng/spin) 中获取设计文件，遵循[构建页面](http://spin.media.mit.edu/build)上的详细说明，并使用激光切割机和 3D 打印机，那么构建转盘应该很简单。

看看我们过去介绍过的几个类似的转盘黑客，比如[一个使用扫描仪的电机](http://hackaday.com/2012/04/11/automated-turntable-photography/)，[一个只是最终工作不顺利的尝试](http://hackaday.com/2013/10/10/fail-of-the-week-photography-turntable/)，还有[一个使用皮带驱动系统的](http://hackaday.com/2012/04/27/scanning-turntable-digitizes-objects-as-3d-models/)。休息之后有一段转盘运行的视频。

[https://player.vimeo.com/video/127438804](https://player.vimeo.com/video/127438804)