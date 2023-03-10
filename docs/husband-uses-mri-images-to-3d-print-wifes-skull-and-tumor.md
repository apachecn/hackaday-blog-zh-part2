# 丈夫用核磁共振成像 3D 打印妻子的头骨和肿瘤

> 原文：<https://hackaday.com/2015/01/17/husband-uses-mri-images-to-3d-print-wifes-skull-and-tumor/>

[Michael Balzer]向我们展示了，在医疗保健方面，你是自己最好的倡导者——[能够打印自己的肿瘤模型是一个额外的收获](http://makezine.com/magazine/hands-on-health-care/)。迈克尔的妻子帕梅拉刚从 T2 的甲状腺切除术中恢复过来，就开始头疼。在第一位放射科医生驳回了她的头部核磁共振扫描后，她寻求第二种意见——并得知她左眼后面有一个 3 厘米长的肿瘤，一个[脑膜瘤](http://en.wikipedia.org/wiki/Meningioma)。 [All Things 3D](http://allthings3d.net/index.html) 的主持人【迈克尔】从她的核磁共振成像中要了 DICOM 文件(标准医学图像格式)。当帕梅拉进行随访时，肿瘤看起来已经开始迅速生长；这是一场虚惊。当[Michael]在 Photoshop 中比较两组 DICOM 图像时，第二次 MRI 没有真正显示肿瘤已经生长。它只是看起来那样，因为放射科医生从不同的角度进行扫描！不用说，这对夫妇对这次误诊很不高兴。

然而，脑膜瘤仍然给帕梅拉带来严重的问题。她面临失明的风险，所以她开始研究切除肿瘤所需的手术。最常见的外科手术是开颅手术:将颅骨锯开，将大脑提起，以便触及其下方的肿瘤。不足为奇的是，如果大脑以错误的方式移动，这将带来对任何神经造成永久性损伤的高风险，导致嗅觉、味觉或视力的丧失。帕梅拉决定寻找一种侵入性更小的替代手术。[迈克尔]从她的核磁共振成像中创建了她的头骨和脑膜瘤的 3D 打印图。他使用了 [InVesalius](http://svn.softwarepublico.gov.br/trac/invesalius) ，这是一款免费软件，用于将 2D DICOM 文件转换成 3D 图像。然后，他将 3D 渲染的头骨上传到 Sketchfab，与潜在的神经学家分享。一旦找到愿意考虑替代手术的神经科医生，[迈克尔]就打印出头骨，并把它送给医生。在设计新的手术过程中，打印是不可或缺的，在这个过程中，一个微型钻头通过左眼睑插入肿瘤。最终， [95%的肿瘤被切除，留下了最小的疤痕](https://sketchfab.com/models/2dab8ac4176f4710a7269d5226878c21)，她的视力得以保全。

如果你想[打印自己的核磁共振或 CT 扫描图](hackaday.com/2014/06/22/converting-cts-and-mris-into-printable-objects/)，不管是为了医疗用途还是为了[用自己的杯子做一个很酷的杯子](http://hackaday.com/2013/12/19/from-ct-scans-to-3d-prints/)，有很多程序可以提供帮助。除了前面提到的 InVesalius，还有 DeVIDE、Seg3D、ImageVis3D 和 MeshLab 或 MeshMixer。