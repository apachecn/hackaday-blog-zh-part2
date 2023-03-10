# 如何直接对廉价的 ESP8266 WiFi 模块进行编程

> 原文：<https://hackaday.com/2015/03/18/how-to-directly-program-an-inexpensive-esp8266-wifi-module/>

ESP8266 是“我想要带 Wifi 的东西”的答案令人惊讶的是，有许多工程师和爱好者没有听说过这种芯片，或者听说过但并不真正了解它是什么。它基本上是困扰业余爱好者和商业界的许多工程问题的答案。

该芯片是一个处理器，集成了 RAM、一些 ROM 和 WiFi 无线电，您需要的唯一外部组件是 4 个电容器、一个晶体和一个外部闪存！很便宜，大概 4 美元/个！或者 5 美元，如果你想在一个漂亮，方便的载板，包括所有这些组件。功耗合理(~200mA) ^([1](http://hackaday.com/2015/03/18/how-to-directly-program-an-inexpensive-esp8266-wifi-module/#cite1)) ，射程疯狂~300m ^([2](http://hackaday.com/2015/03/18/how-to-directly-program-an-inexpensive-esp8266-wifi-module/#cite2)) 无定向设备，一个 PCB 跟踪天线和~4km 如果你想可笑。

更多人需要了解的一个地方是如何直接为该芯片编程。很多时候，项目通过 AT 命令把它当作拐杖使用。请继续阅读，了解如何使用这款芯片与世界打招呼。

## 了解你的硬件

首先，介绍一些背景。先来一张它的图片(被 zeptobars 解封)，用 swimmmerdude 标注。 ^([3](#cite3))

[![ESP8266 Decapped](img/65d68f299e092b322b1a09078e805be0.png)](https://hackaday.com/wp-content/uploads/2015/03/crzy9am.png)

默认情况下，处理器运行频率为 80 MHz，但最高可达 160 MHz，它有大约 80kB 的 DRAM(数据 RAM)和大约 35kB 的高速 IRAM(指令 RAM)。 ^([4](#cite4)) 对，就是说它采用了哈佛的架构。IRAM 在启动时加载用户希望保留在处理器上的任何内容，尽管处理器可以直接从外部闪存以较低的速度运行代码。

### 固件背景

默认情况下，当您购买这些小巧的主板时，其中许多都带有“at”固件，这基本上是一个非常简洁、简单的工具，您可以将这些设备用作通过串行端口控制的简单无线调制解调器。这很简洁，但是很难用它来做特别复杂的事情，正如我之前提到的，它需要使用外部处理器。

[![esp8266-how-to-thumb](img/3de1a221ef44b173ca45b50f85f01431.png)](https://hackaday.com/wp-content/uploads/2015/03/esp8266-how-to-thumb.jpg)

Two different ESP8266 modules

根据某些 GPIO 引脚的配置，芯片可以启动几种模式。我们不会讨论“sd 卡启动”,因为大多数业余爱好者社区还没有真正接受它，但我们将讨论 Flash 启动和 UART 下载。此外，有一个远程固件上传功能，有一些不同的版本和可能性，但我们将保存为另一个职位。

对于我们关心的两种模式，处理器期望在启动时 GPIO15 为低电平，GPIO2 为高电平。GPIO0 在我们将要讨论的两种模式之间进行选择。正常工作期间，我们希望使用一个电阻来拉高 GPIO0。 ^([5](#cite5)) 这将导致 ESP8266 内部的引导加载程序从 EEPROM 芯片读取数据到 ESP8266 的 IRAM 中，并引导我们的程序。然而，如果我们将 GPIO0 设为低电平，则 ESP8266 内部的引导 ROM 将接管并开始通过 UART 进行通信。使用这个引导 ROM，我们可以把程序推到闪存中。利用这一点的一个好方法是将一个开关从 GPIO0 连接到地，这样你就可以在开机时按住按钮随意将其置于编程模式。

这非常可靠，甚至支持不同的波特率。我使用 454，800 作为我的波特率，所以我可以很快地修改和测试我的程序。我的一个项目编译不到一秒钟，刻录大约需要 8 秒钟。有官方工具可以上传固件“XTCOM”，不过我个人喜欢使用 esptool.py ^([6](#cite6)) ，因为它可以让你自动刷新。此外，一旦它完成闪存芯片，即使 GPIO0 被连接到低电平，它也会导致您的固件运行。然后，如果您的代码重新启动，它将自动重新进入引导加载程序进行下一个编程周期。这意味着你可以在开发的时候保持 GPIO0 和 GND 的连接。

[![setup](img/a770b37252ebc9bbdcb949a25e7d232d.png)](https://hackaday.com/wp-content/uploads/2015/03/setup1.png)

总而言之，我们的开发工具看起来像:

*   一个从 GPIO0 到地的开关(带有一个到 VCC 的上拉电阻)
*   GPIO2 和 CH_PD 连接到 VCC
*   GPIO15 接地
*   USB 转 TTL UART 适配器，与 ESP8266 通信，并向为芯片供电的 3.3V 调节器提供 5V 电压

顺便说一句…你可以非常便宜的买到 USB 转 TTL 的 UARTs，看看 electrodragon 的那些不到 1 美元/个的！

## 工具链

对 ESP8266 进行编程有点困难，但是一旦开始，事情就很容易了。在 Linux 和 OSX 上构建工具链有几个选项，在 Windows 上还有一些选项。我试图在我的 ws2812esp8266 自述文件中保持[工具链列表尽可能地更新。关于构建工具链的细节超出了本指南的范围，但是请遵循该指南，或者本](https://github.com/cnlohr/ws2812esp8266)[可能更为最新的工具链教程](https://github.com/esp8266/esp8266-wiki/wiki/Toolchain)，你应该没有问题。一旦构建了工具链，并且可以编译固件，比如我的 WS2812ESP8266 固件，就可以开始本文的其余部分了。

Espressif 已经很好了，免费分发他们的 SDK。这绝对震惊了整个社区，从好的方面来说！这是非常慷慨的举动，很少有公司这样做。SDK 包含一个例子，ROM 和 Espressif 库的头文件。值得注意的是有一个社区库，但是到目前为止我每次使用它时，它都没有达到 espressif 库的成熟水平。也许将来会改变。

请务必查看他们 SDK 中的“include”文件夹。这包括许多令人敬畏的功能，帮助你从零到英雄在任何时间！

## 编程:这方面有一个 ROM

对 ESP8266 进行编程时，需要注意一些事项。一是你可以利用内置在 ROM 中的一系列功能。这意味着您不需要(也不应该)重新实现 MD5(即使使用 hmac)、SHA1、与外部闪存的通信、SPI、UART 功能、软件浮点功能、AES、内存命令、printf、低级 IO 工具，甚至实时事件调度程序，最重要的是……802.11！

驻留在片内 ROM 中的完整功能列表可在 eagle.rom.addr.v6.ld 中找到。您现在应该看看那里，看看开箱即用的 awesome 仙境。

除了片上 ROM 之外，还有更多 API 在上面，使得使用这个东西非常容易。我们可以看到一些辅助工具。因为 ESP8266 可以充当接入点或客户端(或者两者兼而有之，尽管我从未尝试过)，所以它有许多工具可供您使用。默认情况下，ESP8266 有自己独特的 AP。也就是说，当您打开它的电源并启动他们的 API 时，它会以主机模式启动，运行自己的 DHCP 服务器。找一个以 ESP8266 开头的 wifi 网络就能找到。

## 拥抱抽象

如果你想写 main 并拥有自己的主循环，那是不可能的。虽然您可以编写 main，但是 API 希望有自己的主循环。从这个意义上说，对 ESP8266 编程很像对 Arduino 编程。

```
static void ICACHE_FLASH_ATTR procTask(os_event_t *events)
{
    system_os_post(procTaskPrio, 0, 0 );
    printf( "Idle Task\n" );
}

void user_init(void)
{
    system_os_task(procTask, procTaskPrio, procTaskQueue, procTaskQueueLen);
    system_os_post(procTaskPrio, 0, 0 );
}

```

如果你需要事件定期发生，有定时器函数，os_timer_setfn，os_timer_arm 可以在特定的时间间隔调用一个函数。

这对整体环境来说很好，但是，我们实际上还没有讨论如何使用这部分。下面就来说说 802.11 怎么用这个。如果你害怕，我不怪你。试图改变 802.11 设置或连接到网络等是一个可怕的命题。有没有试过在 Linux 或 Windows 中用编程的方式来做这件事？太恐怖了。不过，在 ESP8266 上，这很简单！

## 用 8 行代码将 ESP8266 连接到 AP

一旦您的 ESP8266 启动，如果在它应该连接到现有网络的地方发生了一些事情，编写以下代码，它就会发生:

```
const char ssid[32] = "my_home_ssid";
const char password[32] = "my_home_password";

struct station_config stationConf;

wifi_set_opmode( STATION_MODE );
os_memcpy(&stationConf.ssid, ssid, 32);
os_memcpy(&stationConf.password, password, 32);
wifi_station_set_config(&stationConf);
wifi_station_connect();

```

不，真的，就是这么简单。它只会连接到你的接入点，拉一个 IP，然后坐在那里。不要大惊小怪。最重要的是，它会记住这个操作，下次你启动它时，它会马上连接上。当我用一个好的接入点使用它，我能够让它连接，在开机后约 2 秒钟。是的，真的有那么快。

## 服务 TCP

做一个 TCP 服务器怎么样，一个可以监听端口并发回数据的东西？那肯定很难。没有。下面是我为它编写的一个 HTTP 服务器的例子:

```
//Allocate an "espconn"
pHTTPServer = (struct espconn *)os_zalloc(sizeof(struct espconn));
ets_memset( pHTTPServer, 0, sizeof( struct espconn ) );

//Initialize the ESPConn
espconn_create( pHTTPServer );
pHTTPServer->type = ESPCONN_TCP;
pHTTPServer->state = ESPCONN_NONE;

//Make it a TCP conention.
pHTTPServer->proto.tcp = (esp_tcp *)os_zalloc(sizeof(esp_tcp));
pHTTPServer->proto.tcp->local_port = 80;

//"httpserver_connectcb" gets called whenever you get an incoming connetion.
espconn_regist_connectcb(pHTTPServer, server_connectcb);

//Start listening!
espconn_accept(pHTTPServer);

//I don't know what default is, but I always set this.
espconn_regist_time(pHTTPServer, 15, 0);

```

接收连接怎么办？你可以这样做:

```
//This function gets called whenever
void ICACHE_FLASH_ATTR server_connectcb(void *arg)
{
    int i;
    struct espconn *pespconn = (struct espconn *)arg;

    //espconn's have a extra flag you can associate extra information with a connection.
    pespconn->reverse = my_http;

    //Let's register a few callbacks, for when data is received or a disconnect happens.
    espconn_regist_recvcb( pespconn, http_recvcb );
    espconn_regist_disconcb( pespconn, http_disconnetcb );
}

```

就是这样。发送数据？espconn_sent。关闭连接？espconn_disconnect。无论何时获取数据，都是通过 recv 回调传递的。

你可能已经注意到我使用了 ICACHE ATTR 指令，嗯？还记得我们没有多少 IRAM 吗？这样做会将功能保存在闪存上。指令被缓存，但从闪存加载不会花费太长时间。

## 使用 GPIO

我将在本文中讨论的最后一个要点是 GPIO。这些引脚具有可选的内部上拉电阻(GPIO0..15)和下拉电阻(GPIO16)。它们都可以配置为输入或输出。有一些处理 GPIOs 的实用函数。你需要调用 gpio_init(…)有些是宏，比如 PIN_PULLDWN_DIS(…)，PIN_PULLUP_EN(…)，还有一些可以在 SDK 中找到。您可以使用 gpio_output_set 配置输入/输出。许多 GPIO 可能有多种功能，其中一些功能在默认情况下是启用的，因此，例如，在启动时，您不能对 GPIO12 和 GPIO14 做任何事情，直到它们被选择为 GPIO。

```
    PIN_FUNC_SELECT(PERIPHS_IO_MUX_MTDI_U, FUNC_GPIO12); 
    PIN_FUNC_SELECT(PERIPHS_IO_MUX_MTMS_U, FUNC_GPIO14); 

```

学习编程 ESP8266 就像学习在任何其他环境中编程一样。当您试图弄清楚什么是什么，或者查看是否有一些简单的方法来做您想要做的事情时，SDK 提供的头文件非常有用。到目前为止，数据手册对我来说还不是很有帮助，不过，谷歌是找到如何使用这款器件的最佳工具。

## 社区

因为这部分真的是许多问题的答案，它已经采取了业余爱好者社区的风暴！像[esp8266.com](http://esp8266.com)和俄罗斯同行 [esp8266.ru](http://esp8266.ru) 这样的论坛上，到处都是试图用这部分做些令人敬畏的事情的人！他们都是互相学习如何充分利用这个小角色的人。

## 资源

[1]关于该芯片的大量信息的通用 wiki，如电气特性等。大部分内容都是从中国的数据表中翻译过来的。

[2]我在 ESP8266 上进行的范围测试。

[3]在 reddit 上，swimmmerdude 给出了他对解封芯片的猜测[http://www . Reddit . com/r/electronics/comments/2jq 22 l/esp8266 _ wifi serial _ chip _ decapped _ its _ actually/](http://www.reddit.com/r/electronics/comments/2jq22l/esp8266_wifiserial_chip_decapped_its_actually/) 

【4】地址空间的存储器映射，SPI Flash 布局，寄存器包括 IOMUX:

【5】关于 ESP8266 启动方式的讨论:

[6]esptool . py 站点，包含有关将程序上传到 ESP8266 的信息以及有助于闪存的替代布线方案。

[7]ESP SDK 0 . 9 . 5 的官方 espressif 帖子