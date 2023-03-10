# 会说话的培根在门口迎接你

> 原文：<https://hackaday.com/2014/03/21/talking-bacon-plushie-greets-you-at-the-door/>

![BaconMaterials](img/d1bb9f76fc60d36599de692dfd2e4ce2.png)

[gTar]的人们决定创造一个[动作激活的会说话的培根毛绒玩具](http://blog.incidentgtar.com/hack-plush-talking-bacon-toy/)来迎接来到他们办公室的访客。

他们从一个名为“我的第一根培根”的玩具开始，这个玩具可以从 ThinkGeek 上获得，它是一个毛绒玩具，会大叫“我是培根！”当你挤压它的时候。但是他们把他切开了。我们无法想象这个可怜的有自知之明的培根心里在想些什么！

黑客本身非常简单。他们基本上是用红外运动传感器取代了“挤压”电路，准确地说是 SparkFun 的 PIR 传感器。除此之外，他们还需要一个小型反相器 IC。这是因为标准的 talking bacon 模块需要一个正前沿信号来触发音频输出，他们的 PIR 传感器将输出引脚驱动到低电平，只需轻轻一拍反相器 IC(他们有一个旧的施密特触发器)，您就可以开始工作了！

为了减少运动传感器的感应面积，他们用纸巾卷将它稍稍嵌入【培根】体内。在[培根]的肚子上小心翼翼地打了一个洞，一个熟悉的白色地球仪稍微突出来，提供了一个狭窄的运动感应功能——正好可以捕捉到走进办公室的人。

[https://www.youtube.com/embed/SP8VZaKdQLM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/SP8VZaKdQLM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[https://www.youtube.com/embed/Pl9ivaU8H38?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/Pl9ivaU8H38?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)