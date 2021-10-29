
# Text
## 前言
- Hard Way to learn Python 3
- 符合我做中学的学习理念
- PowerShell中通过D:切换到D盘, 无需cd

## ex1 第一个程序
- 练习print, 字符串通过双引号or单引号括起都可以
-  #（octothorpe）有很多的英文名字，如pound（英镑符）、hash（电话的#键）、mesh（网）等。选一个你觉得酷的用就行了
- 我接下来的任务, 配置我的neovim, 学习PowerShell
## ex2 注释和#号
## ex3 数字和数学计算
## ex4 变量和命名
## ex5 更多的变量和打印
- f"abc is {str}", format print
- round(), 四舍五入
## ex6 字符串和文本
- a=10, str="abcdef = {}", str.format(a)
## ex7 更多打印
## ex8 打印, 打印
- 更多的格式化, formatter="{} {} {} {}", formatter.format(1, 2, 3, 4)
## ex9 打印, 打印, 打印
- 多行字符串, """abc"""
- \n
## ex10 那是什么
- 转义序列
## ex11 提问
- print("How old are you? ", end=' ')
    - print完不换行, 把\n换成end
- age = input()
    - input()返回字符串, age = int(input()), 即可
## ex12 提示别人
- age = input("input your age ")
- pydoc input
    - Windows: python -m pydoc input
    - q for quit
## ex13 参数, 解包和变量
- import module
```python
# argv = argument variable
from sys import argv
# unpack
# they are all string type
name, a, b, c = argv

$ python a.py 1 2 3
```
## ex14 提示和传递
- f"""abc {d}""", 格式化与多行字符串结合
## ex15 读取文件
- file object
- file = open(filename), print(file.read()), file.close()
## ex16 读写文件
- readline, truncate清空, write("abc"), seek(0)
- open(filename, mode), default is r, others are w/r/a/w+/r+/a+
## ex17 更多文件操作
- from os.path import exists
- len(str)
## ex18 命名, 变量, 代码和函数
- def funcName(*args):
    - indentation
## ex19 函数和变量
- 讲变量的局部作用域
## ex20 函数和文件
- readline()返回的str会有\n, print时通过end=""避免打印2个\n
## ex21 函数可以返回某些东西
- return and a = funcName(1, 2)
## ex22 到现在为止你学到了什么
## ex23 字符串, 字节串和字符编码
- bit and byte
- ASCII and Unicode
    - 区分字符集和编码方式
    - UTF-8, Unicode Transformation Format 8 bits
- b''告诉Python处理的是原始字节串
- 从23开始重看



## ex27 记住逻辑关系
- and/or/not
## ex28 布尔表达式练习
- 为什么"test" and "test"返回"test",1 and 1返回1，而不是返回True呢？
    - Python和很多编程语言一样，都是给布尔表达式返回两个被操作对象中的一个，而非True或False。这意味着，如果你写了False and 1，得到的是第一个操作数（False），而非第二个操作数（1），但如果你写的是True and 1，得到的是第二个操作数（1）
- 短路运算
## ex29 if语句
## ex30 else和if
- Python有elif
## ex31 作出决定
## ex32 循环和列表
- list - []
- myList.append()
- for i in myList:
- for i range(0, 10): [0, 10)
## ex33 while循环
- while cond:
## ex34 访问列表的元素
- 通过下标, 从0开始
## ex35 分支和函数
- exit(0)
- input('>')
## ex36 设计和调试
- 不用while, emm, 见仁见智
## ex37 复习各种符号
![image.png](https://pic.rmb.bdstatic.com/bjh/7c44d321df3f68518e1dedf7ecd8deb0.png)
## ex38 列表的操作
- 切片
- 这本书, 不建议有基础的看, 太迷了
## ex39 字典, 可爱的字典
- dict - {}, k-v
## ex40 模块, 类和对象

## ex41 学习面向对象术语


## ex46 项目骨架
- pip list
- sudo pip/pip3.6 install virtualenv
- whereis virtualenv
- 这一节还有很多内容, 反复观看
- which python
- pip install nose, 测试框架

- 这两条命令创建了一个．venvs文件夹，用来存储不同的虚拟环境，然后为你创建了第一个虚拟环境，叫lpthw。虚拟环境就是一个用来安装软件的“假的”地方，这样你就可以针对不同项目使用不同版本的软件包了
    - 安装好以后你需要激活虚拟环境：
    - 这样就为PowerShell运行activate脚本，它把你当前的shell设为使用lpthw虚拟环境。每次使用书中的软件，你都要先执行这条命令。你会注意到接下来的命令中就有一个（lpthw），它表示你正在使用的虚拟环境
- 这样nose就装好了，只不过pip把它装到了．venvs/lpthw虚拟环境下面，而非主系统软件包目录。这样你就可以为不同项目安装不同的相互冲突的Python软件包版本，同时还不会污染主系统级别的配置
## ex47 自动化测试

## ex50 你的第一个网站
- 所谓的“框架”通常是指“让某件事情做起来更容易的软件包”


## 附录 命令行快速入门
- Linux/macOS
    - pwd, hostname, mkdir, cd, ls, rmdir, pushd, popd, cp, mv, less, cat, xargs, find, grep, mam, apropos, env, echo, export, exit, sudo
- Windows
    - pwd, hostname, mkdir, cd, ls, rmdir, pushd, popd, cp, robocopy, mv, more, type, forfiles, dir -r, select-string, help, helpctr, echo, set, exit, runas
- pwd, print working directory
- mkdir, make directory
    - -p 多级目录
    - 创建一个名字包含空格的目录，方法是为名称添加一个引号：mkdir "I Have Fun"
- cd, change directory
    - ~ . .. -
    - cd "I Hava Fun"
- CLI(command line interface) and GUI(graphical user interface)
- ls, list
- rmdir, rm
- pushd/popd, pushd把当前目录压栈, 进入一个新目录, 用popd返回栈顶目录
    - 感觉用处一般, cd -就够用了
- 创建新文件, touch/New-Item, 我一般用vim
- cp, -r递归