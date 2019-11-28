# 进入编程世界的第一课

## 更新

第二阶段课程（S2）已发布， 请阅读 [对 S2 课程的说明](README-S2.md)。

## 前言

这个仓库（*repo*）里保存的是**教材**，也就是需要你阅读和学习的内容。我们另外还有个 *repo* 是你的**学习用书**，我们会在下面告诉你如何使用这两个仓库。

编程（*programming*）并不算是一门**科学**，更像是一种**手艺**，里面有科学，有理论有思想，也有经验和体会。学习编程最有效的方法是——赶紧动手开始写程序，如果不自己动手，听再多、再牛的课程讲解也没用。

在动手写程序的前提下，优秀的课程才能发挥作用——那就是缩短你走弯路的时间，就好像学踢足球或者打高尔夫球，一开始就掌握**正确的姿势**很重要，之后就能够**事半功倍**。

这门课程就能够发挥这样的作用——但必须你亲手开始编程。

为了帮助你做到这一点，我们设计了一个学习方案，你的每个学习单元都由 **听课**、**自学** 和 **提问** 三个环节组成。

#### 听课

这部分以讲解原理和思维方法为主，重点在“学会学习的方法（*learning to learn*）”和“问题解决的方法（*problem solving*）”。

课程的讲解大致上每周一次，在课程讲解的最后会给大家布置自学任务，就是下面这个环节。

#### 自学

你要通过我们提供的教材和学习用书完成 **自学任务**。方法很简单：
* 使用下面的课程大纲打开指定章节进行阅读；
* 一边读一边在 **学习用书** 中完成代码的编写和运行。

我们的教材和学习用书都是用一种叫做 **Jupyter Notebook** 的格式编写的，这种格式编写的 *notebook* 中除了文字，还有**可运行的程序代码**（！）。

学习用书和教材的区别只有一个：在学习用书中，所有写着程序代码的格子（*cell*）都被清空了，等着你自己动手填进去。

所以学习用书就好像我们小时候学写字时用的“描红本”，你可以对着教材“描”和“抄”。不要小看了这个“描”和“抄”的过程，无数实践证明，自己输入一遍和光看就是不一样；而且，程序和描字不同，很多时候你可以自己修改一些地方，改的越多你就掌握的越多。

为了使用 **学习用书**，你首先需要配置好一个（你可以用一辈子的）编程环境，然后从我们的共享代码仓库获取学习用书并运行，具体来说按照下面的两个指引操作即可：

1. [编程环境配置指南](x1-setup.md)
2. [如何使用配套学习用书](x2-students-book.md)

自学过程中遇到问题是正常的，所以下面这个环节很重要。

#### 提问

我们鼓励大家提问，在学习过程中遇到问题就及时提出来，及时解决。

万事开头难，一开始快速清障前进，后面就会越来越顺。

