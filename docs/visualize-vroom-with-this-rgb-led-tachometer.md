# 用这款 RGB LED 转速表来观察轰鸣

> 原文：<https://hackaday.com/2014/07/07/visualize-vroom-with-this-rgb-led-tachometer/>

[Pete Mills]最近购买了全新的福特嘉年华，其燃油经济性超过了他的吉普车。他很快发现，他可以通过福特的 OpenXC 平台实时访问大量的发动机和底盘数据，并利用这些数据构建了新像素转速表 blue shift。这辆车已经有一个环节，但这个更直观，可以在外围看到，只是简单的乐趣。

如果你没听说过，OpenXC 平台是福特消费者打开 OBD2 宝藏王国的钥匙。它通过其车辆接口解锁魔法，该接口插入 OBD2 端口并将 CAN 总线消息转换为 OpenXC 格式。这些消息被打包成 JSON 格式，可以通过蓝牙或以太网/Wi-Fi 发送到 Android、Python 或 iOS 设备。

[Pete]使用蓝牙，并在 Arduino Pro Mini 上使用 BlueSMiRF。他从汽车的车载 USB 端口获取电力，但未来计划使用 OpenXC VI 端口。blueShift 读取转速数据，并在发动机加速时显示绿色轨迹。在最高转速时，它显示红色 LED。这一次是粘性的，将持续不到三秒钟或达到新的正 RPM 的时间。[Pete]也在读取汽车的前灯状态。它们一亮，RGB LEDs 就会变暗，以避免他在夜间失明。

[Pete]想做一个比特百惠盒子更美观的外壳。他几乎绕过 3D 打印机设计，但最终组装了一台 Prusa i3v，并提出了这种 RAM 安装兼容外壳。他精彩的文章和代码在他的博客上，但你可以跳转到观看一个简短的演示和完整的解释视频。还可以用 OpenXC 让[智能刹车灯](http://hackaday.com/2013/09/15/smart-brake-lights-and-more-with-openxc/)甚至[创作艺术](http://hackaday.com/2013/09/18/team-van-gogh-uses-openxc-to-create-art-from-your-drive/)。

blueShift 的演示视频:

[https://www.youtube.com/embed/qYp3V5nOi-k?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/qYp3V5nOi-k?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

完整解释:

[https://www.youtube.com/embed/lUmPiPhLRXw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&start=34&wmode=transparent](https://www.youtube.com/embed/lUmPiPhLRXw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&start=34&wmode=transparent)