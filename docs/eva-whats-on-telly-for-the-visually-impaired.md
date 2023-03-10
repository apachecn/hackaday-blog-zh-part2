# 伊娃:电视上为视障人士播放什么节目

> 原文：<https://hackaday.com/2015/03/04/eva-whats-on-telly-for-the-visually-impaired/>

[可咀嚼的布料]肯定是用他的树莓派做好事了。随着时间的推移，他女朋友的爷爷视力越来越差。他喜欢看电视，但在阅读有关频道和节目的屏幕信息时有困难。为此，【可咀嚼的布料】开发了一个名叫伊娃的电子语音助手，她从网络服务中获取电视节目表，并通过谷歌翻译的 TTS 功能用她可爱的声音大声朗读出来。

伊娃的引擎盖下是一个树莓皮。一个 USB 集线器为 Pi 供电，并装有一个小型 USB 声卡、一个 Wi-Fi 加密狗和一个控制器插入的 USB 子板。子板来自 USB 键盘，它在 awesome 控制器中再次出现。它由一个操纵杆和两个街机按钮组成，使用 USB 键盘的控制器与 Python 脚本进行交互。

[chewabledrapery]的脚本向一个名为 atlas 的 web 服务发出格式化请求，该服务返回带有电视时间表和内容描述的 JSON 对象。伊娃然后转向谷歌翻译，通过一个小放大器和抢救 PC 扬声器朗读格式化的文本。为了最大限度地减少网络调用的次数，伊娃的一些经常性的沉思被存储在本地。休息之后是 EVA 的完整巡演。

我们喜欢看到帮助人们的黑客。还记得这个 [RFID 有声读物阅读器](http://hackaday.com/2014/08/23/rfid-audio-book-reader-for-the-visually-impaired/)吗？

[https://www.youtube.com/embed/ocwmer5dliU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/ocwmer5dliU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)