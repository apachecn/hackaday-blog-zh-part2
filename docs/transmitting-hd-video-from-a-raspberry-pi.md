# 从树莓派传输高清视频

> 原文：<https://hackaday.com/2015/03/28/transmitting-hd-video-from-a-raspberry-pi/>

RTL-SDR 电视调谐器加密狗引爆业余无线电界已经有几年了；这是一个简单的监听数字电视频率的设备，但它是那些能够带来很多乐趣的工具之一。现在，我们有了一个传输加密狗。它仅用于从 Pi 传输现场高清电视，但这本身就非常有趣，并开辟了许多可能的构建。

这个构建的关键硬件是 UT-100C DVB-T 调制器。这是一个 169 美元的 USB 加密狗，能够在 1200-1350 MHz 之间传输，通过[一个特别版的 OpenCaster](http://www.avalpa.com/the-key-values/15-free-software/33-opencaster) 可以传输无线电视。没有放大器，所以你不会把电视传送很远，但它确实工作。

在构建的 Raspberry Pi 端，标准摄像机使用 [raspivid](http://www.raspberrypi.org/documentation/usage/camera/raspicam/raspivid.md) 捕获 H.264 视频，并使用 ffmpeg 将其转换为符合 DVB 的流。在 Raspberry Pi 世界中，这些都是老掉牙的软件，剩下的由 OpenCaster 负责。

虽然这似乎是完全过度建设的四轴飞行器的完美解决方案，但请记住，在 23 厘米波段上传输需要许可证。在超高频电视波段传输是一个坏主意。