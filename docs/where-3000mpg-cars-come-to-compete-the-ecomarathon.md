# 3000 英里/加仑以上的汽车来竞争:生态马拉松

> 原文：<https://hackaday.com/2015/04/15/where-3000mpg-cars-come-to-compete-the-ecomarathon/>

每年，来自世界各地的团队聚集在一起参加生态马拉松赛(T1)，这项赛事(讽刺的是由壳牌举办)要求来自高中和大学的团队创造节能的电动、燃气和混合动力汽车。今年的比赛在底特律举行，所以我去看看。

![vehicle-blur](img/8c03932eb7efca8525075c6e0713e380.png)这项赛事分为两类参赛车辆:竞争最高燃油效率的原型车和“城市概念”车，后者更注重正常驾驶环境，看起来*稍微*更接近合法上路的车辆。这两类汽车都可以是全电动的，也可以由天然气、柴油、压缩天然气或其他替代燃料提供动力。车辆行驶在一条 0.9 英里的赛道上，这条赛道蜿蜒穿过底特律市中心，每辆车的效率都是在它们绕赛道完成固定圈数后进行测量的。

尽管这些团队中有许多是由拥有大量资金的大学支持的，但团队成员个人的技能对团队的成功有着巨大的影响。我和俄亥俄州的一个团队谈过，他们的电动汽车团队完全由机械工程师组成，他们实际上能够组装一辆功能齐全的汽车。

生态马拉松要求每辆电动汽车都有一个定制设计的电机控制器，这对一个时间有限且几乎没有电气经验的团队来说是一个巨大的挑战。为了尽可能快地启动并运行某些东西，该团队采用了一个 Arduino，并将其连接到一组并行 fet，这些 fet 经过 PWMed 以控制其驱动电机。不幸的是，他们的简单设计最终在比赛中烧毁了一堆 fet，可能是由于栅极驱动不足。尽管如此，该团队还是在比赛结束前让他们的汽车正常工作，并以 109 公里/千瓦时的功耗获得了第 11 名。

![vehicle-inside](img/5460ae7a04c33ad119ccc75beca5510c.png)

相比之下，其他一些团队拥有令人印象深刻的电子设备；围绕微控制器构建的定制车辆控制器，以及相当多的与手机或 Android 平板电脑接口的控制器，通过蓝牙或 USB 显示实时数据。几个团队甚至有网络界面显示来自他们车辆的实时遥测数据。

尽管有相当复杂的电子设备，但大多数车辆都是基于单缸汽油内燃机，并且大多数使用商用发动机控制器。

大多数团队从现成的割草机引擎或类似大小的东西开始。一些团队只是运行引擎库存，而其他人则添加机械或电子燃油喷射，并制造自己的气缸和活塞。配备普通引擎的车队通常表现得出奇的好，因为仅仅在赛车的空气动力学方面就损失了大量的效率。

每辆车的构造都有很大的不同:一些车在管状金属框架周围有简单的设计，而另一些设计是精心制作的复合材料叠层，带有碳纤维防滚架和支撑。一些汽车有汽车质量的油漆工作，而其他人有一个非常粗糙的完成。不管外观如何，我看过的几乎每辆车都有某种令人敬畏的临时拼凑的修复(注意下图中的易拉罐)。

![um-engine-sc](img/632abc108b02aeef174b07beba899961.png)

大多数原型车都有非常符合空气动力学的车身形状，学生们花大量时间进行模拟，以确保它们尽可能高效。车辆阻力的最大来源之一是车轮，所以许多车辆在车轮上有空气动力学罩，或者实际上在车内移动车轮。每个团队都有自己的身体设计，大多数设计都是独一无二的。

尽管这些原型汽车与你在路上可能看到的汽车相去甚远，但这项比赛将学生们聚集在一起，研究和创造节能的机械和电气设计。这些设计可能不会在短期内直接转化为道路上的车辆，但我相信学生们会利用他们对工程和黑客技术的技能和热情，使未来的车辆更加令人敬畏。

想看看比赛的分数，看看有哪些学校参加了比赛吗？越过[前往结果页面](http://www.shell.com/global/environment-society/ecomarathon/events/americas/2015-results.html#iframe-L2RldHJvaXQv)。