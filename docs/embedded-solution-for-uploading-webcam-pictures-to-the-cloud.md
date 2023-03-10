# 将网络摄像头图片上传到云端的嵌入式解决方案

> 原文：<https://hackaday.com/2013/06/07/embedded-solution-for-uploading-webcam-pictures-to-the-cloud/>

![carambola-webcam-uploader](img/a37481004aa9aa2f45c8d0a7380ee5b0.png)

当我们去外地的时候，我们有朋友照看这些猫。但是我们总是让服务器运行着一个网络摄像头(使用 Linux“motion”软件激活运动)，这样我们就可以自己查看他们了。但是这个项目可能会激发改变。它利用杨桃 2 的特性来捕捉图像，并将它们上传到 Dropbox。

上图中绿色 PCB 是小型黄色 PCB 的开发板，实际上是杨桃 2。它使用与那些 [HC-05 蓝牙模块](http://hackaday.com/2012/01/30/firmware-programmer-for-a-cheap-bluetooth-module/)相同的技术焊接在开发板上。该屏蔽板包括一个运行 Linux 的高通 SoC 和一个 WiFi 无线电。开发板给它供电，并允许它连接到 USB 网络摄像头。

让一切运行起来需要一点命令行功夫，但对初学者来说应该不难。Linux 老手会知道定期从网络摄像头拍摄快照是一项简单的任务。上传到一个安全的云存储站点就不是了。一个 Bash 脚本处理繁重的工作。它使用 Dropbox 应用程序 API，所以这不会违反他们的服务条款，你也不必从命令行找出自己的认证方法。