# 基于 NAS 的转码有助于在 IPhone 上查看安全摄像头

> 原文：<https://hackaday.com/2012/08/10/nas-based-transcoding-facilitates-security-cam-viewing-on-iphone/>

![](img/55786cf7124e1cb160657caedb8dfccc.png "security-camera-iphone-transcoding")

[Zitt]有一个安全摄像头，它会在任何时候检测到运动时向他发送信息。不管这看起来有多烦人，我们相信他有理由需要这么多即时反馈。当他在 iPhone 上查看提要时，真正的问题出现了。他的解决方案是关闭相机的通知功能，然后[使用他自己的脚本对一个剪辑进行代码转换，并发送一封电子邮件](http://pinball-mods.com/blogs/?p=223)。

正如您在上面看到的，最终结果是一封简洁的电子邮件，其中包括最近捕获的剪辑，以及到实时提要的链接。他一直将剪辑存储在 LG N4B2 网络存储服务器(NAS)上，因为他在设备上获得了 Linux 系统的 root 访问权限，所以这是新系统的一个简单起点。在他从 source(处理代码转换)编译了 FFmpeg 之后，他开始编写脚本来备份录音和发送电子邮件。

他想补充的一点是清除旧备份视频的方法。我们自己也遇到了类似的问题，所以我们决定分享我们的一行程序来解决这个问题。休息后再找。

这里有一个 cron 作业，每天下午 4:50 运行，删除超过三周的备份视频文件。如果你不明白它是做什么的，就[查阅文档](http://www.gnu.org/software/findutils/manual/html_node/find_html/Deleting-Files.html)。

```
50 16 * * * find /Videos/backup/*.mpg -mtime +21 -exec rm {} \;
```