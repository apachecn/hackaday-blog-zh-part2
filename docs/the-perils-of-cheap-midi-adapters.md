# 廉价 MIDI 适配器的危险

> 原文：<https://hackaday.com/2013/07/11/the-perils-of-cheap-midi-adapters/>

![MIDI](img/aea30d2e7d889451ec000f873703689c.png)

[Arvydas]最近买了一个 Rock Band 3 Wii 键盘，认为这将是一个非常棒而且非常便宜(9.99 英镑)的 MIDI 控制器。键盘有一个合适的 DIN-5 MIDI 输出端口，所以理论上唯一需要插入电脑的是一个 USB 转 MIDI 适配器。与键盘不同，MIDI 适配器是一件廉价的中国次品，但只要有一些独创性和一些组件，他就能让一切正常工作。

已有 30 年历史的 MIDI 规范包括一些如何正确连接 MIDI 设备的示意图。这些原理图中最重要的部分是 MIDI in 上的光隔离器，考虑到早期 MIDI 键盘的成本高达数千美元，这是一个很有价值的附加元件。似乎[Arvydas]' MIDI 转 USB 适配器不包括这个重要的组成部分，而是用一个简单的电阻来代替它。任何能降低成本的东西，对吗？

为了让 MIDI 适配器工作，[Arvydas]去了 Maplin，买了一个 optioisolator，所有东西都连接在试验板上，他让它工作，并最终将电路移植到适配器的 PCB 上。

让这个 MIDI 适配器正常工作是一件伟大的工作，特别是因为它怀疑这个廉价的适配器是否能与任何 MIDI 设备一起工作。