可以使用 GitHub 提供的 Issues 功能来提问，只要访问 [这个页面](https://github.com/neolee/pilot/issues)，点击右上的 `New issue` 绿色按钮即可提出问题，记得选择 `question` 这个 *label*（如果提的是关于课程教材中的错误或者改进建议可以选择 `bug` 或者 `enhancement` 这样的 *label*）。

提问是有一些技巧的，经过思考的问题更容易得到靠谱答案。

关于这个问题，有个近乎标准的答案在网上已经存在很久了，那就是大牛 Eric S. Raymond 2001 年发表在 BBS 上的 [How To Ask Questions The Smart Way](http://www.catb.org/~esr/faqs/smart-questions.html)，这篇文章从发表之后一直在不断更新修订，内容清晰详实，附有丰富的“好问题”和“蠢问题”样例，一看就明白；另有质量很不错的 [中文译文](https://github.com/ryanhanwu/How-To-Ask-Questions-The-Smart-Way/blob/master/README-zh_CN.md)（也是开源的）。请务必仔细阅读，尽量按照里面的建议来思考和组织你的问题。

## 课程大纲

#### 第一部分 基础篇

* [第一章 理解编程语言](p1-1-understanding-programming-languages.ipynb)
* [第二章 程序的基本结构（一）：值与变量](p1-2-structure-1.ipynb)
* [第三章 程序的基本结构（二）：操作符与函数](p1-3-structure-2.ipynb)
* [第四章 程序的基本结构（三）：逻辑判断与分支](p1-4-structure-3.ipynb)
* [第五章 程序的基本结构（四）：循环](p1-5-structure-4.ipynb)
* [第六章 程序的基本结构（五）：异常处理](p1-6-structure-5.ipynb)
* [第七章 理解对象与类：起源篇](p1-7-oo-1.ipynb)
* [第八章 理解对象与类：概念篇](p1-8-oo-2.ipynb)
* [第九章 理解对象与类：Python 篇](p1-9-oo-3.ipynb)
* [第十章 字符与字符串](p1-a-string.ipynb)
* [最十一章 课程练习](p1-b-final.ipynb)

#### 第二部分 进阶篇

* [第一章 函数定义再探](p2-1-function-def.ipynb)
* [第二章 程序中的文档](p2-2-docstrings.ipynb)
* [第三章 模块](p2-3-modules.ipynb)
* [第四章 递归](p2-4-recursion.ipynb)
* [第五章 函数也是数据：初级篇](p2-5-functional-1.ipynb)
* [第六章 字符串数据](p2-6-string-data.ipynb)
* [第七章 Iterable 与 Iterator](p2-7-iterable-iterator.ipynb)
* [第八章 列表](p2-8-list.ipynb)
* [第九章 元组，集合，字典](p2-9-tuple-set-dict.ipynb)
* [第十章 树](p2-a-tree.ipynb)
* [第十一章 有限状态机](p2-b-fsm.ipynb)
* [第十二章 数据和数据库](p2-c-database.ipynb)
* [第十三章 函数也是数据：进阶篇](p2-d-functional-2.ipynb)

#### 附录

1. [编程环境配置指南](x1-setup.md)
2. [如何使用配套学习用书](x2-students-book.md)
3. [Git 与 GitHub 入门](x3-git-github.ipynb)
4. [正则表达式入门](x4-regex.ipynb)
5. [MySQL 配置指南](x5-mysql-setup.ipynb)
6. [Redis 配置指南](x6-redis-setup.ipynb)

#### 重要的附注

由于 GitHub 的某些 bug，点击上面的这些链接打开 *notebook* 时可能会出现 `Sorry, something went wrong. Reload?` 的错误，这时可打开下面的链接，改用 Jupyter Notebook 官方提供的阅读器：

> https://nbviewer.jupyter.org/github/neolee/pilot/tree/master/

`ipynb` 后缀的文件就是 *notebook* 文件，文件名最开始的数字对应第几章（`a` 对应第十章，`b` 对应最终章，`x` 开头的则是附录）。

比较推荐的学习方式是，用一个浏览器窗口打开上面列出的课程内容，同时在你自己机器的学生用书目录下运行 `jupyter lab`，并在学生用书的对应 *notebook* 下自己输入代码尝试。

具体可参考这个 [视频指引](https://www.bilibili.com/video/av71399509/)。

## 问题与反馈

如果在学习过程中遇到问题或者发现教材中的错误，可以通过 GitHub 的 Issues 系统提出，这个系统基本上就像一个问答论坛，但它集成了一些功能，让它目的性更强、更容易跟踪问题解决的进度状态。

访问我们课程教材的 Issues 页面：

> [https://github.com/neolee/pilot/issues](https://github.com/neolee/pilot/issues)

点击右上的 `New issue` 绿色按钮来提出问题或者反馈，如果是问题请选择 `question` 这个 *label*，如果是关于教材中的错误或者改进建议可以选择 `bug` 或者 `enhancement` 这样的 *label*。

遇到问题的时候其实也可以到这个 Issues 页面去搜索一下，看看是不是有人提过，得到了怎样的答案；如果没人提过，那就正好可以由你来提出，所有人都会从中获益。

有些常见或者特别有价值的问题我们会整理出来放到课程项目的 [Wiki](https://github.com/neolee/pilot/wiki) 中，方便大家查阅。