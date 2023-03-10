# USB 实现者论坛对开源说不

> 原文：<https://hackaday.com/2013/10/22/usb-implementers-forum-says-no-to-open-source/>

长久以来。爱好者和销售带 USB 端口的硬件的小公司的主要障碍之一是 USB 实现者论坛。售出的每台 USB 设备都需要供应商 ID (VID)和产品 ID (PID ),才能被认证为 USB 兼容设备。Adafruit、Sparkfun 和业余爱好者市场中的其他大公司都向 USB 实现者论坛支付了 USB VID，但这并没有帮助那些在车库里希望出售几百个自制 USB 设备的人。

蜘蛛实验室有一个有趣的想法来解决这个问题。由于 Microchip 和 FTDI 等其他 USB 设备供应商免费提供 USB PIDs，一个非营利基金会可以购买一个 VID，将 PID 提供给制造开源硬件的基金会成员，我们将生活在一个神奇的世界中，那里有被认证为 USB 兼容的自制设备。

这个想法与 VTM 集团不太合拍，他们是 USB 实现者论坛的管理、公共关系、法律、会员和许可部门。作为一种稍微不相称的反应，VTM 小组告诉蜘蛛实验室，

> 请立即停止筹集资金购买用于转让、转售或再许可 PID 的唯一 USB VID，并从您的网站和其他营销材料中删除所有提及 USB-IF、VID 和 PID 用于转让、转售或再许可的内容。

有趣的是，Arachnid Labs 和其他几十个开源 USB VID 的请求还没有到达 USB 实现者论坛的[任何人的办公桌上，这些人是*实际上负责指定 USB VID 和 PID 的*。有很多想法可以绕过 VTM 集团，包括抢注 USB VID 0xF055，但我们不知道为什么不能有一个给出开源 USB PID 的基金会。微芯片、FTDI 和](http://www.usb.org/about) [Openmoko](http://wiki.openmoko.org/wiki/USB_Product_IDs#Conditions) 也是如此，所以也许是时候给惠普、英特尔和微软的一些关键人物发电子邮件了