# 建立一个智力竞赛节目风格的蜂鸣器系统

> 原文：<https://hackaday.com/2012/06/01/building-a-quiz-show-style-buzzer-system/>

![](img/65e05fab9fdd6329247f67f9e6ed019c.png "quizz-show-style-buzzer-system")

这些是[菲利普·克雷蒂安]为他母亲制作的团队蜂鸣器。她是智力竞赛节目的忠实粉丝(我们在考虑 Jeopardy 之类的节目)，他认为她会喜欢家庭游戏的适当设置。

每个单元由一个街机按钮和一个 LED 组成，都位于一个项目箱中。他用电话线将每个蜂鸣器连接到基本单元。我们喜欢这个想法，因为我们有很多旧的电话线，我们的 RJ-45 卷曲包括一个 RJ-11 插槽。这非常适合制作我们自己的电缆。

基本单元包含一个 Arduino 板，该板轮询按钮以查看哪个按钮被首先按下。相应蜂鸣盒上的 LED 会亮起，以便玩家知道谁先进入。这种设置的一个特点是能够从 30 种不同的蜂鸣器声音中进行选择。

如果你感兴趣的话，Hackaday 上还有其他几个测试蜂鸣器项目。我们最喜欢的一个系统是使用塑料碗作为按钮的系统。

[途径 [Adafruit](http://www.adafruit.com/blog/2012/05/31/diy-arduino-based-quiz-buzzer-system/)