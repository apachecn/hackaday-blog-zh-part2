# 以很少的资金构建自己的基于 SDR 的无源雷达

> 原文：<https://hackaday.com/2015/06/05/building-your-own-sdr-based-passive-radar-on-a-shoestring/>

让我们从证据开始。下面是一个我使用雷达系统测量飞机和流星的动画，我用几个简单容易获得的硬件构建了一个雷达系统:两个在易贝购买的 8 美元 RTL 软件定义的无线电软件狗和两个对数周期天线。听着，你要建造的雷达系统是通过监听被测目标反射回来的现有信号来工作的！

几年前，我在一篇非常简短的博客文章中写下了这件事。它主要是作为我们的射电望远镜博客的一个滑稽的小故事，但它最终引起了很多兴趣。因为这一直是一个吸引人的话题，我将更详细地解释我是如何做这个实验的。

[https://www.youtube.com/embed/-k2ZuhAz0ac?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/-k2ZuhAz0ac?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

这将需要几个帖子来展示如何建立一个能够执行这些类型的测量的雷达。第一部分是概述。在以后的文章中，我将详细介绍无源雷达系统不同部分的框图，提供示例数据，并给出一些可用于执行无源雷达信号处理的 Python 脚本。我还将检查策略，以确定一切都按预期运行。所有这一切听起来可能需要很多努力，但别担心，制造一个无源雷达并不太复杂。

我们开始吧！

[![pr1](img/c2e16c43cc1e27d4d8f4b98850dc2da6.png)](https://hackaday.com/wp-content/uploads/2015/06/pr13.png)

A simple passive radar setup. A high power commercial radio transmitter illuminates radar targets, which in this case are an aircraft and a meteor trail that happens to be oriented in a way that allows specular reflection to be seen by the receiver. Two antennas are used: one antenna measures what is transmitted by the radio transmitter and the other antenna is used to record the echoes from the radar targets.

无源雷达是一种特殊类型的雷达，不需要发射机。你依靠别人提供的无线电发射机来照射雷达目标。这可以是你当地的广播电台或电视台，功率高达几兆瓦。与普通雷达相比，它有许多优点:

1.  你不需要发射机，这是一件好事，因为大功率无线电发射机体积大、价格贵、耗电，而且含有危险部件..
2.  成为一名海盗雷达操作员听起来很刺激，但你真的不想在没有 FCC 许可证的情况下进行传输。无源雷达允许你用千瓦甚至兆瓦级的有效辐射功率操作雷达，而不需要制动任何法律法规。
3.  无源雷达系统本质上是多静态的。一个站可以有多个位于不同位置的发射机。这允许估计雷达目标的三维轨迹。有许多雷达目标具有对照射和视角敏感的雷达截面。一个很好的例子是镜面流星余迹回波，只有当照明角度视角组合是镜面反射时，它才具有显著的雷达截面。对于多静态系统，看到这种雷达目标的机会更大，因为在任何给定时间都存在多个不同的同时照射方向。
4.  有许多无线电发射机:电视、调频广播和调幅广播是最明显的，但手机发射塔甚至卫星都可以用于无源雷达。这些发射机覆盖了广泛的频率范围，这对无线电遥感非常有用，因为不同介质和雷达目标的无线电传播特性和散射特性可能高度依赖于频率。例如，如果一个雷达目标在一个频率上没有足够大的雷达截面，那么另一个频率很可能会工作得更好。

[![The first passive radar experiment performed by  Sir Robert Watson-Watt and Arnold Wilkins.](img/99a549ed0c47162266da8d0ef0343111.png)](https://hackaday.com/wp-content/uploads/2015/06/daventry1.png)

A depiction of the Watson-Watts and Wilkins passive radar experiment that detected a Heyford bomber aircraft at Daventry in 1935\. One of the antennas was used to pick up the direct path signal from the BBC short wave radio. This signal was then delayed so that it was out of phase and then used to subtract the direct path radio station signal from the other antenna, leaving mostly the radar echo from the aircraft.

虽然我们现在知道的大多数雷达系统都有专用的发射机，但无源雷达的概念可以追溯到很久以前。第一批雷达实验之一可以归类为无源雷达。1935 年，罗伯特·沃森-瓦特爵士和他的同事阿诺德·威尔金斯进行了第一次飞机跟踪雷达实验，通过探测由英国广播公司短波无线电发射照亮的海福德轰炸机的回波。右图显示了用于执行测量的两个偶极天线和移动实验室。这项开创性的工作是第二次世界大战期间拯救无数生命的[连锁家庭](http://en.wikipedia.org/wiki/Chain_Home)预警雷达系统的基础。

无源雷达有大量的非军事应用。我对被动雷达用于地球物理和天文无线电遥感感兴趣。用于地球物理遥感的一个成功的无源雷达系统的例子是华盛顿大学开发的 Manastash Ridge 无源雷达，用于研究地磁暴期间产生的电离层不规则现象。在过去的 15 年里，这项技术变得更加容易获得，使得用容易获得的硬件进行这些类型的测量成为可能。

Manastash Ridge 雷达使用调频无线电作为被动雷达，这可能是最容易开始的，因为单个电台的带宽相对适中。有了调频收音机，你不仅可以观察到电离层的不规则性，还可以观察到在你周围 100-600 公里范围内飞行的流星和飞机的运动。下图显示了我最近在一次磁暴中进行的测量。你可以看到大规模的电离层不规则结构以每秒 1000 米的速度穿过视野，这与被动雷达接收器北部的北极光有关。

[![fmpr_an](img/968a562839096b88fbb09d81c27ce8f6.png)](https://hackaday.com/wp-content/uploads/2015/06/fmpr_an.png)

An example FM radio passive radar measurement showing echoes from airplanes and ionospheric irregularities observed during a recent geomagnetic storm. Range-Time-Intensity-Doppler color coding is used. The part of the Doppler spectrum that is going away from the receiver is used to determine the value of the red channel, the low-Doppler shift (the part not moving very fast) of the spectrum is used to determine the intensity of the green channel, and the portion of the spectrum with Doppler shifts that indicate the target is moving towards the receiver is used to determine the blue channel. The red, green, and blue channels are then used to form an RGB color for each range-time pixel of the display.

问题是，几乎任何人都可以自己做这些类型的测量。如果有开源软件来分析数据的话。这将为对广泛主题感兴趣的公民科学家打开大门:

*   流星辐射的流星调查。CMOR 雷达通过观察流星辐射发现了 12 个新的流星雨。虽然这是一个有源雷达，但数字电视无源雷达系统也可以做到这一点。雷达可以让你观察到比肉眼更多的流星。
*   通过观察电离层不规则体的回波，绘制北极光的位置和强电离层电场的存在。这告诉我们太阳风和我们星球周围的等离子体之间的相互作用。
*   用流星余迹回波的多普勒测量来测量大气风。这些是 90 到 110 公里高度的中性风的良好示踪物。

如果有一个遍布全球的无源雷达网络，将会有巨大的科学发现潜力。

## 示例硬件

构建一个简单的无源雷达所需的硬件数量少得惊人:

*   个人电脑(五年前的双核电脑即可)。
*   双通道软件无线电。
*   两根天线。

用于 FM 无线电无源雷达的接收器天线对示例如下所示。这两种天线都是对数周期天线，本质上是宽带，但也具有一定程度的方向性。其中一个天线指向调频无线电发射机，用于测量雷达发射的波形。另一个指向相反的方向，用于测量回声。本文中显示的所有示例测量都是使用这些天线进行的。

[![Passive radar antennas for the ISIS passive radar node at the MIT Haystack Observatory.](img/60e7d3f7583664d9f7f2a998daf912f0.png)](https://hackaday.com/wp-content/uploads/2015/06/prant.png)

Directional antennas for the passive radar receiver node at the MIT Haystack Observatory.

需要以相干的方式记录来自这两个天线的信号。这意味着我们需要两个样本对齐的通道。这通常通过使用公共时钟来实现，该时钟用作下变频级和模数转换器的参考。下图显示了可用于无源雷达的两种可能的现成设备。左边是我花 16 美元一起改装的双 RTLSDR R820T 加密狗系统[！](http://kaira.sgo.fi/2013/09/16-dual-channel-coherent-digital.html)右边是 USRP N200 软件无线电，带双通道 TVRX2 调谐器子板。在匆忙实施 RTLSDR 方法之前，有一个警告:为了使一切工作正常，需要做一些细微的调整，包括对齐样本和对齐两个数据流的中心频率。有限的动态范围也使得从系统中获得良好的测量结果更加困难，因为需要仔细调整电平，以使足够的信号进入接收器，同时避免信号的压缩或削波。但是如果你有足够的耐心是可以做到的！我会在下一篇文章中分享这些调整。

为了提高无源雷达系统的保真度，建议在天线和软件无线电之间设置前置放大器和带通滤波器，以降低污染测量的带外噪声，并提高信号电平，使其更适合数字接收机。

 [![two RTLSDR R820T dongles modified to share a common oscillator.](img/ea2861f0ecc56c8c03be56bc37d07061.png "sdr-radar-front")](https://hackaday.com/2015/06/05/building-your-own-sdr-based-passive-radar-on-a-shoestring/sdr-radar-front/) two RTLSDR R820T dongles modified to share a common oscillator. [![Two alternative digital receivers that can be used for passive radar](img/4c6facb77ea322ebbe5788f7fb330e2e.png "sdr-radar-back")](https://hackaday.com/2015/06/05/building-your-own-sdr-based-passive-radar-on-a-shoestring/sdr-radar-back/) Two alternative digital receivers that can be used for passive radar [![a USRP N200 with a TVRX2 daughterboard capable of measuring two receiver channels](img/afe35c0bdfa91c8cb327e7d1f11346a5.png "sdr-radar-filter")](https://hackaday.com/2015/06/05/building-your-own-sdr-based-passive-radar-on-a-shoestring/sdr-radar-filter/) a USRP N200 with a TVRX2 daughterboard capable of measuring two receiver channels

## 信号处理

为了获得被动雷达回波，我们需要对硬件记录的数字信号应用一些信号处理魔法。我们首先需要去掉强的直达波信号，这样我们就可以观察到较弱的回波。Robert Watson-Watt 和 Arnold Wilkins 在他们早期的 Daventry 实验中简单地使用反相信号来抵消直接路径信号。现代信号处理可以更好地做到这一点，不仅可以消除发射机的直接路径信号，还可以消除山坡和其他大型散射体的反射信号，这些反射信号可能会掩盖较弱的目标信号。这是通过使用一种众所周知的称为[线性最小二乘估计](http://en.wikipedia.org/wiki/Linear_least_squares_(mathematics))的统计信号处理技术来对直接路径信号的相位和幅度以及来自山脉和其他强非移动散射体(也称为雷达杂波)的回波进行去卷积来实现的。

在已经估计了强直接路径信号和杂波之后，可以将其从测量信号中减去，并且可以执行信号处理以估计来自飞机或流星的较弱回波。因为我们知道我们感兴趣的较弱目标具有显著的多普勒频移和多普勒扩展，所以我们不能做出与我们对杂波所做的相同的非移动目标假设。然而，我们仍然可以假设目标具有散射多普勒频谱，该频谱在足够长的时间内不会改变，从而允许我们估计距离多普勒频谱。这允许我们对接收到的回波的自相关函数执行去卷积。这就是所谓的滞后剖面反演。虽然这听起来很复杂，但实际上并不复杂。

一旦所有这些都完成了，我们就可以绘制结果了。如果你看到飞机，你的雷达在工作。虽然飞机是令人厌烦的雷达可见物，但它们是迄今为止最容易看到的，而且它们一直都在那里。流星更短暂，但如果你知道要寻找什么，也应该相对容易测量。它们以接近零多普勒频移的快速光点出现。

## 到达角

[![Two antenna interferometry with a passive radar system.](img/c917747ab993b30a280944f5bd3dbcbd.png)](https://hackaday.com/wp-content/uploads/2015/06/pr2.png)

Two antenna interferometry with a passive radar system. The echo arrives at slightly different times on the two antennas, which can be used to determine the arrival angle.

还有许多不同的调频无线电无源雷达可以做到。例如，通过向系统添加第三个天线，可以通过检查彼此隔开的两个接收机天线之间的相位差(到达时间)来执行到达角度方向查找。下面的视频显示了使用两种不同的接收机天线测得的相位差。在该视频中，两个天线之间的相位差用于选择像素的颜色(色调)，回声强度用于对像素的亮度进行颜色编码。同样，可以看到许多飞机和镜面流星回波。

[https://www.youtube.com/embed/rVwuxxhc4WE?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/rVwuxxhc4WE?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

这个帖子到此为止。在接下来的文章中，我将更详细地介绍被动雷达在实践中是如何工作的。

* * *

[![juha3](img/b70ad2a23481a55b2e8772de2f962578.png)](https://hackaday.com/wp-content/uploads/2015/06/juha3.jpg) 我是一名无线电科学爱好者，喜欢与雷达和其他遥感技术打交道。我从小就给电脑编程，还涉猎过电子产品。在攻读题为“雷达测量的统计理论”的博士学位时，我真正进入了设计和制造无线电遥感仪器的领域(在我的网页上可以找到相关链接)。我不满足于只写测量方程，我想在实践中尝试。目前我在麻省理工学院 Haystack 天文台工作，在那里我探索了许多令人兴奋的课题，包括但不限于:电离层、流星和行星物体的高功率大孔径雷达测量；无源雷达、毫瓦级扩频高频雷达、兆瓦级电离层加热、全球导航卫星电离层遥感和射电天文学。我已经发表了两个开源项目，将你的软件定义雷达变成无线电遥感仪器: [GNU Chirp Sounder](http://www.sgo.fi/~j/gnu_chirp_sounder/) ，它允许你收听世界各地的超视距雷达和 Chirp 电离层探测仪；和 [GNU 电离层层析成像接收器(抖动)](http://www.sgo.fi/~j/jitter/web/)，它允许您通过收听卫星上的 150/400 MHz 相干信标来确定电离层电子密度的线积分。