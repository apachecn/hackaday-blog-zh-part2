# 使用十六进制编辑器进行手动数据恢复

> 原文：<https://hackaday.com/2015/04/02/manual-data-recovery-with-a-hex-editor/>

假设你在工作中使用一个基于 SD 卡的便携式录音机——也许是采访。一切都很顺利，直到有一天，你在停止录音前把录音机关掉。如果不按下那个红色的大停止按钮，文件不会关闭，你会在 SD 卡上留下一个非常大的 0kB 文件。怎么拿回来？有一些工具可以帮你做到这一点，但是它们需要钱。你可以用一个十六进制编辑器自己做，这其实很简单。

数据恢复这一壮举所需的软件是 [Roadkil 的磁盘成像仪](http://www.roadkil.net/program.php?ProgramID=12)将 SD 卡上的所有位转储到一个图像文件，免费版本的 [ISO Buster](http://www.isobuster.com/) 显示每个文件的块地址和长度，以及您选择的十六进制编辑器。这个过程开始时只是 hot 的一个实验，通过剪切和粘贴比特到一个十六进制编辑器来创建一个 MP3 文件。在十六进制编辑器中找到一个好文件，复制到一个新文件，并播放。目前为止一切正常；太好了。

对于实际的数据恢复，我们创建了一个电子表格来根据经验猜测丢失文件的位置。从这个地址开始，大约 90MB 的数据被复制到一个新的十六进制编辑器窗口。这就是复苏遇到阻碍的地方。因为之前 SD 卡是插在 Mac 上的，卡上写了一堆数据。这进入了磁盘上第一个可用的位置，恰好是丢失的 MP3 文件的头。

这不是问题；在第一次实验中，已经有一个 MP3 文件的头在十六进制编辑器中，看看这是否可能。通过将几百个字节复制到丢失文件的前面，文件得到了足够的纠正，MP3 播放器可以重建该文件。

这并不完美——采访的前 50 秒是乱码。不过，面试的其余部分被保留了下来，这比失去整个面试要好得多。感谢[列文]送来这封信。

[https://www.youtube.com/embed/IHSCVdF8YYU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/IHSCVdF8YYU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)