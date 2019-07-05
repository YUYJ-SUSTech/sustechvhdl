#  [EE332 Digital System Design Course Lecutre ](sustechvhdl.readthedocs.io)

## 环境需求 ：

本地安装git, python3, sphinx 

*注意：如果安装sphinx的时候，在cmd输入命令无反应，试着退出电脑管家等杀毒软件。*

## 相关教程 ：

- Git 基础
- github设置
- git GUI教程      
- Sphinx-doc编写文档 
- reStructuredText(.rst)语法规则快速入门

## 编辑前准备：

在安装完sphinx后，在安装路径下的文件结构是这样的：

```javascript
│  make.bat                         # window下编译脚本
│  Makefile                         # Linux下Makefile文件
│
├─build         				  # make编译后产生的网页目录在build/html目录下
└─source                            # 文档源码目录
    │  conf.py                      # 配置文件
    │  index.rst                    # 文档源文件入口
    ├─_static                       # 编译过程产生的一些图片之类的
    └─_templates                    # 模板
```

1. 将该路径下的source文件夹删除
2. https://github.com/Joseph669/sustechvhdl将项目clone到该路径下，并将文件名改为source
3. 打开该文件，将文件夹名为“把这里的文件拿到外面”里面的conf.py文件拿到外面

完成了以上三个步骤，就可以在本地测试。即在本地修改完rst文件之后，可在本地看到修改之后的结果，该结果与合并到github后的结果基本相同，用于本地调试。该步骤为：

1. 打开cmd窗口，切换到sphinx的安装路径下
2. 执行.\make html 命令生成html文件
3. 在build/html文件夹中找到生成的文件，用浏览器打开该html文件

![](https://github.com/Joseph669/sustechvhdl/blob/master/figure/cmd.png)

**接下来就可以愉快的进行编辑了，不懂的地方可以看前面推荐的博客，可以看下我之前写的那部分内容**

## 编辑后提交：

1. 在source文件夹下，空白处鼠标右键点Git GUI Here
2. 将修改的文件添加到暂存区（step 1）
3. 简单描述修改的东西，点击commit（step 2）
4. push到远端github上

注意：在提交前最好先fetch，后再在本地merge，防止其他人在之后提交到github冲突了。（针对push失败的情况）

![](https://github.com/Joseph669/sustechvhdl/blob/master/figure/git_GUI.png)

## 管理文档：

*（以下内容普通读者可忽略，文档管理员仔细阅读）*

本文档使用[Read the Docs](https://readthedocs.org/)自动构建，了解详情请点击[这里](https://docs.readthedocs.io/en/stable/intro/getting-started-with-sphinx.html)。下图简单介绍如何该项目如何构建，详细的点击[这里](https://docs.readthedocs.io/en/stable/builds.html)

![](https://github.com/Joseph669/sustechvhdl/blob/master/figure/howtobuild.jpg)

**登录账号后可进行维护，构建**

![](https://github.com/Joseph669/sustechvhdl/blob/master/figure/build_proj.jpg)

![](https://github.com/Joseph669/sustechvhdl/blob/master/figure/maintain.jpg)

