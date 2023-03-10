# 动作感应水枪推文照片让敌人难堪

> 原文：<https://hackaday.com/2015/06/22/motion-sensing-water-gun-tweets-photos-to-embarrass-enemies/>

【Ashish】用[动作感应水枪](http://www.instructables.com/id/Water-squirting-twitter-enabled-intruder-alarm/?ALLSTEPS)将办公室战带到了一个新的高度。这种水枪不仅在检测到运动时会自动开火，还会拍摄受害者的照片，并由[发布在推特](https://twitter.com/lightbluebean)上。

这次黑客攻击始于水枪。【Ashish】用的是超级透雨雷暴机动水枪。他把箱子拆开，剪断了一根电池线。然后他加长了暴露的末端，并把它们从枪中引出到他的控制电路中。他还放置了一个保护二极管，以帮助防止任何反电动势损坏他更敏感的电子设备。新的控制线连接到电路板上的 MOSFET。

[Ashish]正在使用一个[浅蓝色的](http://store.hackaday.com/products/lightblue-bean)板作为微控制器。该 Bean 与 Arduino 兼容，可以通过低能耗蓝牙进行编程。Bean 使用外部 PIR 传感器来检测房间内的运动。当它感应到运动时，它激活 MOSFET，然后打开水枪。

[Ashish]决定使用 Node-RED 和 Python 将 Bean 链接到 Twitter 帐户。该系统在计算机上运行，并监控 Bean 的串行输出。如果它检测到正确的命令，它会启动一个 Python 脚本，使用网络摄像头拍照。第二个脚本会将照片上传到 Twitter 帐户。Node-RED 服务器还可以监控 Twitter 帐户中的直接消息。如果它检测到带有正确密码的消息，它可以使用消息的其余部分作为命令来启用或禁用枪。