# DSP 01:真正的，合法的发烧友的善良

> 原文：<https://hackaday.com/2015/02/27/dsp-01-real-legit-audiophile-goodness/>

大约六个月前，我们看到了[tshen2]在 DSP 01 上的工作，这是一款 2 输入、6 输出的 DSP，是专为极端音响发烧友设计的分频器，这里我们不是在谈论无氧房间。DSP 01 将 USB 音频输出转换为六路输出，为您提供低音、中音和高音的完美均衡，集成 6x100W 放大器，并补偿室内噪音。[最近这个项目有了很大的更新](http://hackaday.io/project/2374-dsp-01-hi-fi-audio-signal-processor),【t Shen】非常乐意分享细节

项目进行到这个阶段并不是没有问题。为了让 DSP 通过 USB 端口与计算机通信，[tshen2]在 [CP2114 USB 至 I2S 桥](http://www.silabs.com/products/interface/usbtouart/Pages/usb-to-i2s-digital-audio-bridge.aspx)中找到了一个潜在的解决方案。这个设备应该起到 USB 音频接收器的作用，将数字音频转换成 DSP 可以理解的内容。[这个芯片在【t 申】的设计](http://www.latentlaboratories.com/blog/2015/2/1/dsp-01-part-6)中没有工作。CP2114 只是做错了 i2s；I2S 规范说时钟必须是连续的。该芯片通过 SPI、固件和其他一些东西实现 I2S，因此与 to-spec I2S 不兼容。

虽然在将音频输入设备时出现了一些问题，但设备的核心仍保持不变。[tshen2]仍在使用 ADI 公司的[DSP](http://www.analog.com/en/audiovideo-products/audio-signal-processors/adau1701/products/product.html)，有趣的 SigmaStudio 被用来[补偿房间的频率响应](http://www.latentlaboratories.com/blog/2015/2/22/dsp-01-part-10-room-treatment-optimized-eq-treble-adjust)。这是一个真实的、合法的、基于科学的音响发烧友领域，对于一个有时可以理解却没有得到应有尊重的领域来说，这是一个令人印象深刻的发展。