# 生命时钟的游戏

> 原文：<https://hackaday.com/2013/10/19/game-of-life-clock/>

![GOLclockOperating](img/bdc91ec752ce119c859d9689cd86a173.png)

[亚历克斯]想做一个 LED 时钟。但是简单地制作一个 LED 阵列时钟太容易了——所以他决定让它[遵循一些有趣的规则……](http://www.brainlubeonline.com/GOL_Clock/index.html)

听说过约翰·康威的《生命的游戏》吗？这很简单——有四条规则。

1.  任何少于两个活邻居的活细胞都会死亡，似乎是由人口不足引起的。
2.  任何有两个或三个活邻居的活细胞都会延续到下一代。
3.  任何有三个以上活邻居的活细胞都会死亡，似乎是由于过度拥挤。
4.  任何一个死细胞，只要有三个活的邻居，就会变成活细胞，就像通过繁殖一样。
    【来自[维基百科](http://en.wikipedia.org/wiki/Conway's_Game_of_Life)

所以[亚历克斯]决定让他的时钟 LED 矩阵遵循这些规则，点亮的像素代表生命。每一分钟，在分钟，时间显示。但是一旦它被展示出来，规则就接管了，展示就瓦解了，遵循着生命的游戏规则。这是一个非常有趣的显示器，正等待被放大到更大的尺寸。

他在自己的博客上写得很好，还附上了他的代码——所以如果你有兴趣，可以看看！如果没有，休息后留下来看看时钟的运行。

[https://www.youtube.com/embed/mwZeDfqhdPw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/mwZeDfqhdPw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)