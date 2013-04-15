---
layout: default
title: Yoda 表示法错在哪里
---


在上一篇[博文](http://www.yinwang.org/blog-cn/2013/04/14/terminology/)里，我提到了 Yoda 表示法。


### Yoda Notation（Yoda 表示法）

![](http://www.yinwang.org/images/yoda-notation.jpeg)


它的含义是，在 C/C++ 里面使用这样的表达式顺序：

    if ("blue" == theSky) ...

这是为了避免意外的写成：

    if (theSky = "blue") ...

“Yoda 表示法”的名字来源于《星球大战》的 Yoda 大师。他说话的单词顺序相当奇特，比如：“Backwards it is, yes!”

一般人认为：使用这个表示法是为了“变通”（wordaround） C/C++ 的一个设计抉择：使用 `=` 来表示赋值，而使用 `==` 来表示比较。这个设计充分的展现了“先辈的罪过”（Sins of our Forefathers）这一词汇的精髓。

我认为：使用 `=` 来表示赋值其实并没有错。真正的错误在于 

> C/C++ 的赋值语句不应该可以返回一个值

就是说，`theSky = "blue"` 不应该是一个“表达式”。也就是说你不应该可以把它放进 `if (...)` 的“条件”里面。如果你真的要赋值又要判断，你应该把这拆开成两行：

    theSky = "blue";
    if (theSky) ...

更近一步。`if (theSky) ...` 这个写法其实也是一个先辈的罪过。theSky 的类型是字符串，它不应该可以直接被作为 bool 使用。`if (...)` 的条件应该必须是一个 bool。 所以这里其实应该写成：

    theSky = "blue";
    if (theSky != NULL) ...

显然这样一来，之前的那种错误就完全不可能出现了，我们也就根本没必要用 Yoda 表示法了。
