---
layout:     post
title:      VIRTUALENV
subtitle:   virtualenv virtualenvwrapper 1
date:       2021-12-15
author:     LEEWARD TAN
header-img: img/post-bg-vmware1.png
catalog: false
---


#### 下一篇文章讲述了virtualenvwrapper, virtualenv是virtualenvwrapper的基础.


#### virtualenv建立一个独立的依赖库，假如你在电脑（全局环境）安装的是Python  2.7，但是你接到的项目必须使用Python 3.7, 但你并不希望升级你电脑（全局环境）上安装的Python版本从Python  2.7->Python 3.7，那么你可以通过virtualenv为你的项目指定一个虚拟环境，在该虚拟环境中选择Python 3.7, 从而与全局环境的Python  2.7保持隔离。虚拟环境就有点像docker,不同的虚拟环境相当于docker不同的容器.

#### 1.通过pip安装该包
   pip install virtualenv
#### 2. 创建虚拟环境

你首先应该创建你的项目文件夹,此处为"test"

test文件夹是空的,注意看文件目录

<small>  virtualenv enve </small>

test是项目文件夹，enve是独立的一个虚拟环境，enve这个虚拟环境表现为一个文件夹，该文件夹包含该虚拟环境的所有包，enve虚拟环境文件夹被包含于test项目文件夹中，注意看文件目录

#### 3.激活你的虚拟环境

  <small>  activate </small>


命令是内置在scripts文件夹中的，毕竟virtualenv 自身也是一个


首先要进入enve这个代表虚拟环境的文件夹中的一个子文件夹Scripts


使用activate命令后，命令行工具的最前面会出现一个括号，enve就是我们创建的虚拟环境的名字


现在查看我们独立的虚拟环境中有哪些包，三个包pip setuptools wheel


#### 4.在我们的虚拟环境中安装其他第三方库

   <small> pip install matplot </small>

在我们独立的虚拟环境中随便安装个包，matplot
再次查看，发现刚刚安装的包在我们的独立虚拟环境中了


#### 5.退出虚拟环境

<small> deactivate </small>

可以看到前面的括号没了



