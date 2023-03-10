# 自动遥控汽车通过航路点导航

> 原文：<https://hackaday.com/2013/06/16/autonomous-rc-car-navigates-by-waypoints/>

![autonomous-rc-car](img/34bf66dfe6e9ca6dd2e1c27b61564f97.png)

看看这辆[Jason]为 chipKIT 设计挑战赛打造的自动遥控汽车。它只需要几个路点作为输入，就能成功地导航一条计划好的路线。

显然，这使用了一个芯片套件作为控制器，具体来说是 max32。[Jason]的文章展示了该设计的所有组件，但你必须去看他最近发布的更新，以了解他为托管所有组件而开发的定制板。它从一个 GPS 模块开始，但它的精确度只够给漫游者一个大画面。为了成功地从一个航路点到达下一个航路点，他还安装了一个陀螺仪，提供非常准确的方向数据，以及车轮上的光学编码器，用于车载行驶距离信息。

我们希望他继续完善设计，并参加明年的自动驾驶汽车比赛。

[https://www.youtube.com/embed/wrCWLSO1FBU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/wrCWLSO1FBU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)