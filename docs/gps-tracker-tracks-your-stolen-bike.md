# GPS 追踪器追踪你被盗的自行车

> 原文：<https://hackaday.com/2014/09/02/gps-tracker-tracks-your-stolen-bike/>

自行车非常适合在拥挤的城市中巡游，但是骑着你的两轮车到处跑有一个严重的缺点……自行车失窃。这是一件大事，例如，纽约市每年被盗的自行车估计在 60，000-100，000 辆之间。其中只有极小一部分被找到。[stbennett]刚刚给自己买了一辆还过得去的自行车，他对被偷不太感兴趣，如果它被偷了，他想找到它，所以他给自己的自行车装了一个[GPS 跟踪器。](http://www.instructables.com/id/DIY-GPS-Tracked-Bike-Lock/all/?lang=es)

整个项目是基于 Arduino 的。它使用了一个 GSM 屏蔽和一个 GPS 模块，以及一些其他小零碎。2 芯 LiPo 电池为所有组件提供所需的电力。这款设备保持超长电池寿命的方式非常巧妙。自行车锁的金属电缆被用作电路中的导体。当电缆插入锁壳并锁定时，电路就完成了，防止电流通过晶体管传到 Arduino。换句话说，Arduino 是关闭的，除非自行车电缆被切断或断开。这样，它就不会 24/7 全天候运行，也不会耗尽电池。

整个系统是这样工作的，一旦自行车锁电缆被切断，Arduino 就会醒来，并在做任何事情之前给出 15 秒的延迟，允许合法用户重新连接自行车锁并关闭警报系统。如果自行车锁没有重新接合，该单元开始寻找 GPS 信号。在那时，它将发出带有 GPS 位置坐标的 SMS 消息。将这些数字输入谷歌地图，你就能知道自行车的确切位置。

当然，你的另一个选择是把你的自行车停在别人无法接近的地方，比如灯柱顶端。