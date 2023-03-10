# 用蓝牙控制一个点并拍摄

> 原文：<https://hackaday.com/2014/09/12/controlling-a-point-and-shoot-with-bluetooth/>

装载点和拍摄数码相机在这里是旧帽子，但[亚历克斯]和[安德烈亚斯]正在把它带到一个新的水平。他们为廉价的佳能相机制作了蓝牙控制器[，允许用 iPhone 或 Android 设备拍照。](http://evothings.com/diy-camera-control-on-your-smartphone-via-an-arduino-uno-ble-shield/)

问题中的相机是佳能 IXUS70，尽管任何由 CHDK 支持的相机都可以使用。我们已经看到一些构建使用这个固件来[每天拍摄日出](http://hackaday.com/2014/07/27/enjoying-the-sunrise-every-single-day/)和[通过无线电链路传输图像](http://hackaday.com/2013/09/12/digital-camera-becomes-video-transmitter/)，但是这个构建更具交互性。

该相机通过一根砍断的 USB 电缆连接到 Arduino 和蓝牙屏蔽上。“duino”使用 JQuery 应用程序与手机进行通信，让任何带有蓝牙模块的手机都能控制相机的变焦和快门。

所有代码都可以在 github 上找到[，下面有一个非常好的构建视频演示。](https://github.com/evothings/EvothingsGallery/tree/master/ble-camera-remote/app)

 [https://www.youtube.com/embed/BR1zAzkk_RE?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/BR1zAzkk_RE?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)