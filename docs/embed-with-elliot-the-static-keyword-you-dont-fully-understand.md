# 嵌入埃利奥特:你不完全理解的静态关键词

> 原文：<https://hackaday.com/2015/08/04/embed-with-elliot-the-static-keyword-you-dont-fully-understand/>

我们最喜欢的 C 编程语言(及其后代)的细微差别之一是`static`关键字。开始时，要了解它有点棘手，因为在不同的情况下，它可能有两个(或三个)微妙不同的应用程序，但它非常有用，值得花时间去了解。

在 Arduino 用户点击离开之前，静态变量解决了 Arduino 编程中出现的一些常见问题。进行这个测试，看看它对你是否重要:下面的 Arduino 片段会打印出“Hello World”吗？

```

void loop()
{
	int count=0;
	count = count + 1;
	if (count > 10) {
		Serial.println("Hello World");
	}
}

```

如果你说“是”，你绝对需要阅读这篇文章。如果你说“不，你需要将`count`定义为`loop()`之外的全局变量，傻瓜！”，原则上你得到了正确的答案，但是将变量定义为`static`更好。我们会知道为什么。

但是这篇文章最简短的总结如下:如果你想让一个变量在包含它的函数调用之间保持它的值，那么声明这个变量 [static](https://en.wikipedia.org/wiki/Static_variable) 。

基本原理是，将变量声明为静态变量会将作用域设置为局部的，但会使变量在程序的整个生命周期中都存在，而不仅仅是在定义它的函数调用中存在。这意味着它不会在每次调用函数时重新初始化，这让我们可以有效地在函数中存储数据。这是程序员工具箱中的一个很好的技巧。

## 范围和期限

为了理解`static`，我们必须将变量对我们代码的可用性的两个相关概念分开:[范围](https://en.wikipedia.org/wiki/Scope_(computer_science))和[持续时间(或生命周期)](https://en.wikipedia.org/wiki/Object_lifetime)。

你们大多数人都知道可变作用域。在许多语言中，如果你在一个函数或块中声明了一个变量，它就留在这个函数或块中。这被称为“局部作用域”或“函数作用域”或类似的东西。如果我们的函数没有显式地将变量传递出去，其他函数就不能使用这个变量。这很棒，因为这意味着你可以命名所有的计数器变量`count`，并且它们不会在函数间相互冲突。你可能知道这个。

C & Co .中的变量也有一个保证可用的生命周期，也称为“持续时间”。在它们的持续时间结束后，您将不能再使用该变量。这与“作用域”的概念密切相关，作用域指定了变量在代码的哪个功能块中可用，但是您会希望在头脑中把它们分开。最简单的方法是将持续时间视为一个时间，将范围视为一个位置(在代码空间中)。

变量的默认持续时间是函数的当前调用。这就是为什么类似于:

```

int counter (void)
{
	int count=0;
	count=count+1;
	return count;
}

```

将始终返回 1。每次调用函数时，`count`被重新初始化为零，当函数返回时，该变量的存储被重新分配，因为它有函数持续时间。(而这正是上面 Arduino 片段的问题。)

我们希望我们的`counter()`函数记录它被调用的次数。我们需要变量`count`具有程序持续时间——只要我们的代码在运行，它就需要存在，而不是在每次函数调用后被重新分配。

### Globals？

强力方法是将`count`声明为一个[全局变量](https://en.wikipedia.org/wiki/Global_variables)，方法是在任何函数之外定义它。全局变量在程序持续期间是有效的，所以包含在`count`中的值将保持可用。到目前为止，一切顺利。但是全局变量的副作用是使得`count`可以从任何其他函数中使用。有时候这正是我们想要的，但很多时候不是。

全局作用域的问题是你不能使用任何其他同名的全局变量，所以你需要小心地选择名字以保持唯一，这样它们就不会冲突。如果你只是使用长的、特定的名字，这并不是一个大问题:例如，`My_Global_Loop_Counter`而不是`count`。

当您打算在第二个函数中使用另一个名为`count`的变量，但忘记声明它时，会出现一个更微妙的问题。第二个函数认为您打算使用全局定义的`count`，于是混乱随之而来。

最后，使用全局变量在不同的函数之间传递数据很有诱惑力。(对于那些还没有适应[指针](https://en.wikipedia.org/wiki/Pointer_(computer_programming))和[结构](https://en.wikipedia.org/wiki/Struct_(C_programming_language))的人来说尤其如此。)如果您使用一个全局变量将函数分布在不同的文件中，那么要跟踪一个流行的全局变量被访问或修改的每一个位置，就需要进行大量的调试工作。也就是说，全局变量*会*导致代码支离破碎，难以调试。

### 不，是静电。

无论如何，如果你买了上面的论点，你真正想要的是一个有程序持续时间但有函数作用域的变量。这正是`static`在应用于函数内部的变量时所做的。这种语言正好具有您想要的特性，所以您不妨使用它。

为了说明这一点，上面的 Arduino 代码片段将与一个全局定义的`count`变量一起工作，

```

int count;
void loop()
{
	count = count + 1;
	if (count > 10) {
		Serial.println("Hello World");
	}
}

```

但是当使用`static`编写时，它也更加简洁:

```

void loop()
{
	static int count;
	count = count + 1;
	if (count > 10) {
		Serial.println("Hello World");
	}
}

```

因为“伯爵”这个名字不是全球公开的。它也在使用它的函数中声明，所以不存在它属于谁的问题。这很有效。你不能打败它。

静态和全局变量(所有带程序持续时间的变量)默认预初始化为零，所以我们不需要写上面的`static int count = 0;`。然而，如果我们希望初始值不为零，我们可以这样定义变量:`static int count = 42;`。

然而`static int count = 42;`有些令人毛骨悚然。看起来好像我们在声明变量，然后在每次通过代码时设置它的值。但是`static`关键字阻止了这一点。相信我们，或者修改上面的演示代码来亲自测试一下。

## 数据隐藏和单例等等

还有第二个相关的用法需要提及。当在任何函数之外使用时，在文件的顶层，`static`将范围限制在所讨论的文件。相比之下，全局变量具有真正的全局范围，因此可以跨文件使用。`Static`在函数之外定义的变量就像一个准全局变量:在程序运行期间，在文件内定义的每个函数都可以使用它，但在文件之外却不能使用。

这是一个这种准全局功能非常有用的例子。假设我们想将计数器代码分离到一个计数器库中。我们从这样的事情开始:

```

int counter(void){
	static int count;
	count++;
	return count;
}

```

每次从其他代码中调用`counter()`时，该函数会保留旧的值`count`，并加 1，计数器就会像它应该的那样工作。这是函数范围的静态定义。

但是现在想象一下，我们也想重置计数器。我们可能需要一个`reset()`函数将值设置回零。但是`count`有函数作用域，所以我们的`reset()`函数就碰不到它了。这里的解决方案是在文件范围内使用静态类型声明。

在您的文件“counter.c”中可能会有这样的内容:

```

static int count;

int counter(void){
	count++;
	return count;
}

void reset_count(void){
	count = 0;
}

static void my_secret_function(void){
	count = 42;
}

```

因为`count`在文件范围内被定义为静态的，所以文件中的所有函数都可以使用它，并且该值在函数调用之间保持不变。此外，因为`my_secret_function()`被定义为静态的，所以不能从这个文件外部调用，尽管这里定义的函数可以像往常一样调用它。

在文件范围内定义静态变量(和函数)非常适合存储库所需的特定于库的内容，但不需要在外部看到。这很像面向对象语言对公共和私有数据和方法的处理。

然而，与面向对象模式相比，我们只有一个数据实例。你不能轻易创造第二个。这就是软件工程师所谓的[单例](https://en.wikipedia.org/wiki/Singleton_pattern)。这些单例非常适合跟踪全局状态，您只需编写一些简单的函数来修改和访问数据。由于数据是`static`和文件本地的，您知道您不能从外部搞乱它，并且操作函数在您可以`#include`它们的任何地方都可用。

单例的缺点是它们只有一个。例如，如果您想要两个计数器，这段代码不会有帮助。当您遇到这种情况时，您将需要全面的面向对象支持。

## …还有 Arduino

这是大量的 C 理论，所以如果你用 Arduino 编程，你可能会认为它不适用。如果你这样想，你在最后一次“嵌入”时没有注意；Arduino 是 C/C++，增加了便利库。事实上，Arduino 反复调用`loop()`函数的特殊方式使得了解一点作用域变得几乎是强制性的:除非你做些什么，否则每次循环中所有的函数调用持续时间变量都会被清除。

正如我们在介绍性的例子中看到的，如果不在每次循环中重置变量，就无法初始化`loop()`中的变量。如果您不知道`static`关键字，您可能会采用强力解决方案，将变量定义为全局变量。许多 Arduino 示例就是这样做的。

什么会出错？

```

int i;

void loop(){
	i++;
	Serial.println(i);
	delay(100);
	doSomethingTwice();
}

void doSomethingTwice(){
	for (i=0; i<2; i++){
		Serial.println("twice?");
	}
}

```

好吧，假设你已经习惯了，就像我们一样，使用`i`作为一个通用的循环变量。假设您在另一个函数中重用了它而没有定义，甚至可能是在另一个函数中。ino "文件，您可以从循环中调用它。因为`i`是一个全局变量，意外的第二次使用实际上是完全合理的。编译器不能帮你找到错误，但是你的程序不能正常工作。可怜的 Arduino 不会向上计数，只会一直印“3”。

这个问题有两个原因:忘记在`doSomethingTwice()`中声明`i`，以及创建一个具有易于重用名称的全局变量。你*会*不时忘记声明变量。我们都是。当我们这样做时，我们希望编译器让我们知道。

所以有两种方法可以避免这个问题。第一个解决方案是给全局变量起个疯狂的名字，这样它们就不太可能被重用。“我的神奇的全球循环计数器”会很好用。甚至打一次就让我再也不想打了。

“正确”的解决方案解决了最初导致我们使用全局变量的问题。我们简单地将计数器变量定义为`loop()`内部的静态变量，然后它有程序持续时间，但有函数范围，一切正常。现在我们甚至可以不受惩罚地调用计数器变量`i`，因为它的作用域是`loop()`。

```

void loop(){
	static int i;
	i++;
	Serial.println(i);
	delay(100);
	doSomethingTwice();
}

void doSomethingTwice(){
	// You'll get an error here b/c i isn't declared.  Thanks, compiler!
	for (i=0; i<2; i++){
		Serial.println("twice?");
	}
}

```

如果您想在一个“草图”中的不同函数之间共享变量，该怎么做呢？一种方法是直接将它们作为参数传递，但是你会再次看到许多人求助于全局变量，这些变量可以简单地从每个相关函数中访问。如果你注意给变量起好名字，这不是一个大问题，所以我们不会坚持。

但是您也可以“正确地”这样做，在文件级别将全局变量定义为`static`。您仍然可以在自己的函数中犯一些细微的错误，但是通过声明变量`static`，您就不会将它们与 Arduino 基础设施中其他地方定义的变量混淆。当你已经穿着吊带裤的时候，它就是一条腰带，但是除了多一点点打字之外，它不会花费你任何东西。

## 结论

当您希望值在函数调用中保持不变，但又不需要扩大范围时，可以对函数中的变量使用`static`关键字。当您希望函数和变量的行为类似于准全局变量时，在文件级对它们使用`static`关键字，它们在文件内的任何地方都是可访问的，但对外部是隐藏的。

看到了吗？那毕竟没那么神秘。