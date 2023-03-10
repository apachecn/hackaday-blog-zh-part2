# 无人驾驶固定翼飞机在停车场穿针引线

> 原文：<https://hackaday.com/2012/08/16/autonomous-fixed-wing-drone-threads-the-needled-in-a-parking-garage/>

![](img/b41839e2f2cb798752733191f90c8de4.png "autonomous-fixed-wing-drone")

我们已经对四轴飞行器有了一些喜爱，但仍然有空间在侧面做一些小事情。这架[固定翼无人机可以完成一些相当惊人的导航](http://web.mit.edu/newsoffice/2012/autonomous-robotic-plane-flies-indoors-0810.html)。麻省理工学院的 Robust Robotics Group 正在展示他们对这架飞机所做的工作，最终在一个停车场进行了一次不顾死亡的飞行(休息后的视频)。这听起来可能不是一个巨大的成就，但考虑到翼展超过两米，在同一赛道上重复运行使其在几厘米内夹住支撑柱。

不像精密的四轴飞行器[依赖于静止的高速摄像机来获得反馈](http://hackaday.com/2012/03/09/vijay-kumars-ted-talk-on-the-state-of-quadcopter-research/)，这种无人机是独立的。它确实依赖于从它的环境地图开始，结合使用激光测距仪和惯性传感器来绘制它的路线，并在必要时进行调整。我们认为它必须比四轴飞行器计划得更远，因为它没有刹车和悬停的能力。然而，这是该设计的优势之一。由于它使用固定翼方法，所以在相同电池容量的情况下，它可以比四轴飞行器在空中停留更长时间。

[https://www.youtube.com/embed/kYs215TgI7c?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/kYs215TgI7c?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[via [Reddit](http://www.reddit.com/r/gadgets/comments/ya4rw/autonomous_robotic_plane_flies_indoors_at_mit/)