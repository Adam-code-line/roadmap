# Python 学习路线

> 写在前面：对于本人来说，我的 Python 是在高中学校里学的，高中教材涉及的范围很广但不精，包括但不限于网络编程（Flask 框架）、嵌入式开发（开发板）、数据科学（numpy, pandas, matplotlab等等）。因此，下面我所写的 Python 学习路线并不能反映本人学习 Python 的真正路径，只是我认为可能适合大学同学的一种学习路线。当然，虽然这篇学习路线更加偏向于后端开发/网络编程，我也希望大家能借此爱上 Python，多多尝试在不同领域的应用，掌握这个啥都能干的工具。

## Python 环境安装

Python 是解释型语言，无需编译，只需要一个 Python 解释器就可以执行，真正做到了 **Run Anywhere** 。Python 环境安装实际上就是准备 Python 的解释器。不同的 Python 代码会使用到不同的包，可能存在依赖冲突，所以建议一开始就使用 **Anaconda** 管理 Python 虚拟环境，给你的电脑一个干净的 Python 环境。当然 **Anaconda** 为人诟病的一点就是环境过于臃肿，因此也可以选择精简版的 **Miniconda** 。

怎么选择？请看：[【Python】Anaconda和Miniconda的区别-CSDN博客](https://blog.csdn.net/u013172930/article/details/146040467)

* Anaconda 官网：[Advance AI with Open Source | Anaconda](https://www.anaconda.com/) 可以在里面找到 Anaconda 和 Miniconda 的安装包。
* [Anaconda安装教程（2025年保姆级超详解）【附安装包+环境玩转指南】 - 知乎](https://zhuanlan.zhihu.com/p/1896552549621936802)
* [【2025最新版】Miniconda3安装教程超详细图文教程（附完整安装包） - 知乎](https://zhuanlan.zhihu.com/p/1908614432663250054)

## Python 编辑器/IDE

* IDLE Shell

  与 Python 相捆绑的官方编辑器，功能简单，界面简朴，但好处就是无需专门安装，初学者刚开始学习基础语法时可以考虑使用这个。

* VSCode

  轻量级但具有良好扩展性的知名IDE。配置 Python 详见：[【教程】vscode+anaconda配置python环境](https://sazerac-kk.github.io/p/教程vscode-anaconda配置python环境/)（PS：这是我们wkk学长的教程，在bing的搜索结果里面意外地靠前）

* PyCharm

  JetBrains 出品的 Python IDE，个人的首选，功能丰富，工程化大项目必备，而且基本上也是开箱即用。对于 Python 后端开发来讲，PyCharm 拥有 Flask、Django、FastAPI 等框架的支持，基本上可以说是最合适的 IDE 了。官网：[PyCharm: The only Python IDE you need](https://www.jetbrains.com/zh-cn/pycharm/)

还有其他的一些选择：Spyder（数据科学专精）、Jupyter Notebook（与文档结合、交互式）、Thonny 等等。

## 语法

在此之前，我要提一下大名鼎鼎的 **“Python 之禅”**。

```
>>> import this
The Zen of Python, by Tim Peters

Beautiful is better than ugly.
Explicit is better than implicit.
Simple is better than complex.
Complex is better than complicated.
Flat is better than nested.
Sparse is better than dense.
Readability counts.
Special cases aren't special enough to break the rules.
Although practicality beats purity.
Errors should never pass silently.
Unless explicitly silenced.
In the face of ambiguity, refuse the temptation to guess.
There should be one-- and preferably only one --obvious way to do it.
Although that way may not be obvious at first unless you're Dutch.
Now is better than never.
Although never is often better than *right* now.
If the implementation is hard to explain, it's a bad idea.
If the implementation is easy to explain, it may be a good idea.
Namespaces are one honking great idea -- let's do more of those!
```

我认为任何一个学习 Python 的同学都应该看一看这一段话，每一个人对于编程可能都会有自己的看法，也可能都会有自己的一些习惯，但这一段话所反映的设计理念绝对会对 Python 学习有益。

* 优美优于丑陋(Beautiful is better than ugly)
* 明了优于隐晦(Explicit is better than implicit)
* 简单优于复杂(Simple is better than complex)
* 复杂优于凌乱(Complex is better than complicated)
* 扁平优于嵌套(Flat is better than nested)
* 稀疏优于稠密(Sparse is better than dense)
* 可读性很重要(Readability counts)
* 即使实用比纯粹更优, 特例亦不可违背原则(Special cases aren't special enough to break the rules, Although practicality beats purity)
* 错误绝不能悄悄忽略, 除非它明确需要如此(Errors should never pass silently, Unless explicitly silenced.)
* 面对不确定性，拒绝妄加猜测(In the face of ambiguity, refuse the temptation to guess)
* 任何问题应有一种，且最好只有一种，显而易见的解决方法(There should be one—and preferably only one—obvious way to do it)
* 尽管这方法一开始并非如此直观，除非你是荷兰人(Although that way may not be obvious at first unless you're Dutch)
* 做优于不做，然而不假思索还不如不做(Now is better than never, Although never is often better than right now)
* 很难解释的，必然是坏方法。很好解释的，可能是好方法(If the implementation is hard to explain, it's a bad idea.If the implementation is easy to explain, it may be a good idea.)
* 命名空间是个绝妙的主意，我们应好好利用它(Namespaces are one honking great idea—let's do more of those)

简单来说，Python致力于简化程序员的工作，让一切都变得简明、清晰、优美。每一条原则对应的具体内涵就等大家自己去体会了。

### 基础语法学习要点

- 变量
  - 定义变量
  - 关键字
  - 命名规则
  - 基本数据类型
  - 类型转换
- 运算符和表达式
- 流程控制
  - 条件分支
  - 循环
- 基本数据结构
  - 字符串
  - 列表
  - 元组
  - 集合
  - 字典
- 函数
  - 定义
  - 参数传递
  - 作用域
  - lambda 表达式
  - 常用内置函数
- 模块
  - 导入模块
  - 常用模块
- 包
  - 导入包
  - 生成包
- 异常处理
  - 捕获异常
  - try ... else ... finally 结构
  - 自定义异常
- 文件操作
  - 文件开闭
  - 文件读写
- 面向对象编程
  - 类和对象
  - 三大特性
    - 封装
      - self
      - 属性
      - 方法
        - 类方法
        - 实例方法
        - 静态方法
      - 访问控制
    - 继承
      - 单继承
      - 多继承
    - 多态
      - 方法重写
  - 运算符重载
  - 装饰器
  - 反射

### 资源

* [花了2万多买的Python教程全套，现在分享给大家，入门到精通(Python全栈开发教程)_哔哩哔哩_bilibili](https://www.bilibili.com/video/BV1wD4y1o7AS/?vd_source=8b3f1597864c695baad02815a988028e)
* [黑马程序员Python教程_600集Python从入门到精通教程（懂中文就能学会）_哔哩哔哩_bilibili](https://www.bilibili.com/video/BV1ex411x7Em/?vd_source=8b3f1597864c695baad02815a988028e)
* [Python3 教程 | 菜鸟教程](https://www.runoob.com/python3/python3-tutorial.html)
* [Python教程 - 廖雪峰的官方网站](https://liaoxuefeng.com/books/python/introduction/index.html)
* [styleguide | Style guides for Google-originated open-source projects](https://google.github.io/styleguide/pyguide.html)

实际上 Python 的语法真的是非常简单，上手飞快，学就完事了。

## 进阶知识

这一部分可能并不是 Python 的专属，但是如果你想要用 Python 进行网络编程与后端开发，你可能会用到它们。

* 正则表达式
  * [Regex Learn - 逐步从零基础到高阶。](https://regexlearn.com/zh-cn)
* 异步与多线程
  * [Python并发总结：多线程、多进程与异步编程 - wang_yb - 博客园](https://www.cnblogs.com/wang_yb/p/18643761)

* 数据结构与算法（可能没必要专门学，学校大二的课程够用）
  * [【北京大学】数据结构与算法Python版（完整版）_哔哩哔哩_bilibili](https://www.bilibili.com/video/BV1VC4y1x7uv/?vd_source=8b3f1597864c695baad02815a988028e)
* 数据库编程（包括 SQL 基础与 Python 数据库连接）
  * [Python + MySQL 0基础从入门到精通 MySQL数据库实战精讲教程（2021精华版）_哔哩哔哩_bilibili](https://www.bilibili.com/video/BV1B34y1R7in/?spm_id_from=333.337.search-card.all.click&vd_source=8b3f1597864c695baad02815a988028e)（不一定要 MySQL，其他数据库也是一样的）
* 前端基础（HTML + CSS + JavaScript）（现在有 AI，可能不那么重要了，但是得多少懂一点吧）
  * [3小时前端入门教程（HTML+CSS+JS）_哔哩哔哩_bilibili](https://www.bilibili.com/video/BV1BT4y1W7Aw/?spm_id_from=333.337.search-card.all.click&vd_source=8b3f1597864c695baad02815a988028e)

* 网络编程
  * [最实用的Python网络编程（完整版）_哔哩哔哩_bilibili](https://www.bilibili.com/video/BV1aq4y137T6/?spm_id_from=333.337.search-card.all.click&vd_source=8b3f1597864c695baad02815a988028e)

## Flask

* 官方文档：[欢迎来到 Flask 的世界 — Flask Documentation (3.1.x)](https://flask.palletsprojects.com/zh-cn/stable/)
* [Flask 中文网](https://flask.github.net.cn/)
* [Flask 入门教程 - HelloFlask](https://helloflask.com/book/3/)个人觉得非常易懂的文字教程。
* 视频教程与后端实战：[【最快速度搞定Flask-框架教程】用5小时讲完的python-flask项目实战全套教程-学完直接就业！flask服务，flask平台等入门到精通web开发_哔哩哔哩_bilibili](https://www.bilibili.com/video/BV11PoTYkEE1/?spm_id_from=333.337.search-card.all.click&vd_source=8b3f1597864c695baad02815a988028e)
* 实战（带前端）：[90分钟用Python和Flask开发博客系统_哔哩哔哩_bilibili](https://www.bilibili.com/video/BV1gh411q7xo/?spm_id_from=333.337.search-card.all.click&vd_source=8b3f1597864c695baad02815a988028e)

## Django

* 官方文档：[The web framework for perfectionists with deadlines | Django](https://www.djangoproject.com/)
* 视频教程与实战：[2025版-零基础玩转Python Django5项目实战-学完可就业_哔哩哔哩_bilibili](https://www.bilibili.com/video/BV1N1421U76L/?spm_id_from=333.337.search-card.all.click&vd_source=8b3f1597864c695baad02815a988028e)
* Python + 微信小程序实战开发：[18天学会 Python+微信小程序实战开发（全套课程）_哔哩哔哩_bilibili](https://www.bilibili.com/video/BV1Xy4y1s792/?vd_source=8b3f1597864c695baad02815a988028e)

## FastAPI

待更新……