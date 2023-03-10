# 咖啡支付系统不会使你的保修失效

> 原文：<https://hackaday.com/2014/12/27/diy-coffee-payment-system-doesnt-void-your-warranty/>

[奥利弗]回来了，他最近的咖啡机黑客更新。他最新的黑客技术允许他在现成的咖啡机上添加一个[咖啡支付系统](https://www.youtube.com/watch?v=uXPG3yZxTzM "coffee payment system")，而无需修改咖啡机本身。这个项目是他之前在[咖啡壶黑客](http://hackaday.com/2014/11/25/enhanced-coffee-brewer-knows-how-much-of-a-caffeine-addict-you-are/ "coffee maker hacks")的冒险的更新，记录了谁用完了所有的咖啡。

支付系统从一个小项目外壳内的 Arduino Uno 克隆开始。Arduino 使用咖啡机的服务端口通过串行与咖啡机通信。该端口很容易从机器外部获得，因此您不必打开机箱并冒着保修失效的风险。

该系统还包括 RFID 读取器和蓝牙模块。RFID 阅读器允许每个用户拥有他们自己的识别卡。用户可以在读卡器上刷卡，系统就会知道他们的账户里还有多少余额。如果他们有足够的信用，机器会倒一杯美味的咖啡。

Arduino 使用蓝牙模块与 Android 手机通信。[奥利弗的]安卓应用是用麻省理工学院的 app inventor 打造的。它跟踪帐户信用，并允许用户添加更多。该系统目前可以跟踪多达 40 个账户。[Oliver]还提到，您可以使用任何蓝牙终端程序来控制系统，而不是智能手机应用程序。

[https://www.youtube.com/embed/uXPG3yZxTzM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/uXPG3yZxTzM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)