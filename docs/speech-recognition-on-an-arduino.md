# Arduino 上的语音识别

> 原文：<https://hackaday.com/2012/09/22/speech-recognition-on-an-arduino/>

![](img/5f8c001b0d80cd3ff7e7d34d7eabff1d.png "speech")

语音识别通常是相当高性能的计算机的权限，这些计算机拥有数百兆赫兹的内存。将语音识别引入 Arduino 中的低功耗微控制器听起来像是疯狂的科学家或博士生的工作，但这正是[Arjo Chakravarty]所做的。他为 Arduino 开发了[μ语音库，允许对有限的一组语音命令进行语音识别。【T2](http://arjo129.github.com/uSpeech/) 

大多数语音识别系统使用 FFT 和非常复杂的数学来确定用户所说的音素，[Arjo]的系统消除了这种不必要的复杂性，转而使用非常非常基本的积分和微分。

从[Arjo]的[μSpeech](http://cloud.github.com/downloads/arjo129/uSpeech/%C2%B5Speech.pdf)用户指南(PDF 警告)中我们可以看到，可以将一个小麦克风连接到 Arduino 的模拟输入，并接受语音命令，如“左”、“右”和“停止”。准确率也相当不错——如果μSpeech 试图识别单词，准确率为 80%，如果μSpeech 被编程为识别单个音素，准确率为 30-40%。

遗憾的是，我们找不到μSpeech 运行的演示视频，但是非常欢迎您通过 github 为您自己的项目获取它。[给我们发一个μSpeech 的视频](http://hackaday.com/contact-hack-a-day/)，我们会把它放上去。