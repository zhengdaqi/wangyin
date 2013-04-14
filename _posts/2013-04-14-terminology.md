---
layout: default
title: 几个超炫的专业词汇
---

从同事的[博客](http://thomas.tuerke.net/on/design/?thread=-701829031)上学会了几个超炫的专业词汇，激动不已。觉得这些词汇可以言简意赅的概括我的好几篇博文，自己的文章水准真是自愧不如。现在来见识一下真正大师级的英语词汇：


* Yoda Notation（Yoda 表示法）

  在 C/C++ 里面使用这样的表达式顺序：

      if ("blue" == theSky) ...

  这是为了避免意外的写成：

      if (theSky = "blue") ...

  “Yoda 表示法”的名字来源于《星球大战》的 Yoda 大师。他说话的单词顺序相当奇特，比如：“Backwards it is, yes!”

  使用这个表示法是为了“绕过”C/C++的一个设计抉择：使用`=`来表示赋值，而使用`==`来表示比较。这充分的展现了“先辈的罪过”（Sins of our Forefathers）这一词汇的精髓。

* Mental Speedbump（头脑减速杠）

![](http://www.yinwang.org/images/speedbump.jpeg)

  由于设计的不协调性造成的用户的注意力分散。比如，很多软件喜欢弹出一个窗口问你“是否继续？”

* Pearl Effect （珍珠效应）

  由于早期的设计缺陷，而让用户不得不采用的“变通方案”或者“附加过程”。它们其实没有珍珠那么好看。（请比较：Sins of our Forefathers）

* Sins of our Forefathers（先辈的罪过）

  在当时看起来合乎逻辑并且合情合理的历史遗留设计，最后回顾起来真的很傻b。与 Pearl 相比，这些是有意识的加进去的，而不是不小心的错误，虽然这两者都会造成“变通”（workaround）。

* Katrina Effect（卡特里娜飓风效应）

  这个词描述的是一种飓风过后完全重头来过的悲惨景象。这种现象现在经常出现在重装或者升级软件之后，或者 Windows 安装完软件之后要你重启机器（关掉所有窗口）。

* Wordaround

  因为开发过程的失败而让用户必须进行的一些操作。这些通常是设计失误。
