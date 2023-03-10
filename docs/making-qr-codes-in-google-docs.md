# 在谷歌文档中制作二维码

> 原文：<https://hackaday.com/2013/09/28/making-qr-codes-in-google-docs/>

![screen-shot-2013-09-18-at-1-48-20-am](img/0ba3b176fbc8fa5c063b43a3d4bfe184.png)

[Jordi]给我们发来了这个关于如何在 Google Docs 中生成二维码的好建议。如果你需要一次制作很多，这将会非常方便，而且它们可以随时更新！

在他的例子中，他设置了创建 vCards 的代码，这样他就可以快速方便地将联系人转移到他的手机上。该代码拉入一个 Google API QR 生成器，并为您提供一个 QR 代码作为图像！以下是他的代码，可以很容易地修改以满足您的需要:

```
=image(&quot;https://chart.googleapis.com/chart?chs=200x200&amp;cht=qr&amp;chl=BEGIN:VCARD%0AN:&quot; &amp; A2 &amp; &quot;%20&quot; &amp; B2 &amp; &quot;%0ATEL;CELL:&quot; &amp; C2 &amp; &quot;%0AEMAIL:&quot; &amp; D2 &amp; &quot;%0AEND:VCARD&quot;)
```

或者如果你只是想要最基本的:

```
=image(&quot;https://chart.googleapis.com/chart?chs=200x200&amp;cht=qr&amp;chl=&lt;strong&gt;YOUR CELL&lt;/strong&gt;&quot;)
```

如果你需要完整的演示，休息后会有视频。那些想摆弄更多二维码黑客的人会喜欢从二维码形成图像的[和将二维码铣入铜层的](http://hackaday.com/2012/04/13/qart-codes-the-better-way-to-put-picture-in-a-qr-code/)。

[https://www.youtube.com/embed/sRuObJ538pA?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/sRuObJ538pA?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

【谢谢乔迪！]