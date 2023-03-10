# 用亚马逊 Echo 控制 Nest 设备

> 原文：<https://hackaday.com/2015/07/25/control-nest-devices-with-amazon-echo/>

[ZPriddy]正在寻找一种用 Amazon Echo 控制他的 Nest 恒温器的方法。他不想满足于使用 AWS 或其他托管服务。[ZPriddy]想要一个可以完全由他自己托管和管理的东西。最终结果就是他所说的“回声疗法”。

【ZPriddy】从学习如何使用 Alexa 技能包(ASK)开始。ASK 是官方 SDK，允许发烧友为他们的 Amazon Echo 添加功能。对[ZPriddy]来说不幸的是，他找到的大部分示例代码都是为在 Amazon Lambda 上使用而设计的，但这并没有阻止他。在找到一些 Amazon Echo 请求和响应的例子后，他就上路了。

[ZPriddy]选择使用 Flask 实现一个简单的 web 服务器。web 服务器监听 Amazon 请求并做出适当的响应。它还提供身份验证，以确保一定程度的安全性。该服务器能够同步同一家庭中多个 Nest 设备的温度，但它也可以增加或增加整个范围内的温度。这是通过一些简单的语音命令完成的，比如“告诉 Nest 我有点冷”。如果你喜欢亚马逊 Echo hacks，一定要看看另一个用于控制 WeMo 设备的工具。

[https://www.youtube.com/embed/WMfxfmuqJc8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/WMfxfmuqJc8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)