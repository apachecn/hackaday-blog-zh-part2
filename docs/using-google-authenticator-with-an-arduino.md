# 通过 Arduino 使用 Google 认证器

> 原文：<https://hackaday.com/2013/09/14/using-google-authenticator-with-an-arduino/>

Google Authenticator 是一个生成一次性密码(OTP)的应用程序。这些密码通常用作身份验证的第二个因素，与您的普通密码一起使用。OTP 的工作原理是在两台设备上共享一个秘密和一个同步时钟。当您生成密码时，会创建一个基于密码和时间戳的哈希。这证明你可以接触到这个秘密，而且只能使用一次。

为了保护他的乐高迷你模型，[卢卡]使用谷歌认证器和 Arduino 建立了一个[认证系统。一个 web 应用程序用来生成一个秘密，这个秘密可以使用数组配置到 Arduino 中，使用 QR 码配置到 Google Authenticator 中。Arduino 使用的是](http://www.lucadentella.it/en/2013/09/14/serratura-otp/ "Serratura OTP")[库](https://github.com/lucadentella/ArduinoLib_TOTP "TOTP Library")，它实现了基于时间的一次性密码认证(TOTP)。

存在一些挑战，包括在 Arduino 上保持良好的时钟源，但这看起来是一种有趣的身份验证方式。休息之后，观看该项目的快速视频概述(对于英文字幕，点击 CC 按钮)。

[https://www.youtube.com/embed/AQuTeuIpuTg?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/AQuTeuIpuTg?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)