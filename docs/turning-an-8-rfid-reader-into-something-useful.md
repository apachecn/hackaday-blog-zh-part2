# 把一个 8 美元的 RFID 阅读器变成有用的东西

> 原文：<https://hackaday.com/2013/02/16/turning-an-8-rfid-reader-into-something-useful/>

[杨奇煜]不久前在 Deal Extreme 上偶然发现了一个非常非常便宜的 RFID 阅读器，钱多得用不完，就把它加到了他的购物车里。当 USB RFID 阅读器到达时，[他注意到它有些奇怪的地方](http://skyduino.wordpress.com/2013/02/01/hack-lecteur-rfid-chinois/)(法语，[traduation](http://translate.google.fr/translate?hl=fr&sl=fr&tl=en&u=http%3A%2F%2Fskyduino.wordpress.com%2F2013%2F02%2F01%2Fhack-lecteur-rfid-chinois%2F))。RFID 阅读器以 USB HID 设备的形式出现在他的电脑上，每当 RFID 卡在线圈上方挥动时，它就会向文本编辑器中吐出字符。唯一的问题是这些字符不是 RFID 卡上记录的十六进制值。这是怎么回事？

[结果是](http://skyduino.wordpress.com/2013/02/08/hack-lecteur-rfid-chinois-huge-success/) ( [英国](http://translate.google.fr/translate?hl=fr&sl=fr&tl=en&u=http%3A%2F%2Fskyduino.wordpress.com%2F2013%2F02%2F08%2Fhack-lecteur-rfid-chinois-huge-success%2F))，这个随机的中国电子琴向计算机发送 10 个字节的数据，就像[这个有据可查的 RFID 阅读器一样。](http://www.ardushop.com/kits/electronic-brick-125khz-rfid-card-reader.html)显然，这两种 RFID 阅读器都采用 RFID 卡的十六进制值，将这些字节转换为十进制，并通过查找表传递每个数字。这是谁也猜不到的，但是既然[杨奇煜]知道了它是如何工作的，他也可以知道如何逆转这个过程。

不幸的是，问题中的 RFID 阅读器[目前在 Deal Extreme](http://dx.com/p/intelligent-id-card-usb-reader-174455) 缺货。然而，看到那里大多数可用的电子产品都非常相似，只是在外壳上印刷的名称不同，如果在其他地方有几乎相同的 RFID 阅读器，我们也不会感到惊讶。