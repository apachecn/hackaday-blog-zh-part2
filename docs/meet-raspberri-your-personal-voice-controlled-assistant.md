# 认识一下“Raspberri”，您的个人语音控制助理

> 原文：<https://hackaday.com/2014/02/07/meet-raspberri-your-personal-voice-controlled-assistant/>

![raspda](img/d52c12c02e750766d536991fa1a93baa.png)

我们都看过老电影场景，高管用对讲机呼叫他的助理处理一些任务。[Jan]可能不是主管，也可能没有助理。他确实有 Raspberri，他的声控个人数字助理。Raspberri 最初是一个老式的 Televox 对讲机。[Jan]在一家二手商店发现了它，并抢购了它，希望在未来的项目中使用它。当[Jan]得到一个树莓派并学会如何使用它时，这个项目最终发生了。他决定将 Televox 和 Pi 合二为一，创建自己的电子助手。

[Jan]开始在他的 Pi 上添加一个便宜的 USB 声卡和 WiFi 模块。他还添加了一个 3 瓦的音频放大器板。Televox 使用单个扬声器作为音频输入和输出。[Jan]不想对这个案例做任何修改，所以他保留了这个安排。使用单个扬声器意味着音频放大器和声卡的麦克风输入完全短路。为了避免这种情况，[简]增加了一个 DPDT 继电器，由 Televox 上原来的一键通按钮控制。继电器在 USB 声卡上的麦克风输入和音频输出之间切换。Televox 箱子里的所有东西都很合适。

硬件完成后[Jan]将注意力转向了软件。他用 PiAUISuite 进行语音输入。语音输出由一个简单的 shell 脚本处理，该脚本使用 google voice 将文本转换为语音。对于中间处理，比如从气象网站获取数据，[Jan]创建了定制的 python 脚本。最终结果相当不错。在说出命令和收到回答之间有一点延迟。这可能是因为通过 WiFi 传输音频文件。然而，[简]总是可以说他的助手出去给他拿更多的咖啡而逃脱惩罚！

![pda-inside](img/8f3707a98bfe2cd237dfbadf931173ea.png)

[https://www.youtube.com/embed/Wx3FHyCZ478?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/Wx3FHyCZ478?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)