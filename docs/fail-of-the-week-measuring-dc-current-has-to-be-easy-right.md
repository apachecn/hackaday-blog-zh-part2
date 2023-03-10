# 本周失败:测量 DC 电流一定很容易，对吗？

> 原文：<https://hackaday.com/2015/03/10/fail-of-the-week-measuring-dc-current-has-to-be-easy-right/>

[DainBramage]需要一个直流安培计来检查他的业余电台在备用电池供电的情况下还能维持多久。他手头上已经有一个只能测量交流电的钳形表，另一个只能测量几毫安。因为他没有高达 25 安培的电表，所以他决定用从零件箱里捡来的零件自制一个 DC 电流表。测量 DC 电流并不太难。将待测电流通过精密电阻，并使用灵敏的电压表测量电阻上的电压降。

I = V/R

到目前为止，一切顺利。如果是在深夜，你已经喝了很多咖啡，忙着建立你的直流电流表，事情可能很快就会变糟。[DainBramage]的第一步是建立一个合适的分流。他有很多旧的 1ω、10W 电阻。他使用其中的 9 个进行了串并联组合，以创建一个强大的 1ω、90W 分流电阻(如果你想挑剔的话，0.999999999 欧姆)。这给了他一个很好的 1 伏特每安培比率，使他很容易做测量。

下一步是将分流器连接到合适的电压表上。幸运的是，他有一个微型伏特计，是从一个无线电产品上拆下来的。由于他没有电压表的数据，他在电表输入端连接了一个 10k 的电阻，慢慢地增加了施加在电表上的电压。在 260 毫伏时，指针触及满刻度，电压表输入端的电压为 33 毫伏。[DainBramage]然后描述了他用来计算具有 10A 和 25A 测量范围所需的电阻的数学方法。他错过了抓住失败的机会。然后，他的项目日志描述了将所有这些放在一个箱子里并打包的一些无聊的细节。

过了一会儿，他的更新突然出现。他可能意识到的第一件事是，他需要更精确的读数，所以他增加了连接器，以允许连接更精确的电压表，而不是模拟 Micronta。在这一点上，他仍然没有抓住失败，尽管它就在他的面前。

当他试图将自制的安培计与 12V DC 电源串联连接到他的业余无线电台时，他挠头了。每当他试图发射信号时(此时无线电正在吸收电流)，无线电就会关闭。如果您仍然没有发现故障，请尝试计算当电流为 1A 和 5A 或更大时，1ω分流电阻两端的电压下降了多少。