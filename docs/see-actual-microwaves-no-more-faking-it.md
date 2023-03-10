# 看到真正的微波炉——不再假装

> 原文：<https://hackaday.com/2015/09/08/see-actual-microwaves-no-more-faking-it/>

上周，我们看到很多人对无线信号的虚拟化感兴趣。它使用平板电脑作为接口设备，向你展示你周围的无线信号是什么样子的，如果你眯起眼睛，不去想太多，这种感觉会令人印象深刻。但对我来说，这很令人失望，因为我知道实际上有可能看到无线电波的样子。在这篇文章中，我将向你展示如何*通过修改一个你可以在家里制作的咖啡罐雷达来实现它。*

麻省理工学院已故的伟大教授 David Staelin 曾经告诉我，“如果你制作一个新的仪器，并把它对准大自然，你会学到新的东西。”在我提到的所有[咖啡罐雷达](http://ocw.mit.edu/resources/res-ll-003-build-a-small-radar-system-capable-of-sensing-range-doppler-and-synthetic-aperture-radar-imaging-january-iap-2011/)中，迄今为止最有趣的一项是直接测量和可视化 2.4 GHz 辐射，这种辐射在我们的 WiFi、无绳电话(如果你还有的话)和许多其他消费品中使用。当你真的可以做到的时候，没有必要用虚假的想象来欺骗自己。

### 改装麻省理工学院咖啡罐雷达

麻省理工学院咖啡罐雷达向数百名好奇的学生、黑客和资深工程师介绍了雷达、电磁学、RF/模拟设计和信号处理的研究。它被用于私人和政府实验室，成为其他大学的全学期课程，甚至出现在蒙古国家电视台上。

我们将使用该雷达直接对其自身发射器发射的 2.4 GHz 微波场进行成像。

雷达将被配置为显示时变的 2.4 GHz 场，就好像时间静止不动一样。为此，我们将雷达配置为在多普勒模式下工作。这种雷达的独特之处在于，您可以 DC 耦合其前端混频器的输出，从而创建一种有时被称为“微多普勒”的测量设备。由此，混频器的输出是与来自雷达所指向的任何雷达目标的散射信号的相位和幅度成比例的电压。在这种模式下，如果你站在雷达前面，靠近或远离它，你会看到一个与你所站位置成正比的缓慢时变波形。

为了直观显示无线辐射，我修改了该混频器输出端的运算放大器电路，以便它可以为一对 led 供电，一个红色，一个绿色。这些电线极性相反。然后，我卸下了接收器罐，连接了一根微波延长线，并用胶带将 led(带延长线)粘到罐的顶部。有了这种新的天线组件，我可以在实验室里自由走动，连接 led 的接收天线为我提供发射载波的相位和幅度的光学指示。

[![Block diagram.](img/07e977e3db181f08a33239aae8a9656b.png)](https://hackaday.com/wp-content/uploads/2015/08/mit_iap_radar_doppler_wavefront-imaging.png)

Block diagram.

当你在发射机天线前移动接收天线时，你会看到 led 从红色到绿色再到红色，来回变化，跟踪从发射天线辐射出来的波前。

为了捕捉 2.4 GHz 无线波阵面的图像，DSLR 的孔径保持打开，而接收天线在发射机天线的前面附近移动。所有这些都必须在黑暗的房间里完成。

### 2.4 GHz 无线信号实际上是什么样的

如果以上描述令人困惑，请观看此视频:

[https://www.youtube.com/embed/rqCus4ER1d0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/rqCus4ER1d0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

这就是 2.4 GHz 无线辐射的样子。从这些测量中，你可以看到当它离开透射的 cantenna 时的波前曲率。当我们接近距离 2d^2/lambda(其中 d =发射天线的直径)时，我们可以看到[波前变成平面波](https://en.wikipedia.org/wiki/Near_and_far_field)。此外，您可以看到，led 的亮度随着与发射器的距离成反比而下降，正如人们所料。

[![](img/98ded7def6a79df71308d72d8ac5b827.png)](https://hackaday.com/wp-content/uploads/2015/08/imaged-field.jpg)

是的，这个图像的粒度受到我有多少耐心在发射器前面移动接收器组件的限制。对于上面的图片，我花了大约 1-2 分钟。为了获得更好的细节，在 DSLR 快门打开时花更多的时间移动接收器组件。

对于您家中或办公室中的每台无线路由器，这就是辐射场的样子。

### IEEE 微波理论与技术协会(MTT)视频竞赛

这项工作有助于刺激由 IEEE MTT 主办的[创新竞赛](http://www.mtt.org/education/202-youtubeyouku-competition-winners)，其中一些方法被用于各种场景，结果令人惊讶(滚动到下面大约 2 分钟的视频):

[https://www.youtube.com/embed/VaTdotYE_dw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/VaTdotYE_dw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

### 轮到你了

你完全有能力测量和观察无线传播的本质。亲眼看看无线信号在您的实验室和家中传播的样子。如果你仍然不相信这是给你的，看看[大卫·施奈德的] [咖啡罐雷达演示](https://www.youtube.com/watch?v=Zr78A6cJDa4)，和我自己的[视频演示多普勒频移](http://www.youtube.com/watch?v=FOWopYv-JTM)使用硬件。

### **作者简介**

[Gregory L. Charvat](http://glcharvat.com/Dr._Gregory_L._Charvat_Projects/About.html) 喜欢对无线辐射进行成像，是《小型和短程雷达系统》的作者，麻省理工学院媒体实验室的客座研究科学家，Hyperfine Research Inc .和 Butterfly Network Inc .的联合创始人。Greg 是 G. L. Charvat 电气工程实用方法系列的编辑。格雷格是麻省理工学院林肯实验室的前工作人员，在那里他创建了麻省理工学院穿墙雷达麻省理工学院建造雷达课程。除此之外，他还做了很多事情，参与了很多有趣的事情。