# 在 OSX 上构建 ARM 交叉编译器

> 原文：<https://hackaday.com/2012/12/07/building-an-arm-cross-compiler-on-osx/>

![arm-cross-compiler-for-osx](img/0f79b65608f241cfffe4d683b57f0ab8.png)

我们已经尝试在 Linux 平台上构建我们自己的 ARM cross 编译器，但这并不容易。幸运的是，Mentor Graphics 提供了一个免费的交叉编译工具链(以前叫做 Code Sourcery G++)。但是那些想在 Mac 上开发的人就没那么幸运了。有一个脚本可以提供帮助，[Michael]写了一个指南，详细介绍了如何使用 crosstool-ng 在 Mountain Lion 上构建一个 ARM 工具链。

Crosstool-ng 是一个脚本，当编译所有不同的组件时，它自动完成大部分需要做的事情。但是在运行它之前，需要做一些基础工作。例如，OSX 附带的一些工具与脚本寻找的 GNU 工具不完全兼容。“grep”就是一个例子。Mountain Lion 有 BSD 版本的 grep，但是它缺少 crosstool-ng 使用的一些 GNU 版本的命令。[Michael]将指导您解决这个问题和一些其他问题，直到您拥有一个正常运行的工具链。