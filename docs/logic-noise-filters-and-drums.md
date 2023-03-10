# 逻辑噪声:过滤器和鼓

> 原文：<https://hackaday.com/2015/03/25/logic-noise-filters-and-drums/>

## 过滤器和鼓

[逻辑噪声](http://hackaday.com/tag/logic-noise/)是用 CMOS 逻辑芯片构建原始合成器的探索。本次会议，我们继续滥用 4069UB 作为放大器。我们将把[最后一节](hackaday.com/2015/03/09/logic-noise-sawing-away-with-analog-waveforms/)的简单单位增益缓冲器变成一个单极点有源低通滤波器。(剧透:是电容。)

虽然非常有用，但这个简单的过滤器有点无聊，而且很难做成动态的。因此，我们将研究一种完全不同的滤波器，双 T 陷波滤波器，它足够尖锐，可以构建正弦波振荡器，也足够可调，可以制作阻尼振荡器鼓音。

这是我们前进方向的一个快速演示。请继续阅读，了解我们如何实现这一目标。

[https://www.youtube.com/embed/8r_tpvt4-Jo?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/8r_tpvt4-Jo?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

## 过滤

上节课，我们构建了一个放大器，并研究了增益:输出电压摆幅与输入电压摆幅之比。[有源滤波器](http://en.wikipedia.org/wiki/Active_filter)是一种放大器，其增益取决于输入信号的频率。这让我们可以划分出我们喜欢或多或少的不同频率范围。(不过，一般来说，你不需要放大器来滤波。参见[无源滤波器](http://en.wikipedia.org/wiki/Passivity_%28engineering%29#Passive_filter)与有源滤波器。)

例如，当你在吉他上拨弦时，会产生各种各样的频率。但是随着时间的推移，弦的振动会被制作吉他的木材减弱，在半秒左右的时间内，剩下的大部分振动都与弦的基本振动频率有关(由手指在品上的位置决定)。更高频率的振动是最先消失的。这表明了制造“自然”发声乐器的声音合成策略:产生各种频率，然后过滤掉较高的频率。

## 单极低通滤波器

鉴于上次我们已经制作了几个简单的放大器电路[，现在可以快速了解所有滤波器中最简单的一种:单极滤波器。这是电路图:](http://hackaday.com/2015/03/09/logic-noise-sawing-away-with-analog-waveforms/)

![filter.sch](img/a906ccfdea2ff34eb6f71c0f111da19f.png)

是的，那是一个附加的电容器。这就是全部了。但是听一听有什么不同:

[https://www.youtube.com/embed/FMi54WlW-mU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/FMi54WlW-mU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

记住上次关于负反馈放大器的直觉。我们有两个电阻，一个在输入和 4069 之间，另一个在(反相)输出和输入之间的反馈中。当输入电压在 4069 的零线电压附近波动时，输出在相反的方向波动。电压摆幅与增益之比取决于反馈路径抵消输入信号电流的努力程度。

同样的直觉也适用于滤波器，只要你了解电容的一点。电容器只是不情愿地让电流通过。电容器在被“充电”到能抵抗任何进一步输入电流的电压之前通过的电流量称为其电容。或者，在电子数学中:C = Q/V 或 V = Q/C，其中 Q 是电容上的电荷，也是一段时间内的电流(每秒电荷)总和。

简而言之，你放入电容器的电荷越多，它产生的电压就越高，以阻止更多的电荷进入。电压上升的速度与电容的 1 成正比，与通过的电流成正比。

对我们来说，这意味着给定的电流很容易在短时间内通过电容，但很难在更长时间内通过相同的电流，而且如果不增加输入电压来克服电容的“充电”电压，就不可能永远通过电流。或者换句话说:电容器容易让高频电流振动通过，抵抗中频，拒绝恒压直流电。

那么，当我们在单位增益反馈放大器的反馈路径中放置一个电容时，会发生什么呢？由于电容几乎会阻挡非常低的频率，因此所有频率都必须通过电阻，从而获得单位增益。随着我们提高频率，一些电流开始流经电容，总反馈电阻降低。这意味着输出更容易抵消输入，因此中频增益更低。在非常高的频率下，电容很容易通过电流，几乎没有电流需要通过电阻，增益甚至会更低。

更简单地说，电容对低频的抵抗力比高频强。在负反馈放大器中，当更难推动电流通过反馈路径时，输出增益会增加。因此，通过在反馈路径中放置一个电容，我们可以使放大器在低频时增益更大，在高频时增益更小。瞧，一个低通滤波器！

### 可变截止低通滤波器

如果我们想改变截止频率呢？在数学中，像这样的单极点低通滤波器的截止频率是 1/(2 * pi * R * C)。实际上，我们可以通过改变电容或通过电阻改变输入电流来改变截止频率。因此，我们将通过选择电容值来设置基本范围，并通过旋转电位计来改变滤波器的频率响应。对于此处的电路，截止频率范围从 100k 欧姆时的 160 Hz 到 10k 欧姆时的 1600 Hz。

但是改变输入电阻有一个问题；我们还改变整体增益，这取决于反馈电阻与输入电阻的比值。因此，如果要通过大幅改变输入电阻来改变频率响应，可能还需要同时改变反馈电阻来跟踪它，保持总(通带)增益大致恒定。为此，你需要一个立体声/双电位计，它只是两个电位计连接到同一根轴上。用一个旋钮，你可以控制两个相同的电阻。

[https://www.youtube.com/embed/Va0Rhlxpcsc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/Va0Rhlxpcsc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

在我们离开单极滤波器之前，您可以将低通滤波器转换为高通滤波器，只需将电容移出反馈环路，并将其放在输入电阻之前。试试看！

## 双 T 滤波器

如果我们在反馈路径中加入更复杂的滤波元件，我们的故事会变得更加有趣，我们最喜欢的滤波器之一是 Twin T。Twin T 不是上图中的低通滤波器，而是一个[陷波滤波器](http://en.wikipedia.org/wiki/Band-stop_filter)。陷波滤波器通过高频和低频，但被调谐以消除中间的特定频率。

在其原始形式下，双 T 滤波器对于消除信号中的特定干扰频率非常有用。也许你想消除电力线噪声(美国 60Hz，欧洲 50Hz)。将一个调谐到 60Hz 的双 T 滤波器放入链中，你将去除大部分噪声，而不会过多地衰减其余的信号。要了解它为什么被称为双 T，请看电路图:

![twint.sch](img/be41db2c000c34127742e20c47259dbc.png)

双 T 的工作原理是将两个信号路径合并，每个路径都是 T 形的。带有两个电阻和一个接地电容的 T 是一个简单的低通滤波器，本质上是我们上面制作的滤波器的无源版本。串联电容和电阻接地的另一个 T 是高通滤波器。

高通和低通听起来好像一切都应该通过，对不对？是的但是。在滤波器调谐的频率(“截止”频率)，两个输出与输入的相位相差 90 度，但方向相反。理论上，如果两个 Ts 调谐到相同的频率，两条路径在截止频率上完全相互抵消，该截止频率根本无法通过。实际上，你可以让两个分支彼此非常接近，很好地消除调谐频率，但不是完美的。

当我们将双 T 滤波器放入放大器的反馈路径时，会发生什么情况？请记住，负反馈逻辑要求输出产生更大的电压，越难通过反馈路径推回电流。因此，我们不是去除滤波器调谐到的频率，而是放大某一特定频率。如果在我们调谐的频率上有一点点噪声进入输入端，它会被放大很多，而所有其他频率会被衰减。突然你就有了一个正弦波振荡器。

## 鼓

这就引出了今天的杀手电路，并对上述解释进行了一点改进。简而言之，我们对双 T 滤波器进行了一点去谐，这样它只有在受到脉冲时才会响起，然后消失。

首先，我们来玩一会儿，构建电路的双 T 和 4069UB 放大器部分。它只是上面的 Twin-T 滤波器设置在 4069UB 反相器级的反馈路径中，然后通过另一个 4069UB 反相器作为缓冲直接发送出去。它开得太快了，你会听到扳机的滴血声，但这是一个开始。

![drums_simple.sch](img/c34768bf5daa4e05abbb1699fc291357.png)

[https://www.youtube.com/embed/OYIHsXgqpYY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/OYIHsXgqpYY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

### 风雅

基本电路工作后，让我们从两个不同的方面展开。首先，我们将使用另一个振荡器电路来驱动鼓。然后，我们将通过低通滤波器传递音频，以消除一些泄漏的触发脉冲。

这是最终的电路:

![drums.sch](img/3e92c89a9a2be4b254ab12576210f1bc.png)

从左边开始，我们在 40106 上设置了一个极低频振荡器，并使用另一个 40106 级进行缓冲。这就简单地输出了一个可靠的方波。然后信号通过一个电容，电容的作用也是只让高频通过。什么让它通过看起来基本上像一个快速脉冲(绿色)。

![drum_square_to_trigger](img/efb99b7eb1cac160fcb8aebb1d0121a5.png)

触发信号脉冲被插入到 Twin T 的反馈环路中。实际上，触发器连接在哪里并不重要，但如果连接在这里，它与 Twin T 部分的耦合会更小。

[https://www.youtube.com/embed/Qx_vgkgQllE?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/Qx_vgkgQllE?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

最后，我们将信号通过一个低通滤波器，消除馈入输出端的原始触发信号中的 clicky 噪声。

[https://www.youtube.com/embed/gjAa2gu5hDI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/gjAa2gu5hDI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

### 范围

电容和电阻应该用什么值？尝试选择元件值，使低通 T 中的单个电容是两个电容的两倍(2 C)，单个电阻是成对电阻的一半(1/2 R)。这使得两个 Ts 调谐到相同的频率，再次由 1/(2*pi*R*C)给出，其中 R 和 C 分别是成对电阻和电容的值。

在实践中，尽可能使用两倍的电容，并使电阻可调。因为我们会故意去调谐电路，使振荡慢慢消失，所以没有一个可靠的电阻公式。你只需要选择电容器，调整旋钮，直到它工作。也就是说，如果你发现你想要的频率超出了你目前得到的频率范围，不要犹豫更换电容。

[https://www.youtube.com/embed/S5Vy8JVRRdw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/S5Vy8JVRRdw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

### 调整和调谐

使 Twin-T 部分失谐是使该电路作为鼓而不是正弦波振荡器工作的秘密，并且您必须采取的方法有点实验性，所以让我们来谈谈调谐该电路。正如我们之前提到的，如果将双 T 的两半完美对齐，只有一个单一频率会被阻挡，因此只有一个频率会被负反馈电路放大。你会得到一个非常好的正弦波振荡器，但不是鼓。

如果您使 Twin T 的两个半部彼此失谐，特别是如果您通过提高高通滤波器的截止频率使其高于低通滤波器来实现这一点，Twin T 会阻挡越来越宽的频带，从而接收放大器的额外增益。

但是，当你将增益分布在越来越宽的频带上时，在任何给定的频率下，你得到的增益都会变小。当你继续使 Ts 彼此失谐时，你会到达一个点，在这个点上，电路不再放大任何单个频率足以使其自身无限振荡。然而，这是关键所在，如果提供足够强的脉冲信号，滤波器会振荡一段时间。这正是我们对来自速度振荡器的方波通过电容耦合所做的工作。如果你有示波器的话，在示波器上观察阻尼波形是很好的。

![drum_trigger_and_pulse](img/d1b763d7eb3b5ec2cfed72cb6b7b4845.png)

这里有一个接近你想要的声音的步骤。要在较宽的频率范围内实现振荡，请将衰减电位计设置得尽可能低。这将 T 的高通支路设置为非常高的截止频率，这意味着它几乎不通过任何东西。这释放了低通 T 部分来确定音高，并且对于调音电位计的大部分范围，您会得到振荡。通过听振荡器来选取您想要的粗略音高。现在你可以调整衰减壶，直到振荡被阻尼掉，你就准备好了。

但是请注意，这两个电位计会稍微相互影响。那是因为 T 的两条腿只是简单的电连接。因此，当您增加从振荡器到鼓的衰减时，也要准备好调整频率电位计，以保持鼓音调在您想要的音高和衰减率。

[https://www.youtube.com/embed/MF4CCoiy6Hw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/MF4CCoiy6Hw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

## 扩展ˌ扩张

如果你有兴趣探索更多的有源滤波器设计，而不仅仅是这里显示的单极低通滤波器，看看 [Rod Elliott 关于有源滤波器的精彩文章](http://sound.westhost.com/articles/active-filters.htm)。你可以分解并使用运算放大器和双电源，或者你可以继续破解并用 4069UB 级替换他的电路中的任何运算放大器，只要它们只使用负反馈并将运算放大器的正端接地。特别是，看看多反馈拓扑结构和双二阶。

如果你不需要合成器鼓，你可以简单地调整双 T 了，并使用电路作为正弦波振荡器。对于单组电容，它的可调范围不是很大，但如果你需要的是单一频率，你可以选择正确的电容，这样就可以了。它不是最好的正弦波振荡器，但很难超越内置几个无源元件的单芯片构建。

但是不要相信我们的话:这里有一个镜头。黄线是产生的正弦波，紫色是信号的 FFT。竖条为 20dBV，即 10 倍。150Hz 处的第一个峰值是我们的正弦波，第二个峰值的电压下降了约 100 倍。这不是实验室设备，但对于滥用 CMOS 逻辑芯片来说，这是相当可靠的。

![scope_0](img/444b29495d0121308febc67a2def24ff.png)

如果你想抓狂，没有什么可以阻止你向电路提供音频触发脉冲。结果非常类似于我们在之前[制造的同步振荡器，但是它更加柔和，因为这里涉及的波形基本上是正弦波。](http://hackaday.com/2015/02/04/logic-noise-sweet-sweet-oscillator-sounds)

[https://www.youtube.com/embed/aZ8-gXdEulQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/aZ8-gXdEulQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

玩得开心！