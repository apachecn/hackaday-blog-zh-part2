# 逻辑噪声:硅中的时序控制

> 原文：<https://hackaday.com/2015/04/24/logic-noise-sequencing-in-silicon/>

在这一节逻辑噪声课中，我们将把迄今为止制作的一系列模块组合成一个自主的机器噪声盒。好吧，至少我们会开始对这些声音进行排序。

音序器是任何鼓盒的核心，也是任何“严肃”模块化合成器的核心。为什么？因为你不能同时调整所有的旋钮，弹奏音符和跳舞。或者至少我们不能。所以你必须自动化。以前我们是用[开关](http://hackaday.com/2015/02/23/logic-noise-the-switching-sequencer/)来完成的。这次我们用逻辑脉冲来做。

[https://www.youtube.com/embed/rEBHZxlYFDs?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/rEBHZxlYFDs?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

## 4017 十进制计数器

本次会议的特色芯片是 4017 十进制计数器。这是一个奇怪的芯片，是人们希望使用 IC 逻辑芯片计数而不是仅仅将输入输入到微控制器的时代遗留下来的。但这正是它的魅力和可用性所在。

![4017_pinout](img/e6ee0504fa44f1ca07d6d4c98f20532b.png)

最简单的方法是，输入一个时钟信号，十个不同输出(Q0-Q9)中的一个被设置为高电平，而其他的都为低电平。在时钟的下一个上升沿，下一个输出设为高电平，前一个输出设为低电平。这种情况一直持续到计数循环结束。

使 4017 非常有用的一个特性是复位引脚。当复位时设置高电压时，第一个输出(Q0)设置为高电平，所有其他输出归零，芯片再次从零开始计数。这里很酷的一点是，你可以将 reset 引脚连接到一个 Q 输出，一旦到达该输出，计数器就会自动复位。例如，如果 reset 连接到 Q2，计数将变为 Q0，然后是 Q1，然后立即再次复位回到 Q0:Q0，Q1，Q0，Q1…如果你想要一个八进制(除以八)计数器，你只需将 reset 引脚连接到 Q8。

![4017_timing](img/7250319dcf9dacf51cd53ac7cc89e4e9.png)

八步挺标准的(无聊？)并且可以通过选择奇数序列长度来获得漂亮的凹槽图案。但是，如果你想要你的标准鼓机，挂钩复位到 Q8 是一条路要走。

查看时序图，注意 reset 引脚也可以异步使用。也就是说，一旦 reset 线变为高电平，芯片就会复位，而不会等待当前时钟周期结束。例如，在时钟步骤五(在 Q4 上)仍然有效时，我们点击了 reset。

异步复位意味着你的复位源可以来自 4017 芯片及其计数器之外。例如，你可以通过一个按钮将重置线连接到 VCC，并随意重置序列。(如果这样做，请考虑在 reset 线上设置一个下拉电阻，以便在按钮未被按下时保持明确的电压电平。)

还剩下两个别针。当 Q0-Q4 为高电平时,“执行”引脚为低电平，当 Q5-Q9 为高电平时为高电平。当芯片数到 10 时，就会产生一个漂亮的方波，每 10 次计数就有一个周期。顾名思义，这可以馈入另一个 4017 的时钟输入，你将有一个数到 100 的设备。将下一次执行链接到第三个 4017，您可以计数多达 1000 个时钟脉冲。(如果你真的在计数的话，把所有的复位线绑在一起一次归零。)执行对我们来说没那么有用，但不管怎样，下节课我们会稍微讨论一下。

最后，还有“抑制”引脚。在 4017 芯片的大多数实现中，将 inhibit 设为高电平会使芯片忽略输入的时钟脉冲。一些制造商的芯片有一些稍微聪明一点的逻辑，如果“时钟”线保持低电平，“禁止”线切换，禁止线可以两用，以计数高到低的转换。我们不会使用这一功能，所以只需记住将抑制线(引脚 13)接地，这样就不会出现毛刺。

回到重要的事情上。我们有一个芯片，它会在一个接一个的引脚上输出逻辑电压信号，可时钟控制，可复位。这是一个简单序列器的核心。在本次会议中，我们主要是让这些电压阶跃与我们的快速 CMOS 逻辑合成器模块配合良好。

## 基本序列器

我们将在本次会议中构建的音序器只不过是一个由基于 40106 的振荡器计时的 4017，该振荡器以“速度”频率而不是音频速率运行。事实上，你可以就此打住。但对于另一个 4017 逻辑芯片，一些 led 和电阻的低，低价格，你可以有一些豪华的东西。

[https://www.youtube.com/embed/5linx91sLbk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/5linx91sLbk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

我们这个简单的序列器版本将由两个 4017 构建而成，它们之间有共同的时钟和复位线。这意味着两个 4017 将会一直同步运行。我们可以用一个 4017 驱动我们的 synth 器件，另一个驱动 10 个状态 led，而不必担心 led 在汲取太多电流时会拉低输出电压。

![dual_4017s.sch](img/826a755206826ac206567d4ba11657f8.png)

当然，如果你不想要 led，你可以从电路中完全省略第二个 4017。或者，如果你觉得幸运的话，你可以直接把发光二极管挂在信号输出端。但由于我们已经要求 4017 的电流比它们的设计电流多一点，我们认为为了保险和方便，额外的芯片是值得的。此外，它使试验板上的布局更加整洁。

## 用 4017 序列器选通振荡器

用音序器做的第一件事可能是弹奏一堆音符。用我们目前的设置，最快也是最脏的方法是为你想演奏的每个音符构造一个振荡器，然后只有当 4017 的相应“Q”输出设置为高时，振荡器才发出声音。这应该很容易，事实也的确如此。

如果你还记得我们的第一次[会议](http://hackaday.com/2015/02/04/logic-noise-sweet-sweet-oscillator-sounds/)，我们用一个二极管通过选通一个振荡器来创建一个硬同步振荡器声音。回想一下，振荡器都是通过反馈电阻给电容充电来工作的，因此，如果你能排出足够的电流来防止电容充电，你就可以让振荡器静音。

![4017_and_oscillators.sch](img/710146c7ed0379bc5f3af6ff4d5b5b1e.png)

首先看右上方的单音频振荡器，通过输入“A”连接到 4017。当相应的 4017 输出为低电平时，通过反馈电阻(RV2)给电容(C2)充电的任何电流都会被二极管(D1)吸入 4017，振荡器不会振荡。当 4017 的输出为高电平时，二极管截止，振荡器自由工作。轻松搞定。

## 二极管或门

但是如果我们想要一个音符触发多次呢？这里有一个很方便的接口技巧，叫做“米老鼠”逻辑或者更形象的说法，二极管逻辑。其思想是，你可以用一个上拉或下拉电阻来设置所需的默认逻辑状态，然后用通过一组二极管输入的信号来覆盖它。要向或添加更多输入，您只需向电路添加更多二极管，这在您需要七路或函数等奇怪功能时非常有用。

![diode_or.sch](img/f32129a1ce830ce4550eabeaf73969cc.png)考虑完整原理图中的输入 B、C 和 D。当 B、C 或 D 都不是高电压时，二极管(D2-D4)都不导通，下拉电阻(R3)将进入二极管 D5 的电压设置为低，将电流从振荡器中拉出，使其停止工作。当 B、C 或 D 中的任何一个为逻辑高电平时，4017 将通过相应的二极管将电流输出到与电阻的连接点。当这个点为高时，二极管 D5 不导通，振荡器运行，就像上面的单步版本一样。

为什么是二极管 D2-D4？如果 4017 的一个阶段是高的，比如说 B，其他两个阶段一定是低的。如果电路中没有二极管，我们就会将 4017 的两个引脚短接在一起，所有关于标有“二极管 OR”的结点电压的打赌都将落空。这些二极管防止 4017 的一个引脚与另一个引脚发生冲突。

选择二极管或电路中的电阻值有点关键。它需要具有足够低的电阻，以便能够下拉振荡器电路。因此，R3 需要小于调谐振荡器的可变电阻(RV3)的值。但是 R3 需要足够大，以便当 4017 将其高电压推过输出二极管时，结处的电压上升到足以阻挡二极管 D5。

4017 的额定输入或输出驱动电流仅为 3 毫安，电源电压为 10 伏，而电源电压为 5 伏时仅为 1 毫安，这意味着如果我们希望二极管或结处的电压高于 VCC/2，则应使用不小于 2.2 千欧的下拉电阻作为下拉电阻。使用更大的有助于降低 4017 上的电流需求。

事实上，正是这种对 4017 提供大量电流的要求促使使用第二个 4017 来处理 led。我们的 4017 数据手册只规定了连接到 10V 电源的 3 毫安输出驱动或吸电流。(在 5V VCC 电压下，这一电流降至 1 毫安。)对于 led 上的 1K 电阻，我们可能已经消耗了 5 到 10 毫安的电流——远远超过了芯片的额定电流。给单个 4017 芯片增加更多负载来驱动二极管或甚至更多输出是自找麻烦。你可以想象缓冲 4017 的每个输出，但在某些时候，更容易将另一个 4017 扔进设计中。

无论如何，撇开技术细节不谈，这是处理音序器对单个振荡器的控制。我们已经了解了如何从多个序列器级运行一个振荡器。每个 40106 芯片有六个振荡器，你应该能够用最少部件做出合理的旋律。

[https://www.youtube.com/embed/02P2mTz7rug?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/02P2mTz7rug?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

## 门触发脉冲电路

现在是时候推动我们的打击乐器了。如果你还记得我们 [Cowbell 会议](http://hackaday.com/tag/logic-noise/)中的双二极管 VCA，我们实际上构建了一个“栅极触发”转换器。在 modular synth 行话中,“门”信号是一个逻辑信号，只要(例如)一个键被按下，它就保持高电平，然后当它被释放时，它立即回落到低电平。4017 的单个输出看起来很像门信号——每个输出在其完整的阶跃期间且仅在其阶跃期间为高电平。另一方面，cymbal 的衰减幅度电路在阶跃开始时需要一个快速脉冲，称为“触发”信号。

![diode_vca_interface.sch](img/e41ed6b51d6fa9b8ebe8ff6f4d80cba3.png)

栅极到触发器电路的核心是一个电容(C1)。电容器一侧的电压变化会让一点电流通过，直到电容器充电到足以抵抗进一步的电流。这将我们的门信号的前沿和后沿变成正负尖峰脉冲。

我们选择使用二极管(D5)只通过正电压尖峰。剩下的问题，我们在牛铃会议中忽略了，是负尖峰信号没有通过 D5。事实上，如果电路中没有从地(D7)指向上的二极管，电容 C1 的右边极板将会卡在相对于地的负电压上。从左侧的 4017 发送的额外正脉冲可能会将电压提高到零伏，但肯定不足以通过二极管 D5 并发出声音。简而言之，你会有一次成功，然后你就再也听不到它了。

从地向上的二极管(D7)通过在每个负尖峰之后将 C1 的右侧充电到至少小于 0V 的二极管压降来防止这种情况。这使得门到脉冲电路的工作有点像泵；当电荷从 4017 侧通过电容器时，它通过 D5，当电荷以另一种方式被拉回时，它通过 D7“止回阀”从地获得。

如果你买那个类比，剩下的钹接口电路应该就清楚了。左手边的二极管或允许多个钹敲击。同样，下拉电阻的选择很重要，但这里对它的要求很低。电阻器 R2 仅负责在击中之间对电容器 C1 的左侧进行放电。如果您运行的是快速序列，请尝试较低的值。

[https://www.youtube.com/embed/6OuF128u1VY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/6OuF128u1VY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

## 双 T 鼓的可变触发脉冲

同样，对于低音鼓的声音，我们需要一个门到触发器的电路，除了使用一个比上面更小的电容，它是一样的。但我们真正喜欢双 t 鼓电路的一点是不同输入电压尖峰的音量动态。也就是说，如果你用一个小的电压尖峰击中 twin-t，它是安静的，如果你用一个大的电压尖峰击中它，它就会变大。在你的鼓模式中加入这种变化会让它们听起来不那么机械，所以值得考虑和花费一些电阻。事实上，这就是我们所需要的。

![4069_drums_interface.sch](img/1b40d7e99e569d01cf21d983d28fe4ef.png)

该电路将 4017 的输出合并到一个有效的分压器中。由于在任何给定时间，4017 的输出中只有一个会为高，我们可以很快算出这一点。当 A 变为高电平时，22K 电阻 R1 和两个并联的 100K 电阻 R2 和 R3 形成一个对地分压器，用于 50K。电阻器连接点处的电压输出为 22 / 72 * VCC，或者在 9V 电源下约为 2.75V。

当 B 或 C 中的任一个为高电平时，有效接地电阻具有 22K 和 100K 电阻的并联电阻，即 18K。由此产生的电压尖峰在 1.4V 左右有一个峰值，因此听起来有点安静。所有这些脉冲都必须通过二极管 D1，因此它们可能会被进一步衰减。您可以随意调整这些值，直到它们听起来正确为止。

[https://www.youtube.com/embed/cc3Rh-KZxm8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/cc3Rh-KZxm8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

## 输出混音器和最终细节

最后，将所有不同的声源通过 100K 电阻，并在放大器的输入端连接在一起，就可以组合起来。这个简单的加法“混合器”又快又脏，而且工作得很好。如果你想让一个声源更安静或更响亮，你可以在合理的范围内改变这些电阻值:你能做到的程度取决于你连接的放大器的输入阻抗。两个因子可能是可以的。实验。

一种更加工程化的解决方案包括从每个声源中消除 DC 偏移，并使用运算放大器或类似器件对它们求和(可能具有可变增益)。这是个好主意，但这本身也是另一个项目。

## 灵感

基于 4017 的经典音序器是“ [Baby 10](http://midiwall.com/gear/babyseq/) ”。最初的目的是驱动电压控制的模拟齿轮，因此除了我们正在使用的开关栅极信号之外，它还会在每一步输出一个可调电压。如果你有任何需要控制电压的东西，用十个电位计来构建一个完整的 Baby 10 是很值得的。你会在网上找到大量的链接。

## 下一次会议

这个会议是关于控制的排序。下节课我们将回到疯狂。我们将继续使用 4017，尽管下次会以“意想不到”的方式。但主要的吸引力将是移位寄存器，特别是 4015。混乱随之而来！