# 在 Raspberry Pi 上运行带有 GPIO 访问的简单 Web 界面

> 原文：<https://hackaday.com/2013/02/02/easy-web-interface-with-gpio-access-runs-on-raspberry-pi/>

这里有一个 Raspberry Pi hack】使用 PHP 和 MySQL 添加了 web 控件。如图所示，它提供了一个网页(使用 Apache2 服务器),允许您更改 GPIO 引脚的状态。这不是超级复杂，但很高兴看到[一步一步地指导安装和配置软件包](http://www.instructables.com/id/Web-Control-of-Raspberry-Pi-GPIO)。

Web 界面 GPIO 控制是我们喜欢的 Adafruit Web IDE 的特性之一。但是这个产品完全是从 RPi 加载的(Adafruit 包使用基于云的代码),并且使用了大多数 Linux 网络管理员习惯使用的工具。MySQL 数据库管理 GUI 命令和 GPIO 修改之间的连接。网页由一个 PHP 脚本提供，该脚本负责轮询和更改数据库值。配置需要一个新的数据库，以及可以访问它的用户名和密码。