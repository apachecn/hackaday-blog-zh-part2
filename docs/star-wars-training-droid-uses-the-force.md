# 星球大战训练机器人使用原力

> 原文：<https://hackaday.com/2014/05/02/star-wars-training-droid-uses-the-force/>

![Star Wars Training Droid](img/07245fbca50410dfb667cce1f5176acf.png)

我们都知道这个场景，欧比万·克诺比给了卢克一个头盔，并放下了防爆盾。他告诉路加“你的眼睛会欺骗你。不要相信他们。带着感情伸展出去！”欧比万说起来容易——他没有一个远程训练机器人飞来飞去向他射击。[Roeland]和他的团队正在为 [Hackday 的科幻竞赛](http://hackaday.io/page/276)创造一个现实版的训练机器人。

《星球大战》中的训练机器人可能没有原力支持，但它在空中相当敏捷。为了复制这一点，该团队从标准的 Walkera 瓢虫微型四轴飞行器开始。让一个人来控制这个由无人驾驶飞机变成的机器人本来是很简单的事情，但是[罗兰德和他的同事]想要一个完全由计算机控制的系统。瓢虫可以携带很小的有效载荷，但它没有能力举起一台计算机和传感器套件。该团队从 [GRASP 实验室](http://hackaday.com/2011/07/03/robotic-schadenfreude-quadrotor-blooper-reel/)获取了一份记录，并使用一台带摄像头的外部计算机来控制他们的机器人。

该团队没有使用大型实验室使用的昂贵的动作捕捉系统，而是使用了一对 Wii 遥控器来实现立体视觉。安装在机器人顶部的一个小红外 LED 让 Wii 遥控器的摄像头可以看到它。一台笔记本电脑被用来计算机器人的当前位置。知道了当前位置和期望位置后，笔记本电脑计算并向 Arduino 发送命令，Arduino 随后为机器人的控制器翻译这些命令。

干得好伙计们！现在你只需要添加爆破发射器！

[https://www.youtube.com/embed/YRHqNIK6npY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/YRHqNIK6npY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)