# 哈尔是家庭自动化的管道胶带

> 原文：<https://hackaday.com/2014/05/31/hal-is-duct-tape-for-home-automation/>

![HAL Home Automation](img/c7a43b113e7ad52a216c209cd4e579ea.png)

谈到家庭自动化，有很多不同的产品做不同的事情。很多都是不同公司做的，在一起也不经常玩的很好。这种挫败感最终促使[Daniel]开发他自己的基于 Python 的中间件解决方案，让这些不同的组件作为一个单一的[内聚系统](http://nordness.net/posts/hal "HAL Home Automation")工作。[丹尼尔]到底想控制什么？

首先是门锁。[丹尼尔]住在公寓楼里，所以实际上有两把锁。首先，访客必须按下公寓内部通话系统上的按钮才能进入大楼。第二，公寓的门有自己的死栓锁，需要打开和关闭。[丹尼尔]能够控制大楼的前门，只使用一个连接到 Arduino 的晶体管来模拟物理按钮的按压。原来的按钮仍然完好无损，所以(丹尼尔)仍然可以很容易地“嗡嗡”访客。

公寓的死栓有点棘手。有现成的解决方案来控制死栓，但它们通常很昂贵。[丹尼尔]建立了自己的解决方案使用一个简单的伺服电机栓在门上。伺服系统是由 Arduino 控制的，而 Arduino 又是通过公寓里已经存在的两个坏了的对讲机按钮来控制的。这些按钮最初是用来在访客进入大楼前和他们说话或听他们说话的。他们从未为[丹尼尔]工作过，所以他将他们重新用于自己的项目。整个 DIY 门柜都封装在一个定制的激光切割木盒里。

点击休息时间观看[Daniel]故事的其余部分。

谈到照明，[丹尼尔]在他的公寓里有几个不同品牌的自动灯泡。一个品牌的灯泡是由无线电频率信号控制的。该品牌配有一个转换器盒，可以通过 WiFi 接受照明命令。它还使用了一个简单的 API，允许[Daniel]从他的 Python 代码中轻松控制所有的灯泡。第二个品牌的灯泡没有简单的 API。在四处搜索之后，[Daniel]找到了一个名为 [ouimeaux](https://github.com/iancmcc/ouimeaux "oiumeaux") 的开源项目。Ouimeaux 是一个 Python 库，允许你控制这个特殊品牌的自动化灯泡。这对[Daniel]来说是完美的，因为他已经在他的项目中使用 Python 了。有了这个库，他从网络界面控制灯光就变得轻而易举了。

作为概念验证，[Daniel]还使用 [SparkCore](http://spark.io/ "SparkCore") 模块构建了一个定制的支持 WiFi 的电源插座。他在 T2 有一个独立的职位专门负责这个项目。

对于系统的大脑，[丹尼尔]选择使用树莓 Pi。Pi 使用基于 Flask 的后端系统运行 web 服务器。Flask 允许他用 Python 编写网站代码，这意味着他可以轻松地编写一个可以与各种自动化组件交互的网站。Pi 可以使用各种 Python 库直接与所有现成的组件通信。对于门锁，Pi 通过 [pySerial](http://pyserial.sourceforge.net/ "pySerial") 与 Arduino 通信。[Daniel]还使用了 [Flask OAuth](http://pythonhosted.org/Flask-OAuth/ "Flask OAuth") 来限制只有授权用户才能访问系统。现在每当[丹尼尔]想为来访者开灯或开门时，他所要做的就是按下网页上的一个按钮。

[via [Reddit](http://www.reddit.com/r/raspberry_pi/comments/26pj3h/crosspost_from_rarduino_i_built_a_webmanaged/ "Reddit.com")