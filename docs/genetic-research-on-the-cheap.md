# 廉价的基因研究

> 原文：<https://hackaday.com/2012/09/09/genetic-research-on-the-cheap/>

[![](img/5589faf5038551324816ccaac497045e.png "OpenPCR")](http://hackaday.com/?attachment_id=84652)

当你想到 DIY 硬件时，通常不会想到基因研究工具。但是[Stacey]和[Matt]的[open PCR](http://www.instructables.com/id/Arduino-PCR-thermal-cycler-for-under-85/ "OpenPCR")项目旨在让任何人都能以低廉的成本进行[聚合酶链式反应](http://en.wikipedia.org/wiki/Polymerase_chain_reaction "Polymerase chain reaction - Wikipedia")(PCR)研究。

PCR 是一个将特定的 DNA 片段复制几百万次的过程。它可以用于许多目的，包括 DNA 克隆和 DNA 指纹取证。PCR 也用于亲子鉴定。

这个过程包括在特定的温度下烘烤 DNA 适当的时间。DNA 首先变性，将螺旋分裂成单股。接下来，降低温度，引物结合到链上。最后，另一个温度被用来让[聚合酶](http://en.wikipedia.org/wiki/DNA_polymerase "DNA Polymerase - Wikipedia")复制 DNA。重复这个过程来繁殖 DNA。

OpenPCR 使用 Arduino 来控制固态继电器。该继电器向两个充当加热器的大电阻供电。A [MAX31855](http://www.maximintegrated.com/datasheet/index.mvp/id/7273 "MAX31855") 用于通过 SPI 读取热电偶，并为系统提供反馈。电脑风扇用于冷却设备。

在循环过程中，铝制样品架容纳并加热样品。激光切割，t 型槽结构的情况下具有一些螺旋艺术，并容纳所有的组件。看看这个 85 美元的 PCR 设备能做什么应用将会很有趣。

通路〔t0〕adafruit〔t1〕