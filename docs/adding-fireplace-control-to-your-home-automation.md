# 为您的家庭自动化添加壁炉控制

> 原文：<https://hackaday.com/2013/03/15/adding-fireplace-control-to-your-home-automation/>

![fireplace-automation](img/b3bcd29096dced846b166852abc7e2e1.png)

[詹姆斯]有一个令人钦佩的家庭自动化系统，他一直在努力多年。它可以监控车库门的状态，控制灯光，甚至在停电时通知他。系统中还没有的一件事是他家里的壁炉。你在上面看到的硬件是[他如何接入壁炉远程控制系统](http://www.geek-tips.com/2013/02/23/hacking-a-fireplace/)以实现自动化。

遥控器使用射频与基站通信。与控制使用红外的家庭影院组件不同，这使得它更难接入。当然，我们希望看到对协议的一些[逆向工程，以便可以使用简单的无线电模块，但是【詹姆斯】选择了对他来说意味着最少黑客攻击的路线。他将电线焊接到按钮的 PCB 上，并使用簧片继电器连接到它们。这些让 Arduino 模拟按钮按下。](http://hackaday.com/2010/07/05/reverse-engineering-an-rf-clicker/)

随着钻机连接到家庭网络，他有很多选择。该系统可以感知房子是否有人居住。如果它确定没有人在家，它将关闭壁炉。[James]还提到了监控一氧化碳或房屋火灾的能力，在这两种情况下都可以关闭燃气壁炉。