# Thalmic 实验室关闭免费开发者访问更新:它又回来了

> 原文：<https://hackaday.com/2014/11/18/thalmic-labs-shuts-down-free-developer-access/>

Thalmic Myo 是一款带有 IMU 和肌电传感器的电子臂带，能够测量手臂的方向和肌肉运动。这款设备的用途从假肢到《少数派报告》风格的用户界面。Thalmic 也是一家 Y Combinator 公司，拥有 1500 万美元的资金和技术媒体对这种未来设备的可能用途进行了大量报道。的确，这是一个关于用户界面和伪医疗设备的未来的非凡故事，它可以绕过大多数 FDA 法规。

几个月前，Thalmic 发布了 Myo [的固件更新，阻止了对肌电传感器](https://developer.thalmic.com/forums/topic/1215/?page=1#post-5623)的原始访问。任何想为 Myo 开发的人现在都需要提交申请，并向 Thalmic 及其投资者支付一磅肉——学术机构最高可达 5000 美元。当前版本的固件仅提供对 IMU 数据和“手势”的访问，而不是原始肌肉数据，这些数据在研究 RSI 检测、截肢者假肢或地中海论坛上流传的上百种其他想法时将是无价的。

Thalmic [创办他们的公司](https://web.archive.org/web/20130513060225/https://www.thalmic.com/)的想法是，开放的 SDK 最适合社区，除了最新版本的固件之外，所有版本都可以访问原始传感器数据。几个固件版本之前，Thalmic 删除了对这些原始数据的访问，[打破了许多开源项目](https://github.com/dzhu/myo-raw/issues/4)，这些项目将用于研究人员或任何使用 Thalmic Myo 进行实验的人。幸运的是，一些足够聪明的人发现了版本号[，一个可以读取原始传感器数据的开放库](https://github.com/jwcrawley/myo-raw)。它运行良好，Thalmic 的官方立场是，原始传感器数据在未来将无法使用。如果你想用 Myo 开发一些东西，这个库正好救了你一命。

Thalmic [将很快发布关于获取原始传感器数据的官方声明](https://developer.thalmic.com/forums/topic/1215/?page=1#post-5623)。

说句题外话，如果你想知道几乎所有形式的媒体都是不正当的，试着把它提交给《黑客新闻》,看看 Thalmic 投资者。编辑:不用麻烦了，我们上黑名单了还是怎么的。

**更新:** [Thalmic 已经更新了他们的政策](https://www.thalmic.com/blog/big-data/)，稍后将发布一个允许访问原始 EMG 传感器数据的固件版本。去除原始传感器数据的原因有两个:

*   电池寿命。从臂带中流出原始数据需要很大的能量。显然，在 uC 上计算出“手势”并向*发送这些*可以节省电能。
*   用户体验。肌电图数据因人而异，很难解读。