# 一个开源的 IPad 显示适配器

> 原文：<https://hackaday.com/2014/03/12/an-open-source-ipad-display-adapter/>

iPad 3 和 4 中那些花哨的 2048×1536 像素分辨率显示器可不仅仅用于高清糖果粉碎和网飞观看。英国南安普顿的弗雷迪[制作了他自己的适配器](http://projects.hackaday.com/project/369-OSCAR%3A-The-Open-Screen-Adapter)来将这些高分辨率液晶面板连接到任何有显示端口连接的东西上。它被称为奥斯卡，这是一种开源的方式，可以在一秒钟(或三分之一秒，或四分之一秒)内添加大量像素。)班长。

iPad 3 和 4 中的液晶面板没有使用几乎所有其他液晶面板中常见的 LVDS 连接。它使用 DisplayPort 协议的扩展，这意味着任何具有这些端口之一的显卡都已经为这个面板做了大量工作。唯一需要的是一个适配器来控制电源和背光，这很容易由 ATMega32U4 处理。这使得 OSCAR Arduino 兼容，可以轻松添加传感器和 USB 玩具。

OSCAR 可以在 Kickstarter 上以 65 英镑(约 100 美元)的价格买到。除此之外，你还需要通过普通渠道购买一台 iPad retina 显示屏，价格约为 65 美元。不完全便宜，但尝试找到另一个比这个价格更好的 1080p 显示器。