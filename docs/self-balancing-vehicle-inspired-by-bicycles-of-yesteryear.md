# 受昔日自行车启发的自平衡车

> 原文：<https://hackaday.com/2014/11/16/self-balancing-vehicle-inspired-by-bicycles-of-yesteryear/>

[XenonJohn]并不是自动平衡车领域的新手。他是医疗周期团队的成员，也是 Hackaday 奖的半决赛选手。在医疗自行车上的工作暴露了一些改进设计的机会，最重要的是支撑车辆和骑手的单个宽轮。单轮车的设计比双轮车更难学骑。[XenonJohn]想要制造一个改进的自动平衡器，这辆[新的](http://www.instructables.com/id/Raleigh-Chopper-inspired-self-balancing-scooter/?ALLSTEPS)将有两个独立控制的轮子。

虽然成品看起来像是从自行车车架开始的，但自动平衡器的车架实际上是完全定制的。车把和香蕉座是作为老式自行车的配件购买的。为两个车轮提供动力的是一对 24v 有刷电机，每个电机都预先安装了 6:1 的减速齿轮箱。车轮是一个完整的汇编零件不打算去一起。BMX 自行车轮圈被绑在山地车前轮毂上。轮毂有盘式制动器，但[XenonJohn]在那里安装了一个大的齿形滑轮。然后，皮带将驱动电机齿轮箱连接到皮带轮上，完成传动系统。

磷酸铁锂电池套件购自易贝，使用八节电池可输出 24v 和 15AH 的电流。仅这些电池就占了项目成本的很大一部分，将近 300 美元。控制车辆的是 Arduino Mega，它利用了 FreeSix IMU 库。Mega 通过 I2C 接收来自 Sparkfun SEN-10121 板的输入，该板包含加速度计和陀螺仪以及连接到车把上“制动”杆的旋转开关。Arduino 然后向 25 安培的剑齿虎电机控制器发送命令，以保持你在城镇中嗡嗡作响时的平衡。

下面视频。

[https://www.youtube.com/embed/Q4laxhssY8o?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/Q4laxhssY8o?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)