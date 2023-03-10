# 树莓 Pi 比特币矿工

> 原文：<https://hackaday.com/2013/06/23/turning-the-raspberry-pi-into-a-bitcoin-miner/>

开采比特币正在成为一件徒劳的事情，但总会有一些新的硬件出现，让那些铁杆矿工保持领先地位。一种这样的硬件是新的定制 ASIC 设备，其速度与 FPGA 一样快，但价格低得多。许多这类 ASIC 器件采用有趣的封装，看起来就像一个大的 USB 拇指驱动器。当然，这是一个完美的机会来展示树莓 Pi 可以做什么，它可以以与当今采矿中使用的最佳图形相当的速度挖掘比特币。

树莓派根本没有足够的马力以任何有价值的速度开采比特币。然而，有 [USB ASIC 设备](https://www.bitmit.net/en/item/39574-bitcoin-asicminer-block-erupter-usb-asic-333mhash-2-5w-miner)会以和高端显卡差不多的速度为你挖矿。由于可以通过 USB 集线器控制多个 ASIC 设备，所以只需将 USB 集线器插入 Raspberry Pi，加载 [CGminer](https://bitcointalk.org/index.php?topic=28402.0) ，并让您的新 PiMiner 在采矿池上自由移动。

Adafruit Pi Miner 使用一个非常酷的 [LCD 字符显示器和键盘](http://learn.adafruit.com/adafruit-16x2-character-lcd-plus-keypad-for-raspberry-pi/overview)来显示当前的采矿率、接受的份额和足够的信息，以便您计算使用 Pi 驱动的采矿钻机需要多长时间才能实现收支平衡。这四个设备的钻机需要多长时间，我们将留在评论部分。