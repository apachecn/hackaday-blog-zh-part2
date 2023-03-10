# 你车库里的雷达成像:合成孔径雷达

> 原文：<https://hackaday.com/2014/03/17/radar-imaging-in-your-garage-synthetic-aperture-radar/>

了解你为什么被拦下，量化你最喜欢的模型飞机的隐秘性，或者看看各种家居用品在 10 GHz 下是什么样子。在本帖中，我们将描述合成孔径雷达(SAR)成像的基础知识，从历史的角度开始，展示艺术的状态，并描述在你的车库实验室中可以做什么。让我们用微波成像！

## 特区的历史

[![H2S_Radome_And_Scanner_On_Halifax](img/7245e8584c0a9b317d92b588235331eb.png)](http://hackaday.com/wp-content/uploads/2014/02/h2s_radome_and_scanner_on_halifax.jpg)

The H2S radom (antenna covering, above) and antenna (below).

皇家空军在第二次世界大战中经常使用微波雷达进行地面测绘(或对地面地形成像)，目的是使用 [H2S 雷达系统](http://en.wikipedia.org/wiki/H2S_radar)进行导航和炸弹铺设。H2S 在轰炸机的腹部使用了大口径旋转天线。这种天线会绕圈旋转，其波束指向地面。到目标的距离标绘在平面位置指示器(PPI，或大多数人都知道的雷达屏幕)上，显示飞机下方和周围的情况。

该雷达装置的角度分辨率取决于天线孔径大小(例如天线尺寸)。光圈越大，角分辨率越好，就像手电筒上的反射镜提供的光束越大，光束就越窄(这就是为什么聚光灯能把密集的光束射向天空)。下图是一幅典型的 H2S 雷达图像，记录了美国对柏林的空袭。在该图像中，河流以及其他斑点状目标清晰可见，这些目标是受过训练的操作员能够识别的地标。

[![H2S_Display_Cologne](img/289017ed41b9db25aa23e5746a867027.png)](http://hackaday.com/wp-content/uploads/2014/02/h2s_display_cologne.jpg)

Radar ground image of Cologne during a bombing raid in the Second World War.

早期版本的 H2S 在 S 波段(3 GHz)，后来更高分辨率的设置在 10 和 24 GHz(关于这项技术的有趣阅读， [*战争的回声:H2S 雷达的故事*](http://www.amazon.com/Echoes-War-The-Story-Radar/dp/0852743173/ref=sr_1_1?ie=UTF8&qid=1393110086&sr=8-1&keywords=h2s+radar) )。

合成孔径雷达(SAR)是一种现代地面测绘技术，通过在飞机飞行路径上合成的非常大的孔径来实现高分辨率。这是通过在沿飞行路径的已知位置记录反射雷达脉冲来实现的。雷达必须准确地知道飞机的位置和飞行轨迹中的后退扰动，以便所有散射脉冲在时间和相位上对准。此后，SAR 成像算法被应用于数据以处理图像。

[![airborne_SAR_geometry](img/6304fd1d01efa352813d2ea078e00211.png)](http://hackaday.com/wp-content/uploads/2014/02/airborne_sar_geometry.png)

An aircraft (or other moving vehicle) synthesizes an extremely large aperture by recording scattered radar pulses over the flight path and processing these pulses in a SAR imaging algorithm, thereby synthesizing a very large aperture which provides high angular resolution.

## 合成孔径雷达技术的发展

这项技术最早是在 1957 年开发的，当时使用照相胶片记录雷达数据，并使用镜头制成图像处理器。今天，数字化仪和其他数据采集设备可以存储数据进行离线处理，甚至可以实时处理图像。

最先进的机载 SAR 包括[麻省理工学院林肯实验室极限系统](http://www.ll.mit.edu/asap/asap_05/pdf/Presentations/23_Benitz_P.pdf) (PDF)，它工作在 X 波段(10 GHz)，安装在一架旧 707 飞机上，用于测试先进的 SAR 成像概念。

另一个是桑迪亚国家实验室的 Ka 波段 SAR 成像系统([要查看令人惊叹的机载 SAR 图像组合，请访问此处](http://www.sandia.gov/radimg/ka_band_portfolio.pdf) PDF)，来自该系统的机载 SAR 图像示例如下所示。

[![image from Sandia's system](img/bad27986bdc72e01cf15c6893c30c3a1.png)](http://hackaday.com/wp-content/uploads/2014/02/image-from-sandias-system.png)

SAR imagery from the Sandia National Laboratory’s Ka band airborne SAR imaging system.

合成孔径雷达图像看起来几乎像照片，但它不是照片，而是 2D 全息图。与卫星图像不同，雷达不是从上方测量目标场景，而是在相当远的距离从侧面测量。生成的图像是一个有许多阴影的鸟瞰图，其中每个像素都直接映射到飞机的距离和横向飞行路径上。

最近，重量只有几磅的小型轻型机载 SAR 成像系统已被开发用于微型无人机，例如由 IMSAR 制造的[纳米 SAR 成像系统。](http://www.imsar.com/)

## 创建自己的 SAR 成像系统。

[![railsar_geometry](img/aa743863a2bbd4be0bf4d99b0f0a5137.png)](http://hackaday.com/wp-content/uploads/2014/02/railsar_geometry.png)

To SAR image in your garage, try making a rail SAR imaging system, where a UWB radar sensor moves down well controlled path on a linear rail.

机载 SAR 成像超出了大多数黑客和业余爱好者的能力。好消息是，如果您限制问题的范围并降低雷达传感器的最大范围、功率和复杂性，您可以自己以更好的分辨率完成这项工作。为了实现这一点，可以考虑铁路 SAR 成像系统。在这种情况下，超宽带(UWB)雷达设备安装在一个长线性平台上(通常长度为 6 '到 8 ')。雷达脉冲一次，移动，再脉冲一次，每个回波都被记录下来。这个过程沿着轨道重复进行，直到获得完整的数据集。

对于 UWB 雷达传感器，您可以使用我在上一篇文章中描述的传感器[，它可以是脉冲或 FMCW 雷达，也可以是您自己的传感器。对于线性轨道阶段，您可以使用任何东西，从 Genie 车库门开启器组件(它包含一个长铝挤压件内的](http://hackaday.com/2014/02/24/guest-post-try-radar-for-your-next-project/)[丝杠，一辆车骑在螺纹上](http://glcharvat.com/Dr._Gregory_L._Charvat_Projects/$240_Rail_SAR_hardware.html#6))到全尺寸数控刳刨机上的一个阶段。

##### 用废旧零件制作你自己的

一个拼凑在一起的铁路 SAR 的例子是[“后院 SAR”成像系统](http://glcharvat.com/Dr._Gregory_L._Charvat_Projects/$240_High_Res_Rail_SAR.html)，其中 X 波段 UWB FMCW 雷达前端安装在一个 8 英尺长的线性平台上，该平台由 Genie 车库开门器、无绳钻机传输和步进电机组成，遵循所示框图。x 波段微波组件在[火腿节](http://www.arrl.org/hamfests-and-conventions-calendar)获得。

 [![Block diagram of the 'backyard SAR' imaging system.](img/1a7ec1cc60b04cbafb57f05fa3950775.png "Xband_UWB_FMCW_SAR")](https://hackaday.com/2014/03/17/radar-imaging-in-your-garage-synthetic-aperture-radar/xband_uwb_fmcw_sar/) Block diagram of the ‘backyard SAR’ imaging system. [![The 'backyard SAR' imaging system, deployed in my backyard.](img/ae9f97a34baf81cd8cd0f105a6ae7c98.png "xband_uwb_fmcw_sar_callouts-no-border")](https://hackaday.com/2014/03/17/radar-imaging-in-your-garage-synthetic-aperture-radar/xband_uwb_fmcw_sar_callouts-no-border/) The ‘backyard SAR’ imaging system, deployed in my backyard.

按照 [*聚束式合成孔径雷达:信号处理算法*](http://www.amazon.com/Spotlight-Synthetic-Aperture-Radar-Processing/dp/0890067287/ref=sr_1_1?ie=UTF8&qid=1393188963&sr=8-1&keywords=spotlight+synthetic+aperture+radar) 中距离迁移算法一章概述的程序处理来自轨道 SAR 的数据，步骤如下:

1.  交叉距离离散傅立叶变换。
2.  应用匹配滤波器。
3.  执行斯托尔特插值。
4.  2D IDFT 进入图像领域。

正确实施后，将产生下图所示的图像，在 X 波段实现约 1×1”的分辨率，啁啾带宽约为 5 GHz。

 [![Learn why you were pulled over, radar image of my 5.0 Mustang, apparently the headlights reflect the most microwave radiation!](img/cef557e2bd148ed6b20b5f18b02eeaf3.png "xband_SAR_image_mustang50")](https://hackaday.com/2014/03/17/radar-imaging-in-your-garage-synthetic-aperture-radar/xband_sar_image_mustang50/) Learn why you were pulled over, radar image of my 5.0 Mustang, apparently the headlights reflect the most microwave radiation! [![Radar image of 'GO STATE' in thumbtacks.](img/fd8c88baebc252afdc68ce65c3d11b79.png "xband_SAR_image_gostate")](https://hackaday.com/2014/03/17/radar-imaging-in-your-garage-synthetic-aperture-radar/xband_sar_image_gostate/) Radar image of ‘GO STATE’ in thumbtacks. [![Radar image of my Cannondale M300 mountain bike.](img/9f2be471260963d1a3f2936ed78cd0ef.png "xband_SAR_image_bike")](https://hackaday.com/2014/03/17/radar-imaging-in-your-garage-synthetic-aperture-radar/xband_sar_image_bike/) Radar image of my Cannondale M300 mountain bike. [![Radar image of a scale F14 model.](img/c3fcc57feb9a5b97c5c08bf5b07385a3.png "xband_SAR_image_1_32_f14")](https://hackaday.com/2014/03/17/radar-imaging-in-your-garage-synthetic-aperture-radar/xband_sar_image_1_32_f14/) Radar image of a scale F14 model.

##### 构建咖啡罐雷达套件

[![coffee_can_Radar](img/222b37f98cd6f9697e77e0d2bff5405d.png)](http://hackaday.com/wp-content/uploads/2014/02/coffee_can_radar.png)

The MIT coffee can radar kit is capable of producing coarse SAR imagery.

为了使合成孔径雷达成像成为可能，麻省理工学院开发了“咖啡罐”雷达课程，你可以用咖啡罐雷达进行合成孔径雷达成像。合成孔径雷达成像实验的目的是向学生展示，在对一些非常大的目标成像时，可以区分距离和横向距离。

咖啡罐雷达不会产生最好的图像，但它向学生展示了一个概念。为了获取图像，它被放置在带有卷尺的线性轨道上作为位置参考。这可能是 2×6 英寸的长度或某处的直轨。雷达以 2 英寸的增量手动移动，侧面的拨动开关关闭同步信号输出，向计算机显示雷达已经移动。

产生与下图相当的图像。

 [![SAR imaging with the MIT coffee can radar](img/93adc62c292f7d01e9d0ef86ce0b6761.png "MIT_coffeecan_FMCW_SAR")](https://hackaday.com/2014/03/17/radar-imaging-in-your-garage-synthetic-aperture-radar/mit_coffeecan_fmcw_sar/) SAR imaging with the MIT coffee can radar [![SAR image of the Alexander Calder statue, La Grande Volie, 1968 (<a href="http://www.ll.mit.edu/news/iapradarcourse.html")](img/7135ced505ab032b9bc763be83074adb.png "coffee can radar image from LL website")](https://hackaday.com/2014/03/17/radar-imaging-in-your-garage-synthetic-aperture-radar/coffee-can-radar-image-from-ll-website/) SAR image of the Alexander Calder statue, La Grande Volie, 1968 (<a href="[http://www.ll.mit.edu/news/iapradarcourse.html&quot](http://www.ll.mit.edu/news/iapradarcourse.html&quot);) [![SAR imagery of outdoor terrain using the MIT coffee can radar](img/d8eb36575395b75dceadc08ca8a2bd02.png "MIT_coffeecan_SAR_example")](https://hackaday.com/2014/03/17/radar-imaging-in-your-garage-synthetic-aperture-radar/mit_coffeecan_sar_example/) SAR imagery of outdoor terrain using the MIT coffee can radar

试一试，但一定要拍摄大的目标场景。算法已经写好，程序很简单([向下滚动到‘实验 3: SAR 成像’](http://ocw.mit.edu/resources/res-ll-003-build-a-small-radar-system-capable-of-sensing-range-doppler-and-synthetic-aperture-radar-imaging-january-iap-2011/projects/))。

[这里展示了更多铁路车库制造的 SAR 成像系统的例子](http://glcharvat.com/Dr._Gregory_L._Charvat_Projects/Synthetic_Aperture_Radar_%28SAR%29.html)。

## 学习曲线

为您的后院铁路 SAR 设计、构建和编写成像算法并不简单。实施和处理的注意事项包括:必须适应您的波长范围，需要对点目标(大极点或类似目标)进行校准，使用相干背景扣除和其他处理技术。但是我们可以一整天都思考这些问题，最好的学习方法就是自己去尝试:

1.  边做边学，建造[麻省理工学院咖啡罐雷达](//ocw.mit.edu/resources/res-ll-003-build-a-small-radar-system-capable-of-sensing-range-doppler-and-synthetic-aperture-radar-imaging-january-iap-2011/)并尝试 SAR 成像实验。
2.  有关快速阅读的技术背景，请阅读第 4 章，有关大量实际示例的详细信息，请参见本书第 5 章*(使用促销代码 EEE24 获得折扣)*。
3.  马上处理合成孔径雷达图像。[下载用 MATLAB 编写的 X 和 S 波段数据集及其相关处理算法](//glcharvat.com/shortrange/practical-examples-of-small-synthetic-aperture-radar-imaging-systems/)。通过这个，你将学会如何应用校准和相干背景扣除。
4.  需要帮助吗？将您的问题发布到[锡罐雷达论坛](//glcharvat.com/tincan/?page_id=6)。

有了这些资源、耐心、毅力和咖啡，任何人都可以在自己的车库里创建一个 SAR 成像系统。

* * *

[![DSC_0318](img/9a9df01354628ec27ca241513c3991e0.png) ](http://hackaday.com/wp-content/uploads/2014/02/dsc_0318.jpg) Gregory L. Charvat，著有 [*小型短程雷达系统*](http://www.crcpress.com/product/isbn/9781439865996) ，蝴蝶网络公司的联合创始人，麻省理工学院媒体实验室相机文化小组的客座研究科学家，以及 *Gregory L. Charvat 电气工程实用方法系列*的编辑。从 2007 年 9 月到 2011 年 11 月，他是麻省理工学院林肯实验室的技术人员，他在穿墙雷达方面的工作赢得了 2010 年 MSS 三军雷达研讨会的最佳论文，并且是 2011 年 Provost 研究亮点的麻省理工学院办公室。他在麻省理工学院教授短期雷达课程，他的*构建小型雷达传感器*课程是 2011 年排名第一的麻省理工学院专业教育课程，并被其他大学、实验室和私人组织广泛采用。他开发了许多铁路 SAR 成像传感器、相控阵雷达系统和脉冲雷达系统；拥有多项专利；并开发了许多其他雷达传感器和无线电及音频设备。他于 2007 年获得密歇根州立大学电气工程博士学位，2003 年获得 MSEE 博士学位，2002 年获得 BSEE 博士学位。他是 IEEE 的资深会员，曾在 2010 年和 2013 年 IEEE 国际相控阵系统和技术研讨会指导委员会任职，并于 2010 年至 2011 年担任 IEEE 天线和传播学会波士顿分会主席。