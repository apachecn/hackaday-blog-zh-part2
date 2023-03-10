# 口袋妖怪人工智能比你聪明

> 原文：<https://hackaday.com/2014/05/19/pokemon-artificial-intelligence-is-smarter-than-you/>

在不断被一些愚蠢的游戏控制恶棍杀死后，谁没有愤怒地把游戏控制器扔过房间？这太令人失望了！你可能希望有某种方式“越过那一点”。为了朝这个方向迈出一步，[Ben]创造了一个人工智能程序，它将在 Game Boy Advance 的口袋妖怪 Blue 中获胜。

该游戏在一个名为 Visual Boy Tracer 的 Game Boy Advance 模拟器中运行，该模拟器本身是最常见的 GBA 模拟器 Visual Boy Advance 的修改版本。让 Visual Boy Advance 与众不同的是，它有一个内存转储功能，允许用户将 RAM 和 rom 发送到模拟器之外。RAM 保存了模拟器当前需要的所有值，这包括从文本箭头闪烁时间到当前与口袋妖怪战斗的细节以及玩家在当前加载的地图中的位置。内存转储功能是让人工智能理解游戏中正在发生的事情的关键。

![Pokemon Artificial Intellegence](img/526df1778b1e55fa7eb0157a5c59e12c.png)

AI 代码用 python 编写，使用包含 Win32 API 的 pywin32 附加组件。Win32 API 允许程序与 Windows 交互，特别是模拟按键。AI 使用这些模拟的按键来与仿真器交互，而不是将仿真器构建到 AI 代码中。人工智能代理有两个关键目标:导航地图到每个新的教练和击败每个教练没有失去一个口袋妖怪。这些目标需要不同的模式，一个“搜索”模式和一个“战斗”模式。

搜索模式是人工智能最基本的形式，它是一个反应代理。反应剂只是对他们在特定时间看到的东西做出反应。在这种情况下，代理被编程为查找教练旁边的位置。通过知道它在哪里和它需要去哪里，人工智能发送一个模拟的击键来将玩家移动到适当的位置。就位后，人工智能会“挑战”训练者。

当处于战斗模式时，人工智能有更多的工作要做。它首先计算所有对立口袋妖怪组合对每个自己口袋妖怪的潜在战斗伤害。然后，人工智能运行决策树，决定做出什么决定。例如，与健康相关的决策在决策树中处于较高的位置，AI 将在评估任何攻击之前决定治疗虚弱的口袋妖怪。这样可以确保没有口袋妖怪被打败。

即使你不是口袋妖怪的粉丝，你也不得不承认这是 DIY 人工智能的一个惊人的练习。查看视频，了解这个项目的实际情况。

[https://www.youtube.com/embed/8Yq6lvtgrOo?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/8Yq6lvtgrOo?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)