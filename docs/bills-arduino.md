# 比尔的阿尔杜伊诺

> 原文：<https://hackaday.com/2015/02/13/bills-arduino/>

口袋妖怪本身是一个很棒的游戏，但当你意识到不是所有的' mon '都可以在一个游戏中使用，交易是完成交易所必需的，有些口袋妖怪不经过黑客攻击或 1997 年去玩具反斗城是不可用的，你开始看到这个游戏有多阴险。考虑到他最终可以用 Arduino 完成游戏，pepi jn[决定建立一个口袋妖怪存储系统](http://pepijndevos.nl/2015/02/13/catch-em-all.html)。

这个版本的灵感来自于一个早期的帖子[，它也欺骗了交易](http://hackaday.com/2014/01/02/spoofing-pokemon-trades/)。[Pepijn]决定使用 Arduino，而不是围绕高功率微处理器来构建这个项目。男孩们用来互相交流的协议游戏[被非常好地记录下来](http://www.devrs.com/gb/files/gbspec.txt)，尽管那只是战斗的一半。每个使用连接线的游戏都使用专门的数据结构进行传输，在[浏览了一个拆开的口袋妖怪 ROM](http://pepijndevos.nl/2015/02/12/grep-your-way-into-pokemon-red.html) 后，【Pepijn】[弄清楚了一切是如何工作的](https://github.com/iimarckus/pokered/blob/master/wram.asm#L1360-L1385)。

[完成的硬件](https://github.com/pepijndevos/arduino-boy)在 Arduino 的 EEPROM 中保存一个口袋妖怪。如果你想在第一代游戏中抓住所有 151 个口袋妖怪，这不是很快，但无论如何，你都会抓住很多鲤鱼王*。*