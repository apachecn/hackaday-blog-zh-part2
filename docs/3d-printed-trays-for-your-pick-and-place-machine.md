# 用于取放机的 3D 打印托盘

> 原文：<https://hackaday.com/2014/06/12/3d-printed-trays-for-your-pick-and-place-machine/>

拾放机是电子产品的一把双刃剑。他们很快就能搭建好你的电路板，但是如果你没有把所有的东西都设置好，他们很快就会弄得一团糟。抓放器无法从一堆电阻中抓取并放置它——到目前为止，只有人类才能完成。他们需要在卷轴或托盘中组织和定位零件。

[Parker Dillmann]必须装载一些零件，但没有托盘，所以他自己 3D 打印了一些零件。【帕克】在德克萨斯州的一家小型装配厂工作。他正在进行一项[绝密设计](http://hackaday.com/2014/04/16/reload-pro-an-open-source-active-load/)，其中包括 FFC 连接器。不幸的是，连接器装在不友好的取放管中，而不是卷轴中。如果他找不到托盘，[Parker]将不得不再次手工放置这些连接器，这将增加构建每个板的时间，并留下更多出错的机会。

[帕克]没有手工放置每个部件，而是联系了他的朋友[【克里斯·克拉夫特】](http://kraftlab.com/)，他是一位 3D 打印专家。[Chris]证实 3D 打印托盘是可能的，尽管他用来打印的 PLA 不是静电安全的。这对于连接器来说很好，但[Parker]希望通过将他的 PSOC4 芯片也放在印刷托盘中来节省一些托盘空间。

[Parker]使用 SketchUp 设计了一个适合他的 Madell DP2006-2 拾放器的托盘。他在零件周围留出了 0.15 毫米的间隙——刚好足以覆盖印刷过程中的任何不准确之处，但不足以影响零件的放置。他将 STL 文件发送给[Chris],后者使用[simplify 3d](http://www.simplify3d.com/)创建了一个 Gcode 文件。[克里斯]在他的 [MakerGear M2](http://www.makergear.com/) 打印机上打印了 0.2 毫米层高的托盘，结果看起来很棒。它们对于取放机来说足够好吗？

[Parker]收到邮件中的打印好的托盘，并将零件装入其中。拾放器在寻找和放置连接器方面没有任何问题，这使得这项工作取得了巨大的成功。[Parker]甚至为 PSOC4 芯片留出了空间。他计划在试用之前，先用防静电漆把盘子涂上。

我们真的很喜欢这个故事——这是 3D 打印机如何加快制造过程的一个完美例子。既然基本设计已经完成，创建新托盘就是小菜一碟。干得好[帕克]和[克里斯]！

[https://www.youtube.com/embed/IaX2OAxJu0M?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/IaX2OAxJu0M?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)