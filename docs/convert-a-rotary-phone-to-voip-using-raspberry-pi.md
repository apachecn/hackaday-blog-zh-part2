# 使用 Raspberry Pi 将旋转式电话转换为 VOIP

> 原文：<https://hackaday.com/2015/03/09/convert-a-rotary-phone-to-voip-using-raspberry-pi/>

旋转式电话有一种令人怀念的东西，使它成为一件有趣的事情来破解和现代化。[Voidon]测试了他的技能，[用树莓 Pi](http://imgur.com/a/HECDL) 把一个转换成了 VoIP。他使用 RasPi 的 GPIO 引脚从转盘读取脉冲——功能转盘在[转盘](hackaday.com/2014/07/22/usb-rotary-phone-a-lync-to-the-past/) [电话](hackaday.com/2014/06/16/the-rotary-cell-phone/) [黑客](hackaday.com/2012/09/07/rotary-and-cordless-phones-mashup/)中总是受欢迎的功能。旧的 USB 声卡非常适合麦克风和手机音频。

与任何构建一样，有一些意外的大小问题需要解决。虽然 RasPi 可以很好地放入机箱，但没有 USB 电源插孔或以太网电缆的空间，更不用说 USB 电源组了。电力银行的想法被放弃了。[voidon]在 polyfuse 之前将电源线焊接到 RasPi 以保护电涌保护，使用迷你 USB wifi 转换器，并将新的 USB 连接器焊接到声卡。[Voidon]也无法让手机原来的铃声工作，所以他使用树莓派的内置声卡播放铃声。

VoIP ( [SIP](http://en.wikipedia.org/wiki/Session_Initiation_Protocol) )由一些 Python 脚本管理，可从 [GitHub](https://github.com/hnesland/aselektriskbureau) 获得。[voidon]有一些在日常工作中使用[星号](http://www.raspberry-asterisk.org/)的经验，所以看看他将来是否会使用它会很有趣。

[via [Reddit](http://www.reddit.com/r/raspberry_pi/comments/2y21sd/i_converted_an_old_phone_to_voip_using_raspberry/)