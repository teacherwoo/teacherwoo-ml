=====================
Jupyter Notebook使用 
=====================

----------
学习目标
----------

 
学会使用Jupyter Notebook编写运行代码
应用
创建文件
操作cell
运行操作

Jupyter Notebook介绍
----------------------------

Jupyter项目是一个非盈利的开源项目，源于2014年的ipython项目，因为它逐渐发展为支持跨所有编程语言的交互式数据科学和科学计算

Jupyter Notebook，原名IPython Notbook，是IPython的加强网页版，一个开源Web应用程序
名字源自Julia、Python 和 R（数据科学的三种开源语言）
是一款程序员和科学工作者的编程/文档/笔记/展示软件
.ipynb文件格式是用于计算型叙述的JSON文档格式的正式规范
jupyternotebook

为什么使用Jupyter Notebook?
----------------------------------

传统软件开发：工程／目标明确
需求分析，设计架构，开发模块，测试
数据挖掘：艺术／目标不明确
目的是具体的洞察目标，而不是机械的完成任务
通过执行代码来理解问题
迭代式地改进代码来改进解决方法
实时运行的代码、叙事性的文本和可视化被整合在一起，方便使用代码和数据来讲述故事

对比Jupyter Notebook和Pycharm

画图


数据展示



总结：Jupyter Notebook 相比 Pycharm 在画图和数据展示方面更有优势。

 Jupyter Notebook的使用-helloworld
------------------------------------------

3.1 界面启动、创建文件
界面启动
环境搭建好后，本机输入jupyter notebook命令，会自动弹出浏览器窗口打开Jupyter Notebook

# 进入虚拟环境
workon ai
# 输入命令
jupyter notebook
本地notebook的默认URL为：http://localhost:8888

想让notebook打开指定目录，只要进入此目录后执行命令即可

notebook1

新建notebook文档
notebook的文档格式是.ipynb


内容界面操作-helloworld
controlnotebook

标题栏：点击标题（如Untitled）修改文档名 菜单栏

导航-File-Download as，另存为其他格式
导航-Kernel
Interrupt，中断代码执行（程序卡死时）
Restart，重启Python内核（执行太慢时重置全部资源）
Restart & Clear Output，重启并清除所有输出
Restart & Run All，重启并重新运行所有代码
3.2 cell操作
什么是cell？

cell：一对In Out会话被视作一个代码单元，称为cell

Jupyter支持两种模式：

编辑模式（Enter）
命令模式下回车Enter或鼠标双击cell进入编辑模式
可以操作cell内文本或代码，剪切／复制／粘贴移动等操作
命令模式（Esc）
按Esc退出编辑，进入命令模式
可以操作cell单元本身进行剪切／复制／粘贴／移动等操作
3.2.1 鼠标操作
工具栏cell

3.2.2 快捷键操作
两种模式通用快捷键
Shift+Enter，执行本单元代码，并跳转到下一单元
Ctrl+Enter，执行本单元代码，留在本单元
cell行号前的 * ，表示代码正在运行

命令模式：按ESC进入
Y，cell切换到Code模式
M，cell切换到Markdown模式
A，在当前cell的上面添加cell
B，在当前cell的下面添加cell
双击D：删除当前cell
Z，回退
L，为当前cell加上行号 <!--
Ctrl+Shift+P，对话框输入命令直接运行
快速跳转到首个cell，Crtl+Home
快速跳转到最后一个cell，Crtl+End -->
编辑模式：按Enter进入
多光标操作：Ctrl键点击鼠标（Mac:CMD+点击鼠标）
回退：Ctrl+Z（Mac:CMD+Z）
重做：Ctrl+Y（Mac:CMD+Y)
补全代码：变量、方法后跟Tab键
为一行或多行代码添加/取消注释：Ctrl+/（Mac:CMD+/）
屏蔽自动输出信息：可在最后一条语句之后加一个分号
3.3 markdown演示
掌握标题和缩进即可



一级标题
二级标题
三级标题
四级标题
五级标题
缩进
二级缩进
三级缩进

【拓展】 —— Jupyter Notebook中自动补全代码等相关功能拓展
--------------------------------------------------------------------
效果展示：

image-20190312225838970

4.1 安装jupyter_contrib_nbextensions库

安装该库的命令如下：

python -m pip install jupyter_contrib_nbextensions
然后执行：

jupyter contrib nbextension install --user --skip-running-check
在原来的基础上勾选： “Table of Contents” 以及 “Hinterland”

部分功能：

image-20190313100409052

小结
--------------

为什么要使用jupyter
用于数据探索过程
是什么
是一个ipython的web加强版
怎么用
1.通过jupyter notebook 就可以使用
2.保存文件是.ipynb
3.每个内容,都对应的是一个cell
快捷键
Shift+Enter，执行本单元代码，并跳转到下一单元
Ctrl+Enter，执行本单元代码，留在本单元
jupyter模式
命令模式:(enter, 或者鼠标点击进入)
Y，cell切换到Code模式
M，cell切换到Markdown模式
A，在当前cell的上面添加cell
B，在当前cell的下面添加cell
双击D：删除当前cell
编辑模式(esc)
