# 网络控制装饰 led 矩阵框架

> 原文：<https://hackaday.com/2014/06/21/network-controlled-decorative-led-matrix-frame/>

没有比展示给所有人看的项目更好的了。[特里斯坦]的最新项目是一个[装饰 LED 矩阵框架](http://www.viesurip.fr/en/2014/06/17/un-cadre-en-couleurs/)，包含 12×10 大正方形像素，可以显示任何颜色，真的很酷。

这个项目是围绕一个便宜的宜家相框建造的，非常可行，至少对那些有 3D 打印机的人来说。3D 打印机需要创建像素网格，最终在最终帧中看起来非常干净。从电子学的角度来看，主要组件是一组 [Adafruit Neopixel LED 灯条](https://www.adafruit.com/products/1461)，和一个 [Arduino Uno](http://arduino.cc/en/Main/arduinoBoardUno) 带[以太网屏蔽](http://arduino.cc/en/Main/ArduinoEthernetShield)。主控制器甚至包含一个备用电池，用于在拔出帧时的实时时钟(RTC );不错的接触。鉴于框架连接到本地网络，[Tristan]设计了一个简单的 HTML5 接口来控制框架(代码可从 [GitHub](https://github.com/twisterss/CadreCouleurs/tree/master/cadre/web) 获得)。这允许任何本地连接的设备控制帧。

请务必检查建设细节，他们做得非常好。如果你仍然不相信这个项目有多酷，休息之后一定要看看它的视频！这让我们希望你能在这个画面上玩俄罗斯方块。非常好的工作[特里斯坦]！

[http://www.dailymotion.com/embed/video/x1zonmc](http://www.dailymotion.com/embed/video/x1zonmc)