# 脚本缺陷 minteye 验证码

> 原文：<https://hackaday.com/2013/01/16/script-defeats-minteye-captcha/>

![minteye-captcha-defeated](img/d7b69d987dcb9dfe070579ad42f7a56c.png)

我们之前没有听说过 minteye CAPTCHA，但是我们已经看到了能够破解系统的脚本的证据。Minteye 结合了你可能不喜欢的两样东西:广告和验证码。该系统使用滑块来扭曲广告商的图像。一旦滑块在正确的位置，图像变得清晰，你可以点击提交，看看你是否通过了挑战。

像这样的挑战对于视障人士来说是不可能的，所以通常也有音频选项。在这种情况下，音频按钮将指示您向右、向左移动滑块，或者它已经在正确的位置。[Samuirai]使用 Google Chrome 中可用的 text2speech API 来解析这些命令。正如你在上面看到的，“电影之后”是对“移动滑块”的曲解，但他仍然能够获得足够的准确性来解决挑战。休息之后，请观看视频中的脚本。

音频挑战在过去曾被这样利用过。通过音频选项来看看这个关于[击败 reCAPTCHA 的演讲。](http://hackaday.com/2012/06/15/stiltwalker-beat-audio-recaptcha/)

[https://www.youtube.com/embed/u0M7gmS5Eg0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/u0M7gmS5Eg0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[感谢哈迪斯通过 [Shackspace 博客](http://shackspace.de/?p=3765)