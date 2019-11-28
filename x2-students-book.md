# 如何使用配套学习用书

> “A dream written down with a date becomes a goal. A goal broken down into steps becomes a plan.”
> 
> ― Greg Reid

使用“学习用书”不仅可以帮助边学边练，还是你的学习跟踪记录，你的 *proof of work*。要使用学习用书，按照下面的步骤顺序操作：

### 登录 GitHub

无论如何你都必须有 GitHub 账户，GitHub 是个神奇的地方，不仅可以帮助程序员，还可以帮助很多非程序员实现奇妙的社会化大合作。

当然，这很简单，访问 [github.com](https://github.com)，注册一个 GitHub 帐号（如果还没有的话）并登录。

### 获取你的学习用书

第一步，访问本书配套学习用书的共享代码仓库（*repo*），

> [https://github.com/neolee/pilot-student](https://github.com/neolee/pilot-student)

点击右上角的 Fork 按钮，这是 git 的重要操作，它会从我们的 *repo* 分叉出一个一模一样的 *repo* 并加入到你的账号中，这个新的 *repo* 继承了原 *repo* 的历史和现状，但它的未来由你来决定。

在这个新的 *repo* 的首页上有个绿色的 *Clone or download* 按钮，点击它会打开一个小的下拉显示，里面有个文本框写有这个 *repo* 的访问地址，点击它右边的小按钮将其拷贝到系统剪贴板（后面会用）。

第二步，现在要把属于你的这个分叉 *repo* 克隆到你自己的机器本地来，由于你顺利完成了[环境准备](x1-setup.md)，你的机器上已经有完善的命令行界面和软件包管理工具，还装好了 *git*，现在可以打开命令行界面进行如下操作：
* 输入 `cd Code ↩︎` 进入我们之前创建的子目录（如果还没有建立，可以用 `mkdir Code ↩︎` 来创建）；
* 输入 `git clone `，在最后有个空格，在空格后粘贴你前面拷贝的，你 *fork* 的 *repo* 的地址，然后输入回车 `↩︎`；
* 输入 `cd pilot-student ↩︎` 进入克隆好的目录中。

上面的命令会在 `<你的用户根目录>/Code` 目录下创建一个子目录，然后把学习用书从 GitHub 服务器上克隆到这个目录下。

### 安装和运行 Jupyter Lab

因为学习用书都是用 Jupyter Notebook 写就的，要使用就需要安装 Jupyter Lab 环境，在我们已经装好 Python 的前提下这很容易，只要在命令行界面运行下面的命令就可以了：

```shell
python -m pip install --upgrade pip
pip install jupyterlab
```

`pip` 是 Python 自己的软件包管理工具，它负责安装、删除和管理 Python 浩若烟海的第三方代码库，我们以后会经常用到。上面第一行是更新 `pip` 自己，因为我们刚装好 Python，通常需要更新一下 `pip` 自己；第二行则是让 `pip` 安装 Jupyter Lab 以及所有依赖支持包。

> 如果在运行上面第二个命令时报错说找不到、不认识 `pip` 命令，可尝试将 `pip` 换成 `pip3`，即运行 `pip3 install jupyterlab`。

某些环境下运行 Jupyter Lab 需要 nodejs，所以建议也安装好。如果是 Winidows 系统，执行：

```powershell
scoop install nodejs
```

macOS 系统则执行：

```shell
brew install node
```

上述操作都成功后 Jupyter Lab 就准备就绪了，在你克隆好的学习用书目录里运行 `jupyter lab ↩︎` 来启动 Jupyter Lab 的服务程序，并打开一个浏览器页面，里面列出了学习用书里的所有 *notebook*（.ipynb 后缀名的文件），双击就能打开了。

> 注意，运行 `jupyter lab` 的命令行窗口必须保持着，你才能继续在浏览器里使用 Jupyter Lab；如果你用完了，需要退出，在这个命令行窗口按 Control+C 组合键，就会停止 Jupyter Lab 服务，回到命令行交互界面。一般来说不要在 `jupyter lab` 运行时关闭那个窗口。
> 
> 如果在 `jupyter lab` 运行着的时候你需要命令行界面执行一些任务，只要在 ConEmu 里打开一个新的 tab 就可以了，不用动之前的那个。

### 使用学习用书

现在你可以在 Jupyter Lab 中打开 *notebook*，在代码 *cell* 中输入 Python 代码并运行，每学完一章，对应的学习用书中的 *notebook* 也应该经你亲手补完，你当然还可以在 *notebook* 中加入自己的想法，测试自己想到的程序代码等等，总之只要你想做的都可以做，做完之后保存 *notebook*，你的成果就被记录下来了，然后你可以：

* 使用 `git commit` 来把你修改的内容提交到本地仓库（*local repo*）；
* 使用 `git push` 来把你本地仓库中新的变化同步到 GitHub 上的远程仓库（*remote repo*）——这就是你的学习“工作证明（PoW）”。

在学习用书的代码仓库中还有一个特殊的目录 `vor`，意思是 *Voice of Readers*，用来收集像你一样的学习者的反馈，比如你可以写一篇《我的自学之路》，放在这个目录里，然后 *commit* 和 *push* 到你自己的学习用书 *repo* 中，甚至还可以用一种特定流程（叫做 *pull request*）提交回我们的原 *repo* 中，如果被我们接受，就会成为原 *repo* 的内容，被所有读者 *fork* 和阅读。

当然了，上面说的这些都需要你多学一样反正你早晚都必须学会的东西——*git*，我们在附录中有一篇 [Git 与 GitHub 入门教程](x3-git-github.ipynb) 可以参考。

学习需要投入时间，而时间我们没办法糊弄它。

有了 *git* 这样的工具之后，我们在什么时候做了什么样的工作，是很容易证明的，而当我们不小心犯了错误还能回溯到历史版本，相当于我们从某种程度上获得了一些对时间的控制力——这对我们来说真是天大的好事。

未来，我们会专门设置一个 *repo*，通过自动扫描学习用书所有 *forks* 来跟进本书的学习记录——这种记录在过往的书籍中是不可能存在的，然而现在却可以了。将来这种记录的作用甚至有可能比“学历”还要重要。

关于学习环境的准备，还可参考这个 [视频指引](https://www.bilibili.com/video/av71399509/)。

### 问题与反馈

如果在学习过程中遇到问题或者发现教材中的错误，可以通过 GitHub 的 Issues 系统提出，这个系统基本上就像一个问答论坛，但它集成了编程相关的能力，让它目的性更强、更容易跟踪问题解决的进度状态。

访问我们课程教材的 Issues 页面：

> [https://github.com/neolee/pilot/issues](https://github.com/neolee/pilot/issues)

点击右上的 `New` 按钮来提出问题或者反馈，如果是问题请选择 `question` 这个 *label*，如果是关于教材中的错误或者改进建议可以选择 `bug` 或者 `enhancement` 这样的 *label*。

遇到问题的时候其实也可以到这个页面去搜索一下，看看是不是有人提过，得到了怎样的答案；如果没人提过，那就正好可以由你来提出，所有人也都会从中获益。

有些常见或者特别有价值的问题我们也会整理出来放到课程项目的 [Wiki](https://github.com/neolee/pilot/wiki) 中，方便大家查阅。
