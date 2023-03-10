# USB 与以太网转换器的比较:苹果与山寨

> 原文：<https://hackaday.com/2013/03/22/comparing-usb-to-ethernet-converters-apple-vs-knock-off/>

![usb-ethernet-comparison](img/9fb21a74f3b98afe8c53ed04b9c20a88.png)

[Angus Gratton]最近[打开了一对 USB 到以太网转换器](http://projectgus.com/2013/03/anatomy-of-a-cheap-usb-ethernet-adapter/)看看里面有什么。一个是苹果品牌的设备，另一个是来自易贝的无名设备。前者为 30 美元，后者仅为 4 美元。这种类型的比较是我们的最爱之一。苹果产品尤其有趣，因为它们以坚实的硬件选择而闻名，而[山寨产品同样因粗制滥造而臭名昭著](http://hackaday.com/2012/10/10/raspberry-pi-foundation-looks-a-counterfeit-apple-power-supplies/)。

从外面看，这两款设备几乎一样。内部差异从苹果加密狗上的全板金属屏蔽开始，而非品牌加密狗上没有。但是里面的硬件其实挺像的。左边有一个 RJ-45 插孔，旁边是以太网隔离芯片。从那里我们开始看到差异。该品牌有一个空白芯片，苹果的 ASIX AX88772ALF USB 至以太网桥接控制器位于该芯片上。与时钟也有区别；苹果用了两块水晶，而另一块只用了一块。

[via [Reddit](http://www.reddit.com/r/electronics/comments/1an0bj/anatomy_of_a_cheap_usb_to_ethernet_adapter/)