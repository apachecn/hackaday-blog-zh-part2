# 在不平坦的底座上研磨翘曲的 PCB 坯料

> 原文：<https://hackaday.com/2014/12/12/mill-warped-pcb-blanks-on-an-uneven-bed/>

如果你制作的是一次性电路板，在家加工 PCB 是节省时间和金钱的好方法。不过也有不好的一面，有点难。当然，只需[将](http://www.pcbgcode.org/)你的[鹰](http://www.cadsoftusa.com/eagle-pcb-design-software/product-overview/?language=en)设计输出为 CNC 机器可理解的 g 代码，然后开动你的轧机…嗯，没那么容易。

PCB 坯料上的铜的厚度可以从大约 0.001 英寸到 0.006 英寸。当铣板时，理想的情况是铣得足够深，以穿过铜，但不要切入玻璃纤维背板太深。切得太深会削弱木板，折断一点，或者在极端情况下，切穿整个木板。

浅的切割会导致另一个问题，即板表面的切割深度不一致。看看上面左边的照片。棋盘左侧的痕迹似乎刚刚消失。发生这种情况是因为电路板不平。走线缺失的一侧比另一侧低，因此刀头无法触及电路板的该部分。由于理想的切削深度约为 0.010 英寸，即使是非常小的波纹或不平整也会在铣削过程中造成严重的问题。如果你很难想象 0.010 英寸是什么，想想两张纸的厚度，这不是很多。平整度问题有两个主要原因:PCB 板和/或机床底座。床不平整，PCB 就不平整。即使床是平的，PCB 也可能翘曲或弯曲。

PCB 制造爱好者[daedelus]有这个确切的问题，并以真正的黑客方式，决定做点什么。他创建了一个名为[自调匀整器](http://www.autoleveller.co.uk/)的软件程序，该程序采用 g 代码文件，并在铣削操作开始前添加一个探测部分。当修改后的 g 代码文件在 CNC 机器上运行时，它首先以网格模式探测 PCB 的表面，并绘制 PCB 表面的平整度变化。然后，当运行该程序时，它会动态调整刀头的高度，从而使整个纸板的实际切割深度保持一致，而不管纸板是否平整。第一次尝试的结果是一个干净和可用的 PCB。

有一个问题:必须设置机器控制软件来接受探针。如果通过计算机的并行端口与 CNC 机床通信，这很容易做到。并行端口上的输入引脚通过一个电阻拉高，并与 PCB 板电连接。刀具主轴通过线夹引线接地。当刀具接触电路板时，输入引脚被拉低，机器控制软件记录该特定 XY 位置的刀具高度。

[https://www.youtube.com/embed/R8o2Sy-KPUU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/R8o2Sy-KPUU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)