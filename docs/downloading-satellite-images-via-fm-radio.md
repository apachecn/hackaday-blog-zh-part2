# 通过调频收音机下载卫星图像

> 原文：<https://hackaday.com/2015/08/02/downloading-satellite-images-via-fm-radio/>

你知道气象卫星通过调频频率传送天气图像吗？现在你知道了…你可以[用一个 10 美元的调频收音机电子狗](http://mattg.co.uk/words/noaa_sdr/)自己拦截它们！

美国 NOAA 气象卫星位于地球周围的极地轨道上，每颗卫星大约每 12 小时经过同一点。当它在上空时，信号足够强，可以接收。在[Matt]发现这个知识的小片段后，他不得不自己学习如何截取图像。

卫星通过 137MHz 波段传输图像，使用无线电调谐器 USB 加密狗，你可以记录传输，然后将其解码成图片。他用 [CubicSDR](http://cubicsdr.com/) 调谐并记录信号，然后用 [Soundflower](https://rogueamoeba.com/freebies/soundflower/) 拉出干扰，最后用[WXtoIMG](http://www.wxtoimg.com/)——卫星在上方时开始记录，并解码图像。

【谢谢提示 Amirgon！]