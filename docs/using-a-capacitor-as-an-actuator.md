# 用电容做执行器？！

> 原文：<https://hackaday.com/2015/08/20/using-a-capacitor-as-an-actuator/>

[Dan Berard]一直使用[电容器作为致动器](http://dberard.com/2015/08/16/mlcc-piezo-actuators/)。

我们之前已经介绍过丹的[超棒的自建 STM(扫描隧道显微镜)](http://hackaday.com/2015/01/13/cheap-diy-microscope-sees-individual-atoms/)。这些显微镜通过在表面上移动纳米精度的针尖来工作。虽然他获得的图像很棒，但他使用的致动器的一个缺点是刚性差。这限制了系统更快的扫描速度。

在寻找更好的致动器的过程中,[Dan]认为他可以尝试使用 MLCC 电容器！虽然不知道它们的机电属性，但您可能遇到过似乎“[唱](http://product.tdk.com/capacitor/mlcc/en/faq/pdf/31_singing_capacitors_piezoelectric_effect.pdf)”(PDF)的电容器，发出可听见的音调。这是由于钛酸钡的压电特性。实际上，电容器充当弱压电扬声器。

使用 100V 驱动电压[Dan]能够使用电容器获得 300nm 的偏转。为了扩大致动器的范围，他决定“极化陶瓷电介质”，这包括将电容器加热到居里温度 120C 以上。为此，他使用了一个晶体管作为特别的加热板来加热零件。这将致动器的范围增加到 800 纳米，是许多 STM(和其他 SPM)系统的理想选择。

[丹]仍在权衡他的下一个版本的选择，但 MLCC 电容器肯定是一个便宜而有趣的选择。