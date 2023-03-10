# 击败 DRM 延长抗衰老治疗光罩的寿命

> 原文：<https://hackaday.com/2015/03/16/beating-drm-to-extend-the-life-of-an-anti-ageing-therapy-light-mask/>

如今，DRM 出现在越来越多的硬件产品中变得越来越常见。通常，它用于防止使用未经授权的消耗品，有些人可能会认为它有助于防止伪造和帮助支撑收入。但是当 DRM 被用来严重限制产品的使用寿命时，情况就完全不同了。当[travis]写下“Illumimask”光疗设备的运行时间限制时，我们首先必须查找该设备是什么。显然，这些是抗痤疮或抗衰老的光疗面膜，它们使用红色和蓝色发光二极管来杀死皮肤细菌，刺激皮肤细胞，减少瑕疵。虽然这些说法很可能站不住脚，但设备本身足够便宜，不会因为 30 美元一台而伤害你。

问题是，它被限制为每天使用 30 次，每次 15 分钟，总共只有 7 个半小时，实际上可以持续一个月。最后，你只需扔掉这个设备，换一个新的。这看起来像是对一个完美的功能设备的荒谬浪费，这个设备的 LED 可以持续至少 30，000 到 40，000 小时。[travis]的妻子[Bebefuzz]显然对这种情况很生气。所以她做了一个简单的[破解，绕过了施加愚蠢限制的微控制器](https://www.lollipuff.com/blog/329/diy-how-to-reuse-reset-illumask-light-therapy-mask)。用[特拉维斯]自己的话来说，“不是一个疯狂的技术黑客…而是绕过制造商的‘WTF’的非常实用的一个。它包括在电路端子上焊接一个滑动开关，微控制器用它来监控 LED 电流(可能)。不幸的是，这也破坏了 15 分钟的计时器测量，因此她现在必须在 15 分钟治疗周期结束时手动关闭设备。

要查看更多 DRM 黑客，查看我们之前提到的这些，从[咖啡机](http://hackaday.com/2014/12/16/drm_protection_removed_for_coffee/)到 [3D 打印机灯丝](http://hackaday.com/2014/04/10/resetting-drm-on-3d-printer-filament/)到[猫砂盒](http://hackaday.com/2015/01/19/cracking-litter-box-drm/)，甚至[家具](http://hackaday.com/2013/03/04/drm-chair-only-works-8-times/)。