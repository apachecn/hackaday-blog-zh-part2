# 一种移动无线电功率控制器

> 原文：<https://hackaday.com/2014/10/10/a-mobile-radio-power-controller/>

[皮特]，又名[KD8TBW]想把他的八重洲收音机装在他的车里。根据经验，他知道在汽车里有一个收音机不可避免地会让它偶尔开着，这一次，他想要一个当钥匙插在点火开关上时可以打开和关闭他的装置。他最终做了一个移动无线电能量转换器。当交流发电机运行时，它从汽车上获取 12V 电压，当发动机停止时，它关闭一切。

问题中的八重洲收音机——FT-8800 确实有自动断电功能，但这是一种糟糕的做法。没有办法重新打开无线电，无线电必须处于非扫描模式。

在他希望成为 EagleCAD 的最后一个设计中，[Pete]设计了一个带有 ATtiny85 的电路板，可以测量车内的电压；当电压为~14V 时，交流发电机工作，收音机可以打开。降到~12V 的时候就该关收音机了。这是一个伟大的项目，有了 3D 打印的外壳，它可以很容易地被塞进控制台。下面视频。

[https://www.youtube.com/embed/b8SvVXVKk1w?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/b8SvVXVKk1w?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)