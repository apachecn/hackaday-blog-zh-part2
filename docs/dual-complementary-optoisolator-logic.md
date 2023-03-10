# 双路互补光隔离器逻辑

> 原文：<https://hackaday.com/2015/01/09/dual-complementary-optoisolator-logic/>

你见过 CMOS 逻辑，你见过二极管电阻逻辑，你见过基于继电器的逻辑，你们中的一些人听说过棒逻辑。[【朱利安】刚刚发明了光隔离器逻辑](https://www.youtube.com/watch?v=tebprQvrqk4)。他提出了以前没有这样做的两个原因:要么[Julian]非常聪明，要么光隔离器逻辑是一个非常愚蠢的想法。可能只是前者。

每个光隔离器内部都有一个 LED 和一个光电晶体管。这两个器件之间没有电气连接，这正是所谓隔离器所需要的。[Julian]有一天在玩一些光隔离器来创造一个奇怪的推挽电路；一个光电晶体管的发射极连接到另一个的集电极。将光电晶体管的另一端连接到+5V 和 Gnd 意味着他可以在 VCC 和 VDD 之间切换，电路的其他部分都被隔离。这个想法在他脑海中盘旋了几个月，直到他想到将更多的 led 连接到光隔离器的输入端。由于四个 led 的压降，他可以将隔离器的输入连接到+5V 和 Gnd。

[朱利安]脑子里又转了几个轮子，他决定在两个光隔离器之间连接一个开关。将电路的“输入”连接到地使得连接到+5V 的 LED 点亮。将电路的输入连接到+5 使连接到地的 LED 亮起。兔子洞越陷越深[朱利安]。

通过更多的按钮和发光二极管，[Julian]创造了“与”、“与非”或“或非”的东西，这取决于你的观点。他已经有了一个逆变器和几十个来自中国的光隔离器。

从理论上讲，用它来建造一台被称为计算机的东西是可能的，但那会对这种电路的独特性质造成损害。除了基本的“1”和“0”逻辑状态，这些门还可以配置为三态输入和输出。这是巨大的；当你只处理 1 和 0 时，只有两个万能门。如果你能对付一个二，大约有 20 个通用逻辑门。

它还不是三进制计算机([虽然我们看过那些](http://hackaday.io/project/1043-base-3-ternary-computer-from-scratch)，但它很酷，而且很可能不笨。

下面视频。

[https://www.youtube.com/embed/tebprQvrqk4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/tebprQvrqk4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)