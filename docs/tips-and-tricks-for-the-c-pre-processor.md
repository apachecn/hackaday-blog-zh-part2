# C 预处理器的提示和技巧

> 原文：<https://hackaday.com/2013/10/17/tips-and-tricks-for-the-c-pre-processor/>

[![C Pre-processor](img/92dd1ef6a756c2fe127fd2f01b01a181.png)](http://hackaday.com/?attachment_id=105255)

C 预处理器可以帮助你编写更简洁、更容易理解的代码。它还可以让您创建一个由宏和#defines 组成的混乱的球。[s1axter] [写了一篇关于如何使用预处理器并保持头脑清醒的指南](http://www.mybitbox.com/tag/robust-code/ "Robust Code")。

我们已经看到了 C 预处理器的一些巧妙之处，比如一个[全加器实现](http://hackaday.com/2013/10/09/create-a-full-adder-using-the-c-preprocessor/ "Create a Full Adder Using the C Preprocessor")，但是这里侧重于更实际的用途。首先，[s1axter]通过编写简单的宏来解释预处理器如何处理您的代码。接下来是参数，以及元编程中' ## '指令的使用。最后，我们很好地解释了为什么在使用宏时需要担心作用域，以及如何通过使用“do {} while()”语句来保护代码。

如果你对嵌入式编程感兴趣，本指南将帮助你理解一些更复杂的预处理技术。这有助于使您的代码更加清晰，并在几行代码中抽象出硬件依赖性。