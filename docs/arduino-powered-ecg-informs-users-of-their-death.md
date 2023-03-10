# Arduino 供电的 ECG 通知用户他们的死亡

> 原文：<https://hackaday.com/2014/02/13/arduino-powered-ecg-informs-users-of-their-death/>

就在你认为你已经看到 Arduino 做所有事情的时候，[birdyberth]建造了一个由 Arduino 供电的心电图(心电图或 EKG)。[心电图](http://en.wikipedia.org/wiki/Electrocardiography)是一种研究心脏的非侵入性方法。对于我们中的许多人来说，这意味着在我们每年的体检中有 10 分钟的测试。医用级心电图最多可使用 10 个电极。为了简单起见，[birdyberth]走了我们在之前[见过的](http://hackaday.com/2011/08/03/diy-propeller-based-ecg/)[几个电路](http://hackaday.com/2013/07/09/a-handful-of-parts-used-to-form-an-electrocardiogram/)的路线，并将其简化为两个电极和一个接地参考。[birdyberth]指出，只有使用电池电源时，电路才是安全的。

任何心电图的“心脏”都是一个仪表放大器。仪表放大器可以被视为超差分放大器。它们具有缓冲输入、低 DC 失调、低漂移、低噪声、高开环增益和高阻抗等有利特性。缺点是成本。一个典型的运算放大器单件价格可能为 0.50 美元。仪表放大器，像[birdy berth]的[in 128](http://www.ti.com/product/ina128)可以花费 8.30 美元或更多。考虑到要测量的信号，额外的成本是可以理解的。心电图从外部皮肤上“拾取”心脏的电信号。在常用的心电图纸上，1 毫米见方相当于 0.1 毫伏。这里要获得任何有意义的数据，确实需要高增益和干净的信号。

电极是心电图的另一个重要部分。医疗级 ECG 设备通常使用一次性粘合电极，与皮肤形成强有力的电连接，当护士将其扯掉时，会非常疼。[birdyberth]只用锡纸和回形针就能制造出电极。我们认为真正的诀窍在于他用来与皮肤建立电连接的沐浴露。虽然很脏，但这种凝胶为微小电流的流动提供了一个低阻力的路径。

[birdyberth]电路中的实际处理过程很容易理解。来自仪表放大器的信号通过低通滤波器、741 运算放大器发送，然后到达 Arduino。Arduino 使用 16×2 LCD 显示心率，以每分钟心跳数为单位，同时还有一条友好的消息通知您是活着还是死了。当用户断开电极或呼气时，该电路甚至提供心跳的听觉反馈和经典的“扁平线音”。[birdyberth]还在低通滤波器后插入了他的袖珍示波器。正如他的视频所示，熟悉的心电波形清晰可见。我们希望看到这个黑客结合[【阿迪的】心脏模拟器](http://hackaday.com/2013/07/27/heart-shaped-heart-simulator/)的更复杂版本，这样我们就可以实时准确地知道哪种心脏疾病正在杀死我们！

[https://www.youtube.com/embed/85wpkerNxlk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/85wpkerNxlk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[https://www.youtube.com/embed/LoiXVOTI4CI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/LoiXVOTI4CI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)