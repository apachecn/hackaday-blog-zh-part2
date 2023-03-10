# Raspberry Pi 用作 Squeezebox 服务器

> 原文：<https://hackaday.com/2012/12/26/raspberry-pi-used-as-a-squeezebox-server/>

![rpi-squeezebox-server](img/95b0a734c3384e5cc65a3111309d08b0.png)

[Jacken]喜欢他的无损音频，正因为如此，他一直是 Squeezebox 的粉丝。它使高比特率文件的流式传输成为可能。但在罗技收购该公司后，他觉得他们已经做出了一些选择，将该平台推入了地下。但还是有希望的。他想出了如何使用 Raspberry Pi 作为 Squeezebox 服务器，这样他就可以继续使用他的客户端设备，并发布了关于 RPi 性能的细节，同时提供高质量的音频。

首先是坏消息:RPi 板没有必要的马力进行动态下采样。他甚至尝试超频，但这并没有真正帮助。好消息是，这个问题只影响旧的 Squeezebox 客户端(他在 V3 上遇到过这个问题)，并且只在播放比 CD 质量高得多的曲目时(24 位，88.2Khz)。他可以轻松地将这些文件传输到可以播放它们的设备上，甚至可以一次传输多个文件而不会出现任何问题。

你可以按照这个指南在你自己的 Raspberry Pi [上安装 Sqeezebox 服务器。](http://allthingspi.webspace.virginmedia.com/lms.php)