# 视频语音可视化

> 原文：<https://hackaday.com/2015/02/06/video-voice-visualization/>

为了他们在康奈尔大学的 ECE 4760 最终项目，[Varun，Hyun 和 Madhuri]创建了一个实时声谱图,该声谱图可以将声音模式和鸟鸣等音频以灰度视频的形式直观地输出到任何 NTSC 电视，没有明显的延迟。

该系统可以从板载麦克风元件或 3.5 毫米音频插孔接收输入。一个 ATMega1284 微控制器用于音频处理和 FFT 阶段，而另一个' 1284 将信号转换为 NTSC 输出的视频。麦克风和线路音频输入通过 LM358 运算放大器分别放大。由于音频采样频率为 8KHz，低通滤波器会滤除 4KHz 以上的频率。

休息之后，您可以看到团队通过对着麦克风说话和吹口哨来演示他们的项目，并通过线路输入来播放录制的鸟类叫声。他们在项目中内置了三个控件来冻结视频，将视频速度减慢两倍，并在线性和对数标度之间进行转换。还有录制的鸟类叫声可视化的短片和一个老式的拨号调制解调器。

[https://www.youtube.com/embed/bZ4p090KL3w?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/bZ4p090KL3w?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

#### 鸟鸣声

[https://www.youtube.com/embed/y6yHE4OqZSI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/y6yHE4OqZSI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

拨号调制解调器
[https://www.youtube.com/embed/3MZB4BtSd7M?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/3MZB4BtSd7M?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)