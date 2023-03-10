# 最后，一个桌面数控机床与一个真正的主轴

> 原文：<https://hackaday.com/2014/04/30/finally-a-desktop-cnc-machine-with-a-real-spindle/>

虽然廉价的业余爱好数控铣床和路由器是很好的机器，可以让你建造 3D 打印机无法处理的东西，但它们也有其局限性。它们通常由 Dremel 或其他旋转工具驱动，因此通过 Gcode 控制主轴的速度几乎是不可能的。它们通常也是用一块胶合板作为床来建造的——便宜，但重复性不高。[Nomad CNC 工厂解决了这些问题](https://www.kickstarter.com/projects/178590870/the-nomad-cnc-mill)，并且看起来不错，价格也很便宜。

Nomad 团队没有使用 Dremel 或其他旋转工具来切割材料，而是使用连接到真正主轴的无刷 DC 电机。对于一些特定的电机，这允许主轴的闭环控制；将 S4000 Gcode 发送到研磨机将使主轴以 4000 RPM 旋转，S6000 以 6000 RPM 运行主轴，无论是通过泡沫还是铝。这是你不能用大多数台式研磨机和刳刨机中的 Dremel 或 DeWalt 旋转工具做的事情。

除了合适的主轴，Nomad 还具有归位开关、工具长度探针和一些附带的夹具，使双面加工成为可能，并且非常简单。控制磨机的软件是 Carbide Motion 和 MeshCAM，后者是一种非常流行的、很好地组合在一起的 CNC 控制器。当然，工厂本身使用 Gcode，所以它可以与开源 CNC 软件一起工作。

这是一个非常巧妙的包装。下面你可以找到一个游牧民族制作 Hackaday 标志的视频。

![unnamed](img/940bd5933dbfd9d9a12d739faae790e2.png)

[https://www.youtube.com/embed/JIc_NmrS488?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/JIc_NmrS488?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[https://www.youtube.com/embed/Ifs2vF5CT9w?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/Ifs2vF5CT9w?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)