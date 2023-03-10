# 多输入红外遥控中继器

> 原文：<https://hackaday.com/2014/09/29/multi-input-ir-remote-control-repeater/>

[Peter]的家人的有线电视公司很糟糕，这对有线电视提供商来说是一个惊喜，他们的有线电视订阅的数字部分只能与该公司的有线电视盒一起工作。有线电视公司只出租电视盒，没有购买权，而[Peter]的家人需要五个电视盒来安装家里的所有电视，尽管他们只会同时使用两个。为了不浪费金钱，[Peter]使用同轴分配器可以将一个有线电视盒的输出发送到多台电视，但是遥控器呢？为此，他开发了一种红外遥控多点扩展器。有了几块小板子，他就可以把接收器接到房子里的任何一个房间，然后把它发送回一个有线电视盒，给房子里的每台电视提供数字有线电视，同时仍然只租用一个有线电视盒。

接收器模块使用与电缆盒中相同类型的红外模块来解码来自遥控器的信号。对于一些 MOSFETs，该信号通过一个三位螺丝端子馈入位于电缆箱旁边的发射器模块。该模块使用 PIC12F 微控制器接收信号输入，并将其转换回红外线。

[Peter]的系统可以设置为单个接收器和单个发射器、单个接收器和多个发射器、多个接收器和多个发射器，或者您可以想象的任何配置。这种设置确实需要穿过房子墙壁的几根电线，但即使这样也比有线电视公司每个月拿出支票簿要容易得多。

下面视频。

[https://www.youtube.com/embed/ZRVfaCeGWxY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/ZRVfaCeGWxY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)