# 适用于所有人的 USB PIDs

> 原文：<https://hackaday.com/2015/04/03/usb-pids-for-all/>

USB 实现者论坛并没有让任何人制造带有 USB 端口的产品变得容易。为了销售任何带有 USB 的东西并让它像 USB 应该的那样工作，你需要购买一个 USB 供应商 ID，一个 5000 美元的许可证，授予你 65，536 个 USB 产品 ID 的独占使用权。很少有公司会发布 65，000 个产品，而且有很多闲置的 PID。

现在，有人终于做了一件明智的事情[，将一个未使用的 USB VID 投入使用](http://pid.codes/howto/)。pid.codes 获得了单个 VID——0x 1209——的权利，现在他们将剩下的所有 pid 打包给开源硬件项目。

这不是一个由 USB 实现者论坛支持的项目，更像是 pid.codes 方面的合法游戏。没用，因为他们不能重新分配给别人。VID 的原始所有者[interiometrics](http://pid.codes/org/interbiometrics/)在 USB-IF 禁止转让或再许可 VID 和 PID 之前许可了他们的 VID。

您可以通过分叉[pid . codes repo](https://github.com/pidcodes/pidcodes.github.com)，声明一个 PID，并发送一个 pull 请求来获得一个 PID。一旦被接受，这个 PID 就永远是你的了。