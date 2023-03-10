# 如何让亚马逊 Echo 控制假 WeMo 设备

> 原文：<https://hackaday.com/2015/07/16/how-to-make-amazon-echo-control-fake-wemo-devices/>

[克里斯]一直在玩亚马逊回声。这有点像让 Siri 或谷歌成为你家的一部分，但内置了对某些其他家庭自动化设备的支持，如 Belkin WeMo 和飞利浦的设备。问题是[克里斯]不想只局限于这些品牌。他有其他家庭自动化设备，他觉得应该与亚马逊 Echo 一起工作，但没有。就在那时，他想出了一个聪明的主意，就是[模仿一个受支持的平台](http://www.makermusings.com/2015/07/13/amazon-echo-and-home-automation/)。

WeMo 设备使用 UPnP 在网络上执行某些功能。[Chris]想看看这些通信实际上是如何工作的，所以他启动了他的笔记本电脑，并将他的 WiFi 适配器设置为监控模式。然后他用 Wireshark 开始收集数据包。他发现设备检测功能从使用 UPnP 搜索 WeMo 设备的回声开始。然后，设备使用 HTTP over UDP 使用设备的 URL 来响应回显。然后，回显使用该 HTTP URL 请求设备的描述。然后描述作为 HTTP 响应返回。

WeMo 设备的实际“开/关”功能更简单，因为 Echo 已经知道该设备。Echo 只是通过 HTTP 接口连接到 WeMo，并发出“SetBinaryState”命令。WeMo 然后通过 HTTP 强制返回一个确认。

![WeMo Echo](img/243b6d6fe22959f0dda431470845671e.png)

How Echo Communicates with WeMo Devices

[Steve]能够利用这些信息建立自己的 WeMo“虚拟云”。每个虚拟设备都有自己的 IP 地址。他们还需要一个 UDP 广播监听器，以及一个运行在 WeMo 端口 49153 上的 HTTP 监听器。每个虚拟设备还需要能够响应 UPnP 发现请求和“开/关”命令。

[Chris]使用 Linux 服务器，为每个虚拟 WeMo 交换机创建新的虚拟以太网接口。一个 Python 脚本运行 WeMo 仿真，监听 UPnP 广播并为每个虚拟设备发送不同的响应。响应的一部分包括设备的“友好名称”，这是当用户说出语音命令时 Echo 侦听的内容。由于虚拟 WeMo 设备是免费的，这允许[Chris]为每个设备制作多个短语。因此，除了局限于“电视”之外，他还可以为“电视”制作一个独立的设备，执行相同的功能。[Chris]也不再仅限于特定品牌的家庭自动化设备。

破解这个设备还有很长的路要走。有很多硬件可以使用。其他人有没有接触过这些东西(和工作台工具)？