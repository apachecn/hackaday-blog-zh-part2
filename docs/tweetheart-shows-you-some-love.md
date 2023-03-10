# TweetHeart 向你展示一些爱

> 原文：<https://hackaday.com/2015/01/11/tweetheart-shows-you-some-love/>

[Stacey]想要一种更有趣的方式来监控与她的 Twitter 帐户相关的事件。她最终得到的是一盏[美丽的动画心灯](http://thebitchwhocodes.com/2014/12/22/pixelbeat-a-neopixel-heart-that-is-twitter-sensitive-iot/ "TweetHeart")。

她从设计围栏开始。有了激光切割机，她选择用薄胶合板制作它。[Stacey]使用一个叫做[boxe maker](http://boxmaker.connectionlab.org/ "BoxMaker")的在线工具来设计实际的盒子。这个工具使用起来非常简单。你只需输入盒子的尺寸，它就会为你提供一个二维模板，你可以用它来制作激光切割机。最终的胶合板像拼图一样拼在一起。心脏部分由磨砂丙烯酸制成，也是由激光切割而成。

为了照亮心脏，[Stacey]选择使用[新像素](http://hackaday.com/tag/neopixel/ "NeoPixel Projects")。这些就像我们过去见过的许多 RGB LED 灯条，尽管像素密度比大多数都高。她将 LED 灯带切割成合适的尺寸，然后将它们粘在一块胶合板上，形成一个粗略的心形。她在每一步中都测试了灯光，这样她就能准确地知道什么时候出现了错误。

[Stacey]选择使用一个[火花芯](http://hackaday.io/projects/tag/spark%20core "SparkCore")来控制发光二极管。这具有开箱即用的 WiFi 连接的优势。[Stacey]从 NeoPixel 示例程序开始，但很快意识到它们都依赖于延迟功能。这对她来说是个问题，因为她需要不断关注新的 Twitter 事件。她最终不得不自己编写依赖中断的函数。

[Stacey]然后写了一个 Node.js 脚本来监控 twitter，控制 Spark。该脚本监视特定的事件，例如[Stacey]的一条推文被转发，或者用户没有关注[Stacey]。然后，脚本向 Spark 发送一条消息，告诉它刚刚发生了哪个事件。火花然后将重复事件，直到一个新的事件发生。查看下面的演示视频。

[https://www.youtube.com/embed/FnKCuaVDzpQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/FnKCuaVDzpQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)