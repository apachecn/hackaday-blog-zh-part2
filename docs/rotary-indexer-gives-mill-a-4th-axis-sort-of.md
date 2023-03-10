# 旋转分度器为磨机提供第四轴(类似)

> 原文：<https://hackaday.com/2015/07/04/rotary-indexer-gives-mill-a-4th-axis-sort-of/>

旋转分度器是大多数机械工厂的标准配置。这些可以让你握住或夹住一个工件，然后一个带刻度的手柄可以让你旋转工件。当您想要钻孔或攻丝轴向或径向特征时，这很有用。齿轮齿条传动确保工件在加工载荷下不会移动。通常，这些分度器也有一个手动锁，以照顾齿轮齿隙和发挥。自动化它们也不太困难。你可以只使用步进电机(开环)或伺服+编码器(闭环)来驱动转盘。

[smashedagainst]需要在一个零件上钻六个径向孔。他必须在 500 个零件上做总共 3000 个洞。这只是第一次运行，未来可能会有更多的钻探。问题中的零件体积小，重量轻。因此，他没有使用重型工业级装置，而是使用步进电机和 Arduino 建造了一个[全电动旋转分度夹具](https://hackaday.io/project/5984-sort-of-4th-axis)，给他一种旋转第四轴。他的想法是直接使用步进电机来旋转工件，而不需要任何传动装置，但他需要建立自己的钻机来做到这一点。

他最初的原型使用 Arduino Uno，在最终版本中他用 Pro Mini 替换了它，以节省一些空间。Arduino 连接到一个[坚固电路马达驱动器](http://www.ruggedcircuits.com/motor-control/rugged-motor-driver)。在他尝试的几个驱动器中，这是唯一一个设法用足够的扭矩保持步进电机以防止工件在钻孔时移动的驱动器。要钻的孔的数量在 Arduino 中是硬编码的，所以他需要的只是一个按钮。每按一次按钮，步进电机就前进 60 度，给他六个等间距的孔。他使用 NEMA-34 步进电机，这意味着强大的电源。他从一台旧的激光打印机上找到了一个电源，这台打印机有 24V DC 和 5V 输出。

下一步是进行机械装配。他加工了一个装在步进电机轴上的心轴。心轴的表面是六边形的，工件楔入/位于其上。电机组件固定在底板的一端。基板的另一端具有由肘节夹启动的夹紧机构。它也能够旋转(很像车床上的[活顶尖](https://en.wikipedia.org/wiki/Lathe_center))。工件与心轴配合，然后肘节夹具将工件锁定到位。在最初的试验中，一些装配紧固件松动了，钻头发出了一些振动。他解决了这些问题，并发现当他将主轴转速设置为 2400 rpm 时，性能最佳。一旦他把它修好，他就能在不到两个小时内完成一百个零件。快速连续钻六个孔会导致零件变得非常热，所以他首先使用了一些加压空气冷却。后来，他改用基于喷雾罐的多用途渗透润滑剂。观看他的视频的索引夹具在下面的行动。

[https://www.youtube.com/embed/YLRxrawWX1A?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/YLRxrawWX1A?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)