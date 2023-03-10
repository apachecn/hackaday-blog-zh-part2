# 仅用 HTML 和 CSS 渲染分形

> 原文：<https://hackaday.com/2015/01/26/rendering-fractals-with-just-html-and-css/>

What’s better than spending hours and hours with CSStrying to get images and text to center properly? Not [Jim], but he did notice thatCSS3 was a very powerful language. He wondered about building Tetris, a Turing Machine, or rendering fractals purely in CSS and HTML. The jury is still out if a Turing machine is possible, but [he did manage to generate some simple fractals using just CSS and HTML](http://snowflake.me/?p=11), no JavaScript required.

大多数分形是递归的，CSS 规则可以应用于已经应用了规则的 HTML 对象。不完全是递归，因为没有办法用 CSS 动态生成 HTML。然而，只需几个标签，[Jim]就能生成一级毕达哥拉斯树。这种方法需要在 HTML 中为树的每一层放置标签，这极大地限制了酷的因素。这很容易通过几个 CTRL+c 和 CTRL+v 来弥补。

同样的技术可以用来渲染科赫雪花—[见本页](http://srv-a.bwns.be/jim/koch.html)。对，都是 HTML 和 CSS，没有 JavaScript。为什么？因为他可以，这对我们来说已经足够了。