# 基于高速激光的相机闪光灯触发器仅售 2 美元

> 原文：<https://hackaday.com/2014/07/19/high-speed-laser-based-camera-flash-trigger-for-only-2/>

[Matt Kane]在英国一家非常酷的公司工作，他最近完成了 Triggertrap Ada 的工作，这是目前性能最高、功能最丰富的相机触发器。为了好玩，他决定再次挑战自己——他能不能做一个超基础、**超快、**裸机[相机触发器，售价 2 美元？](http://www.vela.io/posts/building-a-laser-camera-trigger-for-2-dollars/)

在最基本的层面上，这只是一个激光笔和一个光传感器。当你拍摄的物体挡住光路时，闪光灯就会触发。通常，这是用红外激光器完成的，但由于他打算使用低成本系统，他将使用基本的 1mw 红色激光指示器，唯一的缺点是您可能会在图片中看到它。

接下来是传感器。理想情况下，我们会使用速度非常快但价格昂贵的光电二极管。光敏电阻很便宜，但是不够快。介于两者之间的一个很好的媒介是光电晶体管，它相对较快，而且便宜。最后，我们需要一个最小触发周期来抵消闪光。[Matt]考虑使用 555 定时器，但是决定只产生一个 45 的脉冲。

添加几个电阻，将它们一起放在试验板上，只需 1.44 美元，他就拥有了一个超级实惠、功能强大的相机闪光灯触发器！看看这支用 BB 枪拍摄的爆炸蜡笔！

![Slow motion crayon destruction](img/8ef4eefa8b0d49d049c4c4ae838b6b51.png)

这当然也可以使用 Arduino 创建[来获得类似的结果。](http://hackaday.com/2009/06/19/arduino-camera-laser-trigger/)