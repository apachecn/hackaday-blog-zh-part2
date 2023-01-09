# 派遣无人机:给物联网装上轮子和翅膀

> 原文：<https://hackaday.com/2015/07/17/send-in-the-drones-putting-wheels-and-wings-on-the-internet-of-things/>

想象你是一个农民，试图在干旱条件下种植作物。最新的土壤湿度数据可以帮助您决定何时何地进行灌溉，这将直接影响您的作物产量和利润。更多的传感器意味着更多的数据和更好的状况空间图像，但是有线土壤传感器的成本会非常高。接入 GSM 或某种网状网络的无线传感器会更好，但每个传感器仍需要电源，维护成本也会迅速攀升。但是如果你能在你的田地里部署大量廉价的 RFID 连接传感器会怎么样呢？如果自动驾驶汽车可以负责轮询传感器和报告数据的工作，会怎么样？这是最近一篇关于移动物联网的学术论文中设想的一个场景。

[![both](img/d2d252ff6d53b0bfd4a9c0a2dab973ee.png)](https://hackaday.com/wp-content/uploads/2015/07/both.jpg)

在这篇论文中，作者[Jennifer Wang]、[Erik Schluntz]、[Brian Otis]和[Travis Deyle]对商用四轴飞行器和遥控汽车进行了研究。两个平台都配备了遥测无线电、GPS 和现成的 RFID 标签阅读器和天线。对于他们的传感器阵列，他们选择了耦合到许多不同传感器的无源超高频 RFID 标签，包括用于测量土壤湿度的电阻传感器。开发了一个地面控制系统，允许四轴飞行器和汽车在 GPS 引导下机动到航路点，以轮询传感器并返回报告。

除了农业，基于廉价传感器和自动驾驶汽车的物联网轮询它们的可能性是无限的。作者正确地指出了基于这些原则构建商业系统的挑战，但通过从 COTS 组件开始并努力将安装成本保持在最低水平，我们认为他们在这里已经做了很好的概念验证。