# 用旧的 BIOS 芯片修复世嘉墨盒

> 原文：<https://hackaday.com/2015/02/19/fixing-sega-cartridges-with-old-bios-chips/>

出于这样或那样的原因，[Dragao]有一个旧的刺猬索尼克弹药筒，它在弹球区舞台的某个地方抛出了一个非法指令。虽然这种非法指令的原因可能是宇宙射线，但如何修复这个墨盒还不太清楚。虽然使用旧电脑的 BIOS 芯片也可以做到这一点。

[Dragao]从 Game Boy flash carts 那里得到了修复这个弹壳的想法。这些墨盒使用的芯片是 Game Boy CPU 的地址和数据线的简单并行接口，Sega Genesis / Mega Drive flash cart 也是如此。问题是找到可以工作的旧 DIP 闪存芯片。他最终在一台旧电脑的主板上找到了一些 8 位宽的芯片，通过堆叠这些芯片，他拥有了一个 16 位宽的闪存芯片。

为了给芯片编程，[Dragao]将所有东西都连接到 Arduino Mega 上，在芯片上放一个 ROM，然后连接到旧的世嘉墨盒上。令人惊讶或不惊讶的是，一切都工作了，现在[德拉高]有了一个完整功能的刺猬索尼克副本。