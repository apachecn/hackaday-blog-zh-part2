# DEFCON 22:黑掉所有的东西

> 原文：<https://hackaday.com/2014/08/09/defcon-22-hack-all-the-things/>

今天早上，我参加了一个名为*Hack All Things*的精彩演讲。是由 GTVHacker 提出的。如果你不认识这个名字，这就是黑掉谷歌电视的组织[。自从那次成功后，他们就没有停止过黑客攻击，这次演讲是关于他们最近开发的 20 多种设备，并且](http://hackaday.com/2012/02/20/sony-google-tv-devices-running-unsigned-kernels/)[公开了这些信息](http://dc22.gtvhacker.com/)(当我检查时，那个链接仍然有誓言，但应该很快就会公开)。

他们提出的攻击有三种风格:UART、eMMC 和命令注入错误。我现在将添加中断，但我会给出他们展示的大多数设备利用的纲要。我觉得这些都很有趣，而且常常很滑稽。

### UART 黑客

PCB 上的 UART 连接通常很容易发现。最常见的是 3 或 4 根针排成一行或一个正方形。因为几乎所有的东西都运行 Linux，所以一旦你有了一个串行连接，这个设备就很熟悉了。让我们看看一些硬件:

*   Epson Artisan 700/800 打印机和 Belkin Wemo 都有 UART 漏洞。
*   Greenwave reality 智能灯泡配有开放式 U-boot，允许您在启动时发出命令以打开 root shell 访问。
*   [文件传输器](http://www.filetransporter.com/)(cloud/nas；是 drobo 的 kickstarter)。基于 Buildroot。UART 报头实际上是在这里填充的！
*   Vizio CoStar LT (ISV-B11)。启动时，它会在 USB 上寻找 fs.sys。研究发现，这是设备正在寻找的 U-Boot 文件。给它你自己制作的 U-boot 镜像，然后你就可以打开这个设备了。
*   [Staples Connect](http://www.staples.com/sbd/cre/marketing/staples-connect/) : wifi、ZigBee(UART)——NAND 芯片上的短路引脚 29 和 30 在上电时破坏 U-Boot，并提供 U-Boot 访问，这是打开根控制台的一个简单途径。

### eMMC 黑客

eMMC 基本上是一个芯片上的 SD 卡。如果你能接入数据线，你就能拥有设备上的数据并监控交易。通常你可以通过焊接到附近的电阻上来接触引脚。这里有一些采用这种方法的设备:

*   亚马逊 Fire TV
*   海信安卓电视(更名为谷歌电视)
*   LG 智能冰箱(LFX31995ST)
*   Vizio Stmart 电视(VF552VXT)
*   索尼 BDP-S5100(蓝光)
*   LG BP 530(蓝光)

### 注射攻击:

无论您是否知道这个术语，您都应该已经熟悉了注射攻击。这最好被描述为实现很差的用户界面；您可以输入文本的地方，不搓擦命令。

*   摩托罗拉 RAZR LTE 基带(处理器独立于 Android)。这是通过 USB 网络连接完成的。
*   PogoPlug 可以通过 web 界面进行注入攻击
*   网件推 2TV 机顶盒。您可以通过 UART 中断引导加载程序。您也可以在引导期间进入根 shell 一两秒钟。你甚至可以通过机器的昵称注入以 root 用户身份运行命令。
*   Ooma Telo 路由器。ssh 已经在运行(仅限局域网)，但默认情况下它是防火墙。您可以通过 web 界面 IPtables 字段注入一个命令来关闭防火墙。(默认 root 密码是！ooma123)。
*   网件 NTV200-100NAS。盒子上的所有东西都有签名。通过 web 界面的另一个注入。更新通过 http 下载。你可以拉下一个应用程序，插入你的符号链接，把你自己的命令转储到设备上来打开一个根 shell。
*   华硕魔方(谷歌电视)。发表演讲的团队在 Play store 上放了一个应用程序以获得 root，但谷歌将其下架(显然他们不喜欢破解他们宝贵硬件的应用程序)。您可以使用内置的媒体应用程序通过其 SMB 装载功能进行注入。

### 获得乐趣:

*   夏日宝贝变焦 WiFi。安全婴儿监控设备根据他们的营销。上传固件有一个硬编码的用户名和密码。这可以通过简单的“curl”命令进行注入攻击。
*   三星 SmartCam。有一个局域网可访问的脚本，它检查密码，但不是为新用户。这可以被利用来让系统认为你在添加一个新用户；当要求您设置密码时，您实际上是在重置 root 密码。

### “天啊，你需要买一个这样的”硬件留到了最后:

![wink-hub](img/af552aa20419f36030d609417f2649a6.png)

Wink Hub 是一项令人惊叹的 pwned 技术。50 美元可以买到一个被称为家庭设备网关的盒子。板上有六个无线电(WiFi、蓝牙、Z-Wave、Zigbee、433MHz Lutron 和 433MHz Kidde)。它将与多种外设接口，如门锁、烟雾探测器、丙烷测量仪、湿度/温度/光感测。

像疯了一样。运行 sudo 命令通过 POST 变量传递值的代码中存在命令注入错误。这些主题不会被转义，因此很容易成为攻击媒介。