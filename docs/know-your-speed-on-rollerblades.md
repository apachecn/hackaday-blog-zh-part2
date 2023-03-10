# 知道你的速度

> 原文：<https://hackaday.com/2015/02/12/know-your-speed-on-rollerblades/>

是一名计算机工程专业的学生，擅长滑旱冰。轮滑鞋不是一种通常装有速度计的交通工具，所以[Anurag]认为这是一个挑战，并设计了这台由 Arduino 驱动的计算机，以给他更多关于他的轮滑鞋骑行的信息。

该设备使用 Arduino 作为大脑，并计算车轮转数(以及做一点数学计算)，以计算骑手的速度。使用这种方法的唯一问题是轮子不是一直在地面上，当骑手的脚离开地面时会稍微慢下来。为了确保获得准确的数据，Arduino 使用超声波测距仪来确定到地面的距离，并推断出何时应该进行速度测量。

除了速度，该设备还可以计算湿度和温度，并可以配置为测量任何数量的东西。它将结果输出到一个小屏幕上，但它可以很容易地通过蓝牙升级，以方便数据记录。如果速度真的是你的目标，你可能也想看看这些电动直排轮。