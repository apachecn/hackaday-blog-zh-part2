# 给树莓派添加散热器

> 原文：<https://hackaday.com/2012/06/26/adding-heat-sinks-to-a-raspberry-pi/>

[Michael Dornisch]惊讶地发现，通过网络传输视频时，树莓 Pi 的主处理器温度达到了约 56 摄氏度(约 133 华氏度)。他认为，如果他能够稍微冷却一下，这可能有助于延长设备的寿命。但是为什么仅仅停留在处理器上呢？他[为 SoC、以太网/USB 芯片和电压调节器](http://michaeldornisch.blogspot.co.uk/2012/06/diy-raspberry-pi-heat-sink.html)增加了散热器。

他从零件箱中拿出一个可能用于显卡的小型散热器。在用他的数字卡尺测量了三个芯片后，他切下了他需要的足迹，从而得到了三个更小的散热器。我们没有意识到热复合材料有足够的夹紧力来在没有任何机械紧固件的情况下保持水槽在适当的位置，但显然它做到了。[Michael]提到可以使用其他粘合剂，如 JB Weld。重要的是，你要用一些东西(即:热化合物或液体粘合剂)来防止芯片表面和铝之间出现任何空气间隙。

他测量的结果是温度下降了 17.3 摄氏度(31 华氏度)。我们环顾四周，Broadcom 芯片上似乎没有内部温度传感器，因此这些表面读数就足够了。如果经常使用它来播放高质量的视频，您认为这会延长主板的寿命吗？我们已经知道[这些温度在硬件](http://hackaday.com/2012/06/23/checking-out-the-temperature-of-a-raspberry-pi/)的规格范围内。

[谢谢西蒙]