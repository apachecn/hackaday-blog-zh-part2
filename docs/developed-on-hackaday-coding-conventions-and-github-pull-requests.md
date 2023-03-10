# 基于 Hackaday 开发:编码约定和 GitHub 拉请求

> 原文：<https://hackaday.com/2014/03/12/developed-on-hackaday-coding-conventions-and-github-pull-requests/>

[![](img/c1dedc8cf58bde4f82bfbab3e6d094f8.png)](http://hackaday.com/wp-content/uploads/2014/03/moolt.png)

Hackaday 社区目前正忙于编写我们的[开源离线密码管理员项目](https://github.com/limpkin/mooltipass)的底层库。当许多有才华的贡献者在一个共同的概念上一起工作时，有趣的讨论就发生了。在我们专门的 Google 小组中，有些是关于命名/编码约定的选择，以及如何/何时批准 GitHub pull 请求。但是不要已经离开了…这个话题实际上比听起来更有趣。

较老和较年轻的固件贡献者之间的年龄差距被猜测为大约 30 岁…并且在这样的时间范围内可能发生许多事情。即使我们的编码员是用 C 语言写的，他们中的大多数人在学校/工作中用其他编程语言编码。他们还在不同的操作系统上使用不同的文本编辑器。可以理解的是，它们中的每一个都有自己偏好的[编码](http://en.wikipedia.org/wiki/Coding_conventions) / [命名](http://en.wikipedia.org/wiki/Naming_conventions_(programming))约定和[缩进样式](https://en.wikipedia.org/wiki/Indent_style)。多通大会是根据多数投票选出的，在收到许多电子邮件后，我们决定与 camelCase 召开一次奥尔曼式的大会:

> 【无效】{if(foo){function call()；}否则{foo = 0；anotherFunctionCall()；}}–79 字符行长度作为软要求–4 个空格，无制表符

大多数贡献者认为这是代码清晰性和跨平台兼容性之间的最佳折衷，但我们很想知道我们的 Hackaday 读者对这个特定主题的看法。

第二件事更像是管理问题。当一个项目处于初期，并且由(或多或少)无报酬的贡献者组成时，管理和审查对主 GitHub 库所做的代码变更的最佳策略是什么？完全可以理解的是，兴趣、业余时间和贡献意愿可能会随着时间的推移而变化。也许我们的一些读者可能已经熟悉了[敏捷软件开发](http://en.wikipedia.org/wiki/Agile_software_development)，这是一组基于迭代和增量开发的软件开发方法，它促进适应性规划、进化开发，并鼓励快速灵活地应对变化。你认为这可以应用到 Mooltipass 项目中吗？

我们很想听到关于这些话题的类似经历，因为我们乐于接受建设性的批评。你可能也想加入我们的[专门的谷歌小组](https://groups.google.com/forum/?hl=en#!forum/mooltipass),看看那里已经发生的不同讨论。另外，我们目前也在为 Kicad 寻找电容式滚轮/触摸按钮封装库。