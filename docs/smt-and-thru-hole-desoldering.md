# SMT 和通孔脱焊

> 原文：<https://hackaday.com/2014/08/21/smt-and-thru-hole-desoldering/>

20 世纪 80 年代初，我在宾夕法尼亚州莱奥拉市的宾夕法尼亚秤公司担任生产技术员，开始接触电子制造。我了解到，要做我想做的事情，我必须在中午前后完成分配给我的任务。作为一名电视修理工，我学到的最重要的一课，除了不要去啃高压电缆，就是先用你的眼睛。我会拿一盒坏的 PCB，基本上是基于 6502 的计算机，可以计数和称重，首先检查它们；通常这样做内容会减少 50%。然后，这是一场识别和修复剩余部件的比赛，为了跟上我的步伐，我必须自己拆焊。

[![Desoldering with IR System](img/3e5dfd7c42885d85d9f559c2db7ec15f.png)](https://hackaday.com/wp-content/uploads/2014/08/ir-lift.jpg)

Desoldering with IR System

它是这样工作的:你可以用指令把单元放在一边，然后生产人员会在某个时候改变组件等等。或者你可以让自己变得孤独。我很擅长用一个古老的 Soldapulit 手动焊钳(众所周知)手工拆卸 28 和 40 引脚芯片。但是要真正烹饪的话，我会等一会儿生产去焊锡机出来。使用拆焊站有一个简单的规则:完成后清理干净！如果做不到这一点，你将会被暂停进入空间站，然后你也可能会招致“生产的愤怒”,这不仅仅是因为你的午餐袋被发现冻成了固体，或者你的椅子被浸泡在去焊剂的化学物质中。

[https://www.youtube.com/embed/VSzXqaJKVJ0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/VSzXqaJKVJ0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

有一件事是我从来都买不起自动去焊台…直到现在。我发现海外和易贝有各种各样的工作站可以模仿他们的产品质量，我在这里展示了一个基于真空的脱焊站，一个基于红外加热的站，以及一些其他工具，如热空气和脱焊镊子。

### 真空脱焊

[![Automatic Desoldering Station utilizes a vacuum to remove solder.](img/16d990a85bdf4062f97e409934c2cbf6.png)](https://hackaday.com/wp-content/uploads/2014/08/auto-desolder.jpg)

Automatic Desoldering Station utilizes a vacuum to remove solder.

基于真空的通孔脱焊站由具有中空尖端和主体的烙铁组成，该烙铁通向玻璃管，该玻璃管在一端被过滤器覆盖，该端也是施加真空的端。诀窍是加热整个焊点(我用了大量的助焊剂来辅助)，然后扣动扳机开始抽真空。在此期间，我还扭动烙铁头，以便将元件引脚从孔或板通孔的壁上断开。如果操作正确，被拆除的 PCB 和元件都可以重复使用。

### 红外线脱焊

基于红外线的系统，被制造商称为红外线焊接机，可以最终将一个较小的区域加热到比热空气更高的温度，或者我是这样认为的。为了屏蔽周围区域的热空气，您需要保持低气流，并使其远离 PCB 的其余部分。为了改变红外线的方向，你可以利用铝箔的反射特性。接下来最重要的事情就是启动排气扇，耐心等待直接加热完成工作。再次，明智地使用通量有所帮助。

[![IR Desolder System for removing larger SMD](img/83ac5230ebef02c637620212d4372c8a.png)](https://hackaday.com/wp-content/uploads/2014/08/ir-desolder1.jpg)

IR Desolder System for removing larger SMD

### 热空气脱焊

热空气也有类似的作用，因为助焊剂会有帮助，可能会有烟雾，你必须耐心等待零件完全松开——半松开是不行的。为此，我推荐一个热风固定器、一个排气扇和一个鸡蛋计时器。如果你没有鸡蛋计时器，我敢肯定某个地方有一个应用程序。

[![Desoldering SMT with Chip Quik](img/643eb529e80b6a4703b48d04c7f60f25.png)](https://hackaday.com/wp-content/uploads/2014/08/smt-de-solder1.jpg)

Desoldering SMT with Chip Quik

### 用快速烙铁和烙铁脱焊

我发现，在不投资任何此类设备的情况下，解除焊接 SMT 的最快方法是使用像 [Chip Quik](http://www.chipquik.com/) 这样的产品，当与焊料金属混合时，它会降低焊料金属的熔点，因为它允许烙铁熔化整个芯片的覆盖区，同时允许将其移除。

[![Solder Sucker, Solder Wick, Chip Quik](img/e86ca60ebd48027fa40e8e88a090e9b5.png)](https://hackaday.com/wp-content/uploads/2014/08/manual-desolder.jpg)

Solder Sucker, Solder Wick, Chip Quik

### 脱焊镊子

最后是镊子。你不需要这些…我当然不需要。但管它呢，当用两个烙铁移除一个有两个引脚的部件时，这种运动有一定的清洁度。哦，是的…首先是大量的焊剂。

[![Desoldering Tweezers](img/268d21d49b69f8cd574cfdf893911166.png)](https://hackaday.com/wp-content/uploads/2014/08/tweezers.jpg)

Desoldering Tweezers

回到故事:四年后，我已经成为当时最好的家用电脑公司的首席设计工程师之一。我们有严格的截止日期，就像拉斯维加斯的 CES 展会，当我们还有 3%的产品要完成时，这是不可避免的。可以肯定的是，能够快速脱焊，更重要的是*而不损坏*不可替代的原型芯片和电路板，是凌晨 2:00 时一项不可或缺的技能，任何头脑正常的技术人员都会在家躺在床上，而不是为他办公室里的床是气垫的工程师拉芯片。我们从未错过一次消费电子展。