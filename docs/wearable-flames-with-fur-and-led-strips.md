# 带毛皮和 LED 灯条的耐磨火焰

> 原文：<https://hackaday.com/2014/04/16/wearable-flames-with-fur-and-led-strips/>

![wearable-flames-with-fur-and-LED-strips](img/c32a4ac0c6be0c34c6407c2c17b9ee45.png)

在今年的火人节上，一个黑客项目的负责人制作了一件非常棒的毛茸茸的 LED 背心来保暖和照明。他正在使用一个 [Teensy 3.0](http://www.pjrc.com/store/teensy3.html) 来驱动 470 WS2811 LEDs 灯条。

垂直对齐的条带在连续序列上运行，使用预编译的动画每秒可达 31 帧。在处理或视频映射中渲染的效果被逐帧捕获，并作为原始颜色数据存储到 SD 卡中。回放使用[新像素库](https://github.com/adafruit/Adafruit_NeoPixel)来控制条带。高分辨率的发光二极管，加上视频映射的火焰和长毛绒，创造了我们在服装上见过的最好的火焰效果之一。

我们还看到 Teensy 3.0 和 WS2811 LEDs 作为一种流行的组合用于[建造巨大的显示器](http://hackaday.com/2013/02/25/building-huge-displays-with-led-strips/)、[23 英尺高的金字塔](http://hackaday.com/2013/09/13/a-23-feet-tall-pyramid-with-0-31-mile-of-led-strips/)，以及最近在 Make Fashion 2014 的 [RFID 夹克中。你有没有做过或看过一个很棒的 Teensy/WS2811 项目，想和我们分享一下？如果是这样，请在下面的评论中告诉我们详情。](http://hackaday.com/2014/03/04/rfid-jacket-flashes-the-crowd-at-make-fashion-2014/)

[https://player.vimeo.com/video/87988933](https://player.vimeo.com/video/87988933)