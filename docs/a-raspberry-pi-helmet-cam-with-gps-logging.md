# 一个带 GPS 记录的树莓 Pi 头盔摄像头

> 原文：<https://hackaday.com/2014/08/14/a-raspberry-pi-helmet-cam-with-gps-logging/>

在过去的 20 年里，[Martin]一直用一个标准的头盔摄像头记录滑雪跑步。这很好，但他觉得他可以通过[构建自己的版本](http://www.stuffaboutcode.com/2014/01/raspberry-pi-gps-helmet-cam.html)并记录额外的数据值，如速度、温度、高度和 GPS，来改进设计。在休息后显示的视频中，第一人称视角显示了 GPS 覆盖图，记录了穿过雪地的路径。[马丁]通过使用一个名为 [picamera](https://pypi.python.org/pypi/picamera) 的 python 模块启动视频捕捉并将位置写入数据文件来实现这一点。然后，他修改了程序，读取当前的帧数，并将 GPS 点同步到视频中的准确位置。 [MEncoder](mencoder) 用于将图像合并成一个媒体文件。

最初的设计是基于几个月前【马丁】开发的 [Raspberry Pi GPS 汽车仪表盘摄像头](http://www.stuffaboutcode.com/2013/10/raspberry-pi-car-cam-gps-data-map.html)。头盔摄像头中的代码利用了许多与收集 GPS 数据点、录制视频和生成覆盖图相同的功能。让这个项目与众不同的是所涉及的挑战。例如，汽车内的相机很少需要处理极端的温度下降或雪山潮湿的天气条件。车辆的外部可能会被雪打坏，但相机仍然相对安全。为了在冒险进入寒冷的环境之前测试树莓派，[马丁]把电脑放在冰箱里，看看会发生什么。幸运的是，它完美地工作。

点击休息时间，阅读故事的其余部分。

[Martin]遇到的另一个障碍是绕过 Raspberry Pi 自定义 Linux 内核中的一个错误，该错误导致相机在同时使用单线传感器时失败。恢复到旧的内核版本解决了这个问题，允许他连接一个温度传感器来记录数据。

一切就绪后，[马丁]在斜坡上试着戴上头盔摄像头。令人惊讶的是，Pi 供电的系统比他预期的更健壮。他能够在一周的时间内捕捉几个小时的镜头，几乎没有问题。唯一出现故障的组件是一根断裂的微型 USB 电源线。这导致 Raspberry Pi 不断重启、短路，最终导致文件系统损坏。

总体结果是 GPS 跟踪、环境感应和视频记录的完美结合。这种类型的设计可以过渡到摩托车头盔和其他运动装备。我们看到了这个系统被整合到水肺潜水、越野自行车和足球运动(以及其他运动)中的潜力；所有这些都给了人们一个进入这些运动员视角的机会。想知道从雪山上飞下来是什么感觉，请看下面[马丁]的视频:

[https://www.youtube.com/embed/wChI6VVYDUc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/wChI6VVYDUc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)