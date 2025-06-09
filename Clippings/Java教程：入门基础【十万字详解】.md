---
title: "Java教程：入门基础【十万字详解】"
source: "https://blog.csdn.net/m0_63815035/article/details/141575029"
author:
  - "[[m0_63815035]]"
published: 2024-09-02
created: 2025-06-09
description: "文章浏览阅读2.2w次，点赞175次，收藏237次。欢迎来到小羊的《Java教程：入门基础》系列的学习之旅！无论你是初学者还是希望深化对Java编程语言理解的开发者，这系列教程都将为你提供系统化的知识和实用的技能，帮助你从零基础起步，逐步掌握Java编程的核心概念和技术。希望大家多多支持小羊吧！！让我们一起开启这段精彩的编程旅程，从零开始Go Go_java编程十万字"
tags:
  - "clippings"
---
![在这里插## 标题入图片描述](https://i-blog.csdnimg.cn/direct/cf41e32d3b3649ce9a543afd4d31abba.gif#pic_center)

![> 						大家好，我是程序员小羊！](https://i-blog.csdnimg.cn/direct/70ea780b77344481b63611d5663fb56c.png)

> ✨博客主页： [https://blog.csdn.net/m0\_63815035?type=blog](https://blog.csdn.net/m0_63815035?spm=1001.2101.3001.5343)
> 
> 💗《博客内容》：.NET、 Java.测试开发、 Python、 Android、 Go、 Node、 Android 前端小程序等相关领域知识  
> 📢博客专栏：  
> 📢欢迎 点赞 👍 收藏 ⭐留言 📝  
> 📢本文为学习笔记资料，如有侵权，请联系我删除，疏漏之处还请指正🙉  
> 📢大厦之成，非一木之材也；大海之阔，非一流之归也✨

## 前言：

> 欢迎来到小羊的《Java教程：入门基础》系列的学习之旅！无论你是初学者还是希望深化对Java编程语言理解的开发者，这系列教程都将为你提供系统化的知识和实用的技能，帮助你从零基础起步，逐步掌握Java编程的核心概念和技术。希望大家多多支持小羊吧！！让我们一起开启这段精彩的编程旅程，从零开始Go Go

## 一、Java入门&IDEA&基础语法

**本节目标：**

- 能够完成JDK和IDEA的安装
- 能够知道Java程序开发流程
- 能够完成Java环境变量的配置
- 能够使用IDEA进行Java程序的开发
- 能够根据需求完成变量的定义和使用(包括输出和修改)
- 能够知道注释，字面量，关键字，标识符的作用

### 1：Java入门

#### 1.1 Java简介

下面我们正式进入Java的学习，在这里，大家第一个关心的问题，应该就是Java是什么，我们一起来看一下：

**Java是什么：**

- Java是一门非常优秀的计算机语言
	- 语言：人与人交流沟通的表达方式
	- 计算机语言：人与计算机之间进行信息交流沟通的一种特殊语言
- Java之父：詹姆斯·高斯林（James Gosling）

![请添加图片描述](https://i-blog.csdnimg.cn/direct/2708655af1894c1db7be02326adb9074.png)

知道了Java是什么之后，大家就会想，我们学完Java可以做什么呢？下面，我们就来聊一聊，Java的三大技术平台：

**1：JavaSE**

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/585d718cc9f8419285f96b385481ba2f.png)

**2：JavaME**

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/d781f829d3d54c50afca125666fd6779.png)

**3：JavaEE**

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/fbc764e6249b4bf3a0c24ddec32cdc76.png)

知道了Java是什么，以及可以做什么之后，我们来说一下这一块的本节安排：

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/7ab4eb6921494237ac1dd4c1b352c899.png)

1、 **要开发一个Java程序，我们得安装JDK，而要安装JDK，我们得先有JDK，所以，我们会先来讲解JDK的下载和安装JDK的下载和安装讲解完毕之后，我们就可以进行Java程序的开发了，这里我会带着大家一起开发第一个Java程序，而大家在练习的过程中可能会出现一些小问题，所以，在大家练习后，我们会讲解一下开发中的常见问题** 。

2、最后呢，我们还会讲解两个小知识，一个是常用DOS命令，一个是Path环境变量，让大家对前面使用过的一些工具能够做到知其然并知其所以然。

#### 1.2 JDK的下载和安装

下面呢，我们来学习JDK的下载与安装，在讲解JDK的下载与安装之前呢，我们先对JDK做一个介绍：

**JDK：** （ **JavaDevelopment Kit**)：Java开发工具包，也就是说必须要有JDK才能开发Java程序

所以，我们得先安装了JDK，然后才能进行Java程序的开发。

了解了JDK是什么之后，我们再来对JDK的版本做一个说明：

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/7a830c3e40be471b830c538243200541.png)

这么多的版本，大家不用记，了解即可。知道三个版本就可以了，这里我们标红了：JDK8，JDK11， JDK17 。JDK8是企业用的最多的版本，JDK11和JDK17是后续长期支持更新的版本。

了解了JDK的版本之后，下面呢，我们来学习JDK的下载。

**JDK的下载：**

- 通过官方网站获取JDK（https://www.oracle.com/）
- 直接下载地址： https://www.oracle.com/java/technologies/javase-downloads.html
- **注意：针对不同操作系统，下载对应的JDK**

JDK下载图解

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/ab5dcdfc403b4b1aaa420a0b4760e331.png)

下载完成后，在本地可以看到下载好的软件：

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/da4dec53695a4145af6f980950178e55.png)

JDK下载好之后，下面我们就要来安装JDK了。

**JDK的安装：**

关于安装，这里我们说两点：

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/3a640c336d794ac2831e885a31de4608.png)

JDK安装图解：

第一步：双击启动下载好的JDK软件，在弹出框界面选择是

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/00e2f528936d421d82e1f24fbe8dc663.png)

第二步：看到如下界面，点击下一步

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/7d30150da4bf42749a74030305e7fa76.png)

第三步：看到如下界面，不要着急安装，因为它默认会安装到C:\\Program Files下面，在这里点击更改

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/6a23b5b00bce4fc7907b6480d439fc08.png)

第四步：看到如下界面，修改安装路径

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/52e28143b5c44ea08fb4e0c9aceb55cd.png)

修改路径后的界面如下，然后点击确定

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/61eb6ed734c94d59bc461bb46f86161b.png)

第五步：看到如下界面，点击下一步，等待安装

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/23dfd2e933ba4f7fa7a1add95591b159.png)

第六步：看到如下界面，说明安装成功，点击关闭即可

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/6cb3448e7909462cb832b08584e87bc5.png)

JDK安装完成后，我们到安装目录下去看看JDK的安装目录：

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/8e2dbe29607b4ad580f940221dd59c74.png)

**目录解释：**

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/ea36d9be20dd41c097facea1a3b15223.png)

到此，我们就完成了JDK的安装，大家赶快根据小羊提供的JDK软件（软件在资料里可以免费下载），完成JDK的安装吧。

#### 1.3 第一个程序

JDK安装完毕后，下面我们来开发自己的第一个Java程序。

首先，我们来说一下，Java程序的开发流程：

开发一个Java 程序，需要三个步骤：编写程序，编译程序，运行程序。如图

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/195d4496256f43a497bd70dba278707e.png)

知道了Java程序的开发流程后，下面我们来实现第一个程序：

第一步：编写程序

① 在D盘根目录下新建一个文本文档文件，修改文件名为HelloWorld.java

② 选中HelloWorld.java文件，用 Windows 系统自带的记事本打开

③ 书写如下程序内容

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/ba8660ff265b4217a41289b278bc1f04.png)

④ 保存文件：Ctrl+s

**注意：**

- 文件后缀名是.java，文件类型是java文件
- 文件名和代码中类名一致

如果后缀名还是文本文档文件，需要按照下面的步骤，勾选文件扩展名

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/bfc740d7789b4a1a85330f15f7011df0.png)

程序编写完毕后，要进行编译和运行程序。而编译和运行程序目前需要在DOS窗口下进行，因此我们先说一下如何打开DOS窗口

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/c60d267814fc4c2f8d98180aecf2b1c8.png)

说完了如何打开DOS窗口，接下来，我们来学习编译和运行程序。

第二步：编译程序

- 格式：javac 文件名.java
- 范例：javac HelloWorld.java

第三步：运行程序

- 格式：java 类名
- 范例：java HelloWorld

如图所示：

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/0571eea10eeb4a49bcaa110f463c3c85.png)

最终再控制台输出了：HelloWorld。到此第一个程序开发完毕。大家赶快动手练习吧。

#### 1.4 常见问题

刚才大家在练习的过程中，有些同学出现了一些小问题，这里呢，我们来讲解一下常见的两个小问题：

**1：单词拼写问题**

![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/daec5dbbd7c0452e9a2080080761d05e.png)

**2：中英文符号问题**

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/391c96b3034447648901b8f44658deb6.png)

而关于中英文符号问题，早期的windows系统报错信息如下：

![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/fbd295363b924e4a8565c4678b11766f.png)

这两个常见的小问题呢，大家了解一下即可，因为很快我们将会使用一款非常优秀的开发工具，这些问题将不会存在了。但是，如果出现类似的问题，我们要学会阅读并解决问题。

最后，再给大家补充一个小知识，JDK11的新特性：

**JDK11开始支持 java命令直接运行.java文件**

- 格式：java 文件名.java
- 范例：java HelloWorld.java

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/9a570e589adc4d08b6b8bdd0268b6272.png)

可能不小心这样写了，不知道为什么，这里我们就给大家统一说明一下。到此，关于第一个程序的常见问题我们就先说到这里。

#### 1.5 常用DOS命令

在后续开发中，我们有些时候需要在DOS窗口，也就是我们前面见到的黑窗口下进行一些操作，所以，我们要掌握一些常用的操心命令。

而这些命令，又需要在黑窗口下运行，所以，这里我们先讲解如何打开DOS窗口，这里我们讲解两种常见的方式：

1. 直接在地址栏输入cmd，回车即可
2. 通过运行窗口打开

第一种方式，我们已经用过了。这里我们重点说第二种方式，通过运行窗口打开：

① 按下win+R

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/b73586f985e54646b124dbdd90b0e300.png)

② 输入cmd

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/d48084f67c9146b28f9772a920d216d9.png)

③ 按下回车键

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/76579922ba4b4b5695384a9b9ea059e3.png)

这样，我们就通过运行窗口打开了DOS窗口。下面呢，我们来学习常用的DOS命令。

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/0c61f5ebe08c4f8099d1193f74068365.png)

根据老师的讲解，大家练习一下常用的DOS命令吧。

#### 1.6 Path环境变量

前面我们使用过JDK的bin目录下的javac和java命令，为什么我们能够直接使用呢？这里我们来讲解一下原理。而要讲解这个原理，我们就不得不提一下Path环境变量。

**Path环境变量的作用：**

- 它提供了windows命令行中指令的可执行文件(比如：.exe文件)路径，让我们在命令行中输入命令时，能够找到对应的可执行文件执行
- 简单说：让命令在命令行中使用有效

为了让大家更好的理解这句话，我们来做一个操作，验证一下：

- 在Path环境变量中配置QQ软件的命令行方式启动
- C:\\Program Files (x86)\\Tencent\\QQ\\Bin

如何配置呢？按照下图配置即可

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/67c6662f943b44caaeea9f3a88898930.png)

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/05620bde65b443f6afdfad7e228f350e.png)

配置完毕之后，我们到DOS窗口中，通过qq指令，就可以启动QQ软件了。

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/282c77d6405a42cd8241c26c258f1230.png)

由此可见，我们把.exe文件所在的路径配置到Path环境变量中，就可以使用.exe结尾的指令来启动程序了。这个时候，我们来说一下，为什么开始的时候我们能够直接使用javac和java指定了。

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/22538fffaebd44fbb8863d07c3d5a9fb.png)

但是，由于这种配置，只配置了较少的命令，而我们在JDK的bin目录下还有很多的命令可以使用，比如：jps,jpackage,jmap等。所以，我们要自己配置JDK的环境变量，为了后续的一些软件能够找到JDK的安装目录，我们分两步来完成Java环境变量的配置：

第一步：配置JAVA\_HOME变量

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/ccf4cc56b3194dc78f5fac4f45e8f798.png)

第二步：编辑Path变量

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/c99afe70d51e420bb46465bf5c2e0dfa.png)

到此，我们就知道了环境变量的原理，并且完成了自己配置Java的环境变量。

### 2：IDEA

前面在讲解第一个程序的常见问题的时候，我们说过了，会讲解一款非常优秀的开发工具，就是这里我们要讲解的IDEA。下面我们说一下这一块的安排：

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/e250ae519712438ca06ea72ac5056fd9.png)

首先，我们来讲解IDEA的概述和安装。

#### 2.1 IDEA概述和安装

那什么是IDEA呢？

\*\*IDEA：\*\*全称Intellij IDEA，是用于Java语言开发的集成环境，是业界公认的目前用于Java程序开发最好的工具

\*\*集成环境：\*\*把代码编写，编译，运行，调试等多种功能综合到一起的开发工具

举例说明，我们前面开发一个Java程序，需要下面这些工具的配合：

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/384686c6d76f4f9896a1fd478ff9d635.png)

而我们现在开发一个Java程序，只需要一个工具就可以了：

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/92292997fa6e4cb08ab6a49f069749b7.png)

它把代码编写，编译，运行，调试等多种功能综合到一起了，这就是集成开发环境。除了IDEA以外，还有下面几种常见的用于Java程序开发的集成环境：

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/e8ebb95181a943cb87571a8ad0d64ceb.png)

知道了IDEA是什么后，下面我们来说一下IDEA的下载和安装。

**IDEA的下载和安装：**

\*\*下载：\*\*https://www.jetbrains.com/idea

也可以直接从小羊给出的资料中获取。

![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/fa2e64cef1784f058c9fecf052cbfe3b.png)

**安装：** 建议修改安装路径

安装图解：可以根据如下步骤完成IDEA的安装

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/a2f5af805f814ef3acaed9f8f05c5b2d.png)

学完了IDEA的安装后，大家赶快动手安装一下吧。

#### 2.2 IDEA中HelloWorld

安装完IDEA后，下面我们就来使用IDEA完成HelloWorld案例。

首先，我们来启动IDEA，启动的时候还有一些基本的配置，一起来看一下：

第一步：双击桌面上的IDEA图标，选择Do not import settings，点击OK

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/26747ae54873416ead41767b7055c6e1.png)

第二步：看到如下界面

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/bc85fd401e584c9fbaad8dffc3087b00.png)

选择：Evaluate for free，点击Evaluate

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/c517511673644e758e71129d813500d4.png)

第三步：看到如下界面，点击Continue

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/816d8308e0284ceb92783a8158c83450.png)

第四步：看到如下界面，启动配置成功

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/36bcd536a4b0475fb28b6a040464180d.png)

**如果需要破解，可以夕夕上买个秘钥有教程！！**

接着，我们来完成HelloWorld案例：

这里先介绍下IDEA中的代码结构：

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/f2ef184f4e1e4e329c40607ecfbd7902.png)

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/451932ef115d4ba680dbd2318bde4321.png)

接着，我们说一下IDEA中完成HelloWorld案例的基本流程：

**① 新建一个空项目(javase\_code)  
② 新建一个新模块(idea\_test)  
③ 在idea\_test模块的src下新建一个包(com.itheima)  
④ 在com.itheima包下新建一个类(HelloWorld)  
⑤ 在HelloWorld类中编写代码(main回车，sout回车)  
⑥ 在IDEA中运行HelloWorld**

下面，我们就一起来完成IDEA中HelloWorld案例的编写，编译和运行

① 新建一个空项目(javase\_code)：

第一步：点击New Project

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/bdb37521627d4cb181d4552fafed0398.png)

第二步：选择Empty Project，点击Next

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/e9e5e3ca6204475bb1da8af58c1b22b2.png)

第三步：修改项目名称，修改项目存储路径，点击Finish，弹出一个窗体，然后点击Create

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/186a04f36b4f4afea7d5df46c7b5ce49.png)

第四步：看到如下界面，空项目创建成功

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/25ac9e7f9656481094b4393fcee849a4.png)

② 新建一个新模块(idea\_test)

第一步：选择File，点击Project Structure…

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/be9250a29b564a1ba276dd3bbbd51628.png)

第二步：在弹出的窗体中，按照1,2,3的步骤选择，来新建一个模块

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/28d4e8bb67c54f728b9d888a3ee14d18.png)

第三步：在弹出的窗体中，默认选择Java模块，JDK选择的也是17，点击Next即可

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/1a2da322c29d45b38be1d5cd668af610.png)

第四步：在弹出的窗体中，修改模块名称，点击Finish

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/d86eec8a1fc54889b91322f0aa017851.png)

第五步：然后点击OK即可

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/93b2a55b6f8a4466afa31a384bcec418.png)

这样我们建好了一个模块：

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/5f648f6799894e9d8549d731c797084b.png)

③ 在idea\_test模块的src下新建一个包(com.itheima)

第一步：展开模块，按照1,2,3的步骤选择，来新建一个包

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/47c88a9dd1194f77b3f122f2c075b5bf.png)

第二步：在弹出框里面输入包名，然后回车即可

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/46f8768491064b9183f3a3ec1d107fa4.png)

这样我们建好了一个包：

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/4ae549036e7b40fda9d29fd7f9f801f3.png)

④ 在com.itheima包下新建一个类(HelloWorld)

第一步：选中com.itheima这个包，按照1,2,3的步骤选择，来新建一个类

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/69669b46d669441da08773481afdb43a.png)

第二步：在弹出框里面输入类名，然后回车即可

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/4adfc27db8e047348bcbb8da13ee1b48.png)

这样我们建好了一个类：

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/33c294c7695c4b47a4ad86e5d781feef.png)

⑤ 在HelloWorld类中编写代码(main回车，sout回车)

在类中编写代码，可以手动编写，也可以采用快捷方式编写

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/1b74f423a02c475ab878a1e2a2dbabb3.png)

⑥ 在IDEA中运行HelloWorld

在代码中，右键选择Run ‘HelloWorld.main()’ 运行

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/0eba5043a8f04c0591fe0839bb99de08.png)

在控制台输出了结果：

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/c8d1aa18d72d4d20adc145af49858b9a.png)

这样我们就完成了IDEA中HelloWorld案例。

#### 2.3 IDEA中基本配置&注释

刚才我在讲解代码的过程中，有同学可能觉得看的不是很清楚，那下面呢，我们就来对IDEA进行两个基本的设置：

第一个：修改背景主题为白色

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/d003df6c1e9743d7b4ea2cbc381933a9.png)

第二个：修改字体大小

按照1,2,3,4进行设置即可

![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/49671d9f866a48c2addfb4b098e7c147.png)

至于其他的设置，后面我们用到的时候再去讲解。

讲解完IDEA的这两个基本设置后，下面，我们说一下注释，那什么是注释呢？

- 注释是指在程序中添加的说明性信息
- 注释不参与程序运行，仅起到说明作用

这里我们再来介绍一下注释的分类：

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/a0ca63e856944692a665dbf002955fae.png)

了解了注释的作用和分类后，下面我们来对前面讲解过的HelloWorld案例添加注释：

```java
/*
    Java程序中最基本的组成单位是类

    类的定义格式是：
        public class 类名 {

        }
 */
public class HelloWorld {
    /*
        这是main方法
        main方法是程序的入口方法，代码的执行是从main方法开始的
     */
    public static void main(String[] args) {
        //这是输出语句，能够将""里面的内容输出到控制台，并且""里面的内容是可以修改的
        System.out.println("HelloWorld");
        System.out.println("Java");
    }
}
12345678910111213141516171819
```

有了注释以后，我们再来看这段代码，明显就容易理解了。后面大家自己在编写代码的时候，也要多写写注释，在实际开发中，我们编写的程序也是要添加注释的。

这样既方便自己阅读，也方便别人阅读。

#### 2.4 IDEA中常用快捷键

为了提高我们后续写程序的效率，这里呢，我们来讲一些IDEA中常用的快捷键：

- 快速生成main方法和输出语句
```python
- main方法：main或者psvm，回车
  - 输出语句：sout，回车
12
```
- 常用快捷键
```python
- Ctrl+D：复制数据到下一行
  - Ctrl+X：剪切数据，可以用来删除所在行
  - Ctrl+Alt+L：格式化代码，建议自己写代码的时候就注意格式
  - Ctrl+/：对选中的代码添加单行注释，如果想取消注释，再来一次即可
  - Ctrl+Shift+/：对选中的代码添加多行注释，如果想取消注释，再来一次即可
12345
```

根据老师的讲解，大家练习一下常用的快捷键吧。

#### 2.5 IDEA中模块操作

IDEA的基本使用我们掌握了，最后呢，我们再来说一下，IDEA中的模块操作，而关于模块操作呢，分为三种：

- 新建模块
- 删除模块
- 导入模块

下面我们分别来操作一下。

\*\*新建模块：\*\*HelloWorld案例中讲解过了，这里就不再讲解了，想不起来了，翻到上面去看看

\*\*删除模块：\*\*删除模块又分为从工作区删除和从硬盘删除，你可以根据自己的需要，选择对应的方式进行删除

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/cbda38e86ece465e82f94924f73a4b91.png)

**导入模块：**

建议把模块复制到空项目所在路径下，然后找到新建模块的地方，只不过这一次不是新建模块，而是导入模块，所以，要选择Import Module

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/c3aa0a4e290d444892ba6d154c382e9d.png)

找到要导入的模块，点击OK

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/684f6445e6a54d6f9aefcc47b5dfaaff.png)

然后一路next，直到出现如下的界面，点击Overwrite即可

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/189925a78e0e412ab6a3feec8683f785.png)

看到下面的界面，点击Finish

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/46efaa76d33c492d94a3942a98495323.png)

最后点击OK即可

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/d2bb9532d5704be897827eb6bf74c207.png)

这样我们就成功的导入了一个模块：

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/e8929d5a993946c3a4a33da3bdeeaeb4.png)

导入模块的注意事项：

- 把模块复制到空项目所在路径下
- 出现如下错误，知道如何处理

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/a2abfb2453224a0ea0b78ed35f2a8426.png)

到此，关于IDEA的模块操作我们就讲完了。

## 二、基础语法

下面呢，我们来学习Java基础语法部分的知识，这些内容是我们后面编写程序的基本功，所以呢，大家得好好学习，下面我们说一下这一块的课程安排：

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/a4911e6872fc4671837d18a19d267790.png)

至于这5个小知识，我们该怎么用，下面呢，我们分别来讲解，首先，我们学习字面量。

#### 3.1 字面量

那什么是字面量呢？

- 直接写出来的人可以理解的数据，在java中叫做字面量
- 举例：“HelloWorld”，666，13.14

那Java中有哪些类型的字面量呢？

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/a3df9e257b6c4e6a97344e8d9f82d11d.png)

知道了Java中的字面量后，下面我们到IDEA中去演示一下字面量的使用：

```java
/*
        字符串字面量：        用双引号括起来的内容。"HelloWorld","黑马程序员"
        整数字面量：        不带小数的数字。666,-88
        小数字面量：        带小数的数字。13.14,-5.21
        字符字面量：        用单引号括起来的内容。'A','0','我'
        布尔字面量：        布尔值，表示真假。true,false
 */
public class LiteralDemo {
    public static void main(String[] args) {
        //字符串字面量
        System.out.println("HelloWorld");
        System.out.println("黑马程序员");

        //整数字面量
        System.out.println(666);
        System.out.println(-88);

        //小数字面量
        System.out.println(13.14);
        System.out.println(-5.21);

        //字符字面量
        System.out.println('A');
        System.out.println('0');
        System.out.println('我');

        //布尔字面量
        System.out.println(true);
        System.out.println(false);
    }
}
12345678910111213141516171819202122232425262728293031
```

讲解完毕之后，大家赶快动手练习一下吧。

#### 3.2 数据类型

刚才我们学习了字面量，而Java是一种强类型语言，针对每种数据都给出了明确的数据类型，那我们刚才学习的几种字面量分别应该是什么类型的呢？

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/7eb01f78f8084b78939bbede8b5d9123.png)

那为什么会有不同的数据类型呢？因为

- 不同的数据类型分配了不同的内存空间
- 不同的内存空间，所存储的数据大小是不一样的

在讲解不同的数据类型前，这里我们先普及一个小知识，就是字节的概念：

计算机中存储数据的最小单位是：字节(byte)，用B表示。

我们可以看一下硬盘存储的文件：以字节为单位

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/1055e439868a41748e5c864f20a6cef1.png)

为了帮助大家更好的理解字节这个单位，我们来说一下，常见的存储单位：

1TB = 1024GB

1GB = 1024MB

1MB = 1024KB

1KB = 1024B

这样呢，我们对字节就能有一个基础认知。有了一个基础的认知之后，我们再来说Java中的数据类型

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/627d016c7745494e9b38036dfc36b10b.png)

今天我们重点学习的是基本数据类型，关于引用数据类型，后面我们会重点学习。

在这里，我们给出每种基本数据类型的内存占用和取值范围，大家了解一下：

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/b88fa74fd0d947028195ca63cfc28eb3.png)

**说明：** E+38表示：乘以10的38次方。同理E-45表示：乘以10的负45次方

整数默认是：int类型

浮点数默认是：double类型

这样呢，我们就了解了Java中的8种基本数据类型，以及每种数据类型占用字节的情况和取值范围。关于数据类型，我们就先讲到这里。

#### 3.3 变量

学完后数据类型后，下面呢，我们来学习Java中非常重要的一个知识：变量。

那为什么要有变量呢？看这里，我们写了一段代码，在控制台显示商品的促销活动：

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/0b55fc31c5a7408a9fcc60bbd7f180d9.png)

结果，老板觉得，这个价格有点高，怕销售不好，所以决定再降100元，要求把所有的998的地方修改为888。于是你就开始改代码，改完之后如下：

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/8486389cb3674587afa6a0dc70381093.png)

结果呢？老板又觉得不划算，让你还是改回998吧，这个时候，你就要哭了。还好要修改的地方不多，要是有很多地方都要进行类似的操作，那多麻烦啊，有没有简化的方式呢？

答案当然是有的，我们找一个空间存储数据：888，并给它起个名字：price

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/d03c6ef3bdd14add96ca04444fb06634.png)

这样我们的代码就可以写成这个样子：

![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/17742f5eae0149f2bd0519c092646b3e.png)

如果要修改price里面的数据，我们只需要修改一处就可以了，代码不需要改动，但是却实现了任意修改price的效果。

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/2afcacf108ef44288d00c6de0dd5ebf3.png)

其实，这就是Java中的变量技术。有了它之后，我们就可以把变化的数据用一个变量存储，代码正常编写即可，如果需要修改数据，我们修改变量的值就可以了。那什么是变量呢？

- 变量就是内存中的存储空间
- 空间中存储的数据是可以发生改变

知道了，什么是变量后，下面我们来说一下变量的定义格式：

- 格式：数据类型 变量名 = 变量值;
- 范例：int price = 998;
	根据变量名进行使用，可以输出，也可以修改值

了解了变量的定义格式和使用方式后，下面我们到IDEA中去演示一下：

```java
/*
    格式：数据类型 变量名 = 变量值;
 */
public class VariableDemo01 {
    public static void main(String[] args) {
        //定义一个int类型的变量，用来表示价格
        int price = 998;

        //输出变量
        System.out.println(price);

        //修改变量的值
        price = 888;

        //再次输出变量的值
        System.out.println(price);
    }
}
123456789101112131415161718
```

学完了变量的定义，输出使用和修改值使用后，大家赶快动手练习一下吧。

#### 3.4 变量的案例

了解了变量的定义和基本使用后，下面我们来做两个案例，熟悉一下变量的使用：

##### 3.4.1 手机信息描述

需求：分析下图指定数据，看看哪些可以通过变量表示，并思考采用那种数据类型，最后通过程序实现

指定数据：京东价，重量，颜色

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/a6cc8b842984479da7bb94e86437cccf.png)

分析：

① 京东价，重量，选择颜色这些字都是固定的，但是他们后面的数据是变化的，所以要用变量表示

② 价格，可以用double或者int类型来表示，这里我们用int类型表示；

重量，用double类型表示；颜色，用String类型表示

分析完毕之后，下面我们到IDEA中去实现一下：

```java
/*
    手机信息描述
 */
public class VariableTest01 {
    public static void main(String[] args) {
        //定义秒杀价变量
        double price = 3599.00;

        //定义颜色变量
        String color = "蓝色";

        //定义版本变量，纪录的是内存大小
        int size = 8;

//        System.out.println(price);
//        System.out.println(color);
//        System.out.println(size);

        //为了输出效果好看一些，我加上一些内容
        System.out.println("秒杀价是："+price);
        System.out.println("你选择的颜色是："+color);
        System.out.println("你选择的版本是："+size);

        //字符串字面值+任意的数据=字符串数据
    }
}
1234567891011121314151617181920212223242526
```

##### 3.4.2 疫情防控信息采集表

需求：分析右图信息，并通过程序实现

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/9b590ca893824e4b8594e7bb1108edc9.png)

通过上图数据，我们可以根据变化的数据，提取出下图：

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/22784f31ed924e4b8f6acf8f6a663621.png)

分析：

① String name = “风清扬”;

② int age = 36;

③ char gender = ‘男’; 也可以采用String类型表示

④ double temperature = 36.2;

⑤ boolean flag = true; 也可以采用char或者String表示

分析完毕之后，下面我们到IDEA中去实现一下：

```java
/*
    疫情防控信息采集表
 */
public class VariableTest02 {
    public static void main(String[] args) {
        //定义变量
        String name = "风清扬";
        int age = 18;
        char gender = '男';
        double temperature = 36.2;
        boolean flag = true;

        //输出数据
        System.out.println("姓名是：" + name);
        System.out.println("年龄是：" + age);
        System.out.println("性别是：" + gender);
        System.out.println("体温是：" + temperature);
        System.out.println("是否接种过疫苗：" + flag);
    }
}
1234567891011121314151617181920
```

#### 3.5 变量的注意事项

关于变量的使用呢，我们讲解几个小的注意事项，大家了解一下，这样呢，遇到变量的问题后，大家就可以知道如何解决了。

变量的注意事项：

- 变量名不能重复
- 变量未赋值，不能使用
- 定义long类型变量，数据后面加L
- 定义float类型变量，数据后面加F

IDEA中代码演示如下：

```java
/*
    变量使用的注意事项
 */
public class VariableDemo02 {
    public static void main(String[] args) {
        int age = 10;
//        int age = 20;

//        int money;
        money = 20;
//        System.out.println(money);

        long money = 1000000000000L;
        float price = 12.34F;
    }
}
12345678910111213141516
```

#### 3.6 关键字

下面我们来学习一个小的知识点：关键字。

首先，我们得知道什么是关键字：

\*\*关键字：\*\*就是被Java语言赋予了特定含义的单词

我们先来看一下，曾经写过的代码中，出现的关键字：

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/3581cf6e4be04d2bb21dcffc7443d4a9.png)

了解了什么是关键字后，我们来说一下 **关键字的特点** ：

- 关键字的字母全部小写
- 常用的代码编辑器，针对关键字有特殊的颜色标记，非常直观

知道了关键字的特点后，这里我们给大家看看Java中的关键字：

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/fc4baaf004774e5e9e8f116b09690230.png)

虽然比较多，但是大家不用担心。因为：关键字，我们不需要专门记忆。这些关键字我们在开发中比较常用的，写的多了，你自然就记住了。好了，Java中的关键字我们就先讲到这里。

#### 3.7 标识符

下面呢，我们来讲解基础语法部分最后一个知识：标识符。

首先，我们来说一下什么是标识符：

\*\*标识符：\*\*就是给类，方法，变量等起名字的符号

比如，我们前面写类的时候，起的名字：HelloWorld，变量的时候，价格，price等，这就是标识符。

那这个符号你能随便写呢，当然是不能的，这里我们来看一下 **标识符的组成规则** ：由数字、字母、下划线(\_)和美元符($)组成

了解了组成规则后，这里我们还得说一下 **注意事项：**

- 不能以数字开头
- 不能是关键字
- 区分大小写

判断下面哪些标识符不符合规则

bj b2 2b \_2b class helloworld

按照我们讲解的规则，大家应该能够判断出来：2b和class是不符合规则的。

知道了标识符的组成规则和注意事项后，这里我们再说一下起名字常用的 **命名约定：**

- 小驼峰命名法
	- 约定1：标识符一个单词的时候，首字母小写
	- 范例1：name
	- 约定2：标识符是多个单词的时候，第一个单词首字母小写，其他单词首字母大写
	- 范例2：firstName
- 大驼峰命名法
	- 约定1：标识符一个单词的时候，首字母大写
	- 范例1：Hello
	- 约定2：标识符是多个单词的时候，每个单词首字母大写
	- 范例2：HelloWorld

一般来说，小驼峰命名法适用于对方法，变量等起名字。大驼峰命名法适用于对类，接口等起名字。

最后再强调一点，就是我们起名字，最好能够做到： **见名知意**

比如，我们前面讲解过的变量的案例中，我们起的名字就做到了见名知意。

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/e5af01a6ab4142c4bbf39657a63d1c88.png)

好了，到此关于标识符我们就先讲到这里。# Java入门&IDEA&基础语法

## 三、运算符&选择语句

**本节目标：**

- 能够知道每种运算符的作用及使用特点
- 能够理解+操作的三种情况
- 能够知道顺序结构语句的执行流程
- 能够使用Debug查看程序的执行流程
- 能够根据需求选择合适的if语句实现
- 能够知道switch语句执行流程和注意事项

### 4：运算符

前面我们学过了通过字面量和变量来表示一个数据，这里呢，我们来学习对数据进行运算。而对数据运算就要用到我们这里要讲解的运算符，而在讲解具体的运算符之前，我们对运算符和表达式做一个简单的描述：

\*\*运算符：\*\*对字面量或者变量进行操作的 **符号**

\*\*表达式：\*\*用 **运算符** 把字面量或者变量连接起来 **符合java语法的式子** 就可以称为表达式。不同运算符连接的表达式体现的是不同类型的表达式。

举例说明：\*\*

int a = 10;

int b = 20;

int c = a + b;

**+** ：是 **运算符** ，是算术运算符

**a + b** ：是 **表达式** ，由于+是算术运算符，所以这个表达式叫算术表达式

知道了什么是运算符和表达式以后，我们来说一下这一块的安排：

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/8590dd76552747d0860746a58c359789.png)

总共要学习5种类型的运算符，后三种标记为灰色了，我们是在哪里用就在哪里学习。这里我们先学习前两种，首先我们来学习算术运算符

#### 4.1 算术运算符

Java中的算术运算符有如下几种：

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/4544cbf10de34163bace45f8f854171f.png)

了解了Java中的算术运算符之后，下面我们到IDEA中去使用一下：

```java
/*
    算术运算符
 */
public class OperatorDemo {
    public static void main(String[] args) {
        //定义两个int类型的变量
        int a = 6;
        int b = 4;

        System.out.println(a + b);//10
        System.out.println(a - b);//2
        System.out.println(a * b);//24
        System.out.println(a / b);//1.5? 1
        System.out.println(a % b);//2

        //整数相除只能得到整数，要想得到小数，必须有浮点数的参与
        System.out.println(6.0 / 4);
    }
}

1234567891011121314151617181920
```

最后，我们来总结一下，刚才在演示代码的时候有两个注意事项：

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/e2ddec984cba4c9d8d65c97757b2e85c.png)

#### 4.2 案例数值拆分

需求：定义一个三位数，将其拆分为个位、十位、百位后，输出在控制台

什么意思呢？下面我们举例来说明一下：

举例：int number = 123；

在控制台输出结果：

个位是：3

十位是：2

百位是：1

知道了要做什么后，下面我们来分析一下如何获取个位，十位，百位：

分析：

① 个位的计算：数值 % 10

123 除以 10（商12，余数为3）

② 十位的计算：数值 / 10 % 10

123 除以 10 （商12，余数为3，整数相除只能得到整数）

12 除以 10 （商1，余数为2）

③ 百位的计算：数值 / 10 / 10 % 10

123 / 10 / 10 % 10（123 / 10 得到12，12 / 10 得到1，1 % 10 得到 1）

分析完毕之后，下面我们到IDEA中去实现一下：

```java
/*
    需求：定义一个三位数，将其拆分为个位、十位、百位后，输出在控制台
 */
public class OperatorTest {
    public static void main(String[] args) {
        //定义一个三位数
        int number = 123;

        //获取个，十，百位数据
        int ge = number % 10;
        int shi = number / 10 % 10;
        int bai = number / 100 % 10;

        //输出结果
        System.out.println("个位是：" + ge);
        System.out.println("十位是：" + shi);
        System.out.println("百位是：" + bai);
    }
}
12345678910111213141516171819
```

#### 4.3 +操作的三种情况

##### 4.3.1 数字相加(类型转换)

在Java程序中，数据参与运算，要求类型一致。这里就涉及到了数据的类型转换。而类型转换又分为两种：

1. 隐式转换
2. 强制转换

\*\*隐式转换：\*\*把一个表示数据范围小的数值或者变量赋值给另一个表示数据范围大的变量

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/ff7b2372af5449788a288edfabd93d90.png)

\*\*强制转换：\*\*把一个表示数据范围大的数值或者变量赋值给另一个表示数据范围小的变量

格式：数据类型 变量名 = (目标数据类型)(数值或者变量)

IDEA中代码演示如下：

```java
/*
    数字相加
 */
public class OperatorDemo01 {
    public static void main(String[] args) {
        int a = 10;
        double b = 13.14;
        System.out.println(a + b);

        int c = (int)(a + b);
        System.out.println(c);
//        double d = a + b;

        short s = 10;
        int i = 20;
        int j = s + i;
//        short ss = s + i;

        short ss = (short) (s + i);
    }
}
123456789101112131415161718192021
```

##### 4.3.2 字符相加

这里我们再来说一下字符参与+操作。

先到IDEA中去讲解，然后再回来总结。

IDEA中代码演示如下：

```java
/*
    字符相加
 */
public class OperatorDemo02 {
    public static void main(String[] args) {
        //定义两个变量
        int i = 10;
        char ch = 'A';//'A'的值是65
        ch = 'a';//'a'的值是97
        ch = '0';//'0'的值是48
        System.out.println(i + ch);
    }
}
12345678910111213
```

代码演示完毕后，回到资料总结：

字符参与+操作，其实就是拿字符在计算机底层对应的数值来进行计算的，这里我们了解一下英文大小写字符和数字字符对应的数据值：

- ‘A’ 65 A-Z是连续的
- ‘a’ 97 a-z是连续的
- ‘0’ 48 0-9是连续的

这里也给大家准备了一张ASCII码表，里面有常用的字符及其对应的数值关系：

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/c3d7daeee83c44ea99e6e77655f655df.png)

##### 4.3.3 字符串相加

接下来，我们继续讲解字符串相加，先到IDEA中去讲解，然后再回来总结。

IDEA中代码演示如下：

```java
/*
    字符串相加
 */
public class OperatorDemo03 {
    public static void main(String[] args) {
        System.out.println("it" + "heima");
        System.out.println("itheima" + 666);
        System.out.println(666 + "itheima");

        System.out.println("itheima" + 6 + 66);
        System.out.println(1 + 99 + "年itheima");
    }
}

1234567891011121314
```

代码演示完毕后，回到资料总结：

- 当“+”操作中出现字符串时，这个“+”是字符串连接符，而不是算术运算
	- “zhongguo”+ 666
- 当连续进行“+”操作时，从左到右逐个执行
	- 1 + 9999 + “岁zhongguo”

#### 4.4 赋值运算符

下面呢，我们来学习赋值运算符。

Java中的赋值运算符有如下几种：

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/blog_migrate/e6cacf3546514978dce7f8ccda603406.png)

了解了Java中的赋值运算符之后，下面我们到IDEA中去使用一下：

```java
/*
    赋值运算符
 */
public class OperatorDemo {
    public static void main(String[] args) {
        int a = 10;
        System.out.println("a:" + a);

        // += : 把左边和右边的数据相加，最后把结果赋值给左边
//        a += 20;
        a = a + 20;
        System.out.println("a:" + a);

        //注意：扩展的赋值运算符底层隐含了强制类型转换
        short s = 1;
//        s += 2;
        s = (short) (s + 2);
        System.out.println("s:" + s);
    }
}
123456789101112131415161718192021
```

最后，我们来总结一下，刚才在演示代码的时候有个注意事项：

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/4eb007e095974b6db6751fe05e559a66.png)

### 5：选择语句

为了控制程序的执行流程，Java 就提供了一些流程控制语句，我们先来举例说明一下：

**顺序结构** ：从上往下，依次执行

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/4852352b047b4cd098ae559b03d9b99e.png)

**选择结构：**

QQ界面的登录，填写账号和密码正确，展示好友列表界面。填写账号或者密码有误，提示：你输入的账号或密码不正确。

这就是通过选择结构来实现的，实际开发中，类似这种逻辑判断的情况非常常见。

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/c986714009964f39b442b24eed8546fc.png)

**循环结构：**

比如说，京东商城中，查询手机数据，京东就会返回给你一堆符合你查询要求的数据。

假如，每一部手机数据的展示需要5行代码，如果最终返回了1000部手机，你就需要编写5000行代码来实现数据展示。

这样就太麻烦了，那么，有没有一种流程语句，能够简化这种操作呢？答案肯定是有的，就是我们的循环结构，它就可以通过一个比较简单的结构来控制我们的手机展示1000次。

比如说，带着这样写就可以了，这就是循环结构。

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/b42d93240a474bfb97accd817f70fe23.png)

了解完毕之后，我们来说一下这一节的安排：

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/38f69b279abc44e884ec85dca2b4a50e.png)

首先，我们来学习顺序结构

#### 5.1 顺序结构

\*\*顺序结构：\*\*是程序中最简单最基本的流程控制，没有特定的语法结构，按照代码的先后顺序，依次执行

**执行流程图：**

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/4b5fe160a65b4b1ea1cb703896e35feb.png)

了解完顺序结构后，下面我们到IDEA中去演示一下：

```java
/*
    顺序结构语句
 */
public class OrderDemo {
    public static void main(String[] args) {
        System.out.println("开始");
        System.out.println("语句A");
        System.out.println("语句B");
        System.out.println("语句C");
        System.out.println("结束");
    }
}
123456789101112
```

这个比较简单，也没什么好练习的。就不练了，我们继续往下学习。

#### 5.2 Debug的基本使用

为了帮助大家更好的理解程序的执行流程，我们来学习Debug，那什么是Debug呢？

\*\*Debug：\*\*是供程序员使用的程序调试工具，它可以用于查看程序的执行流程，也可以用于追踪程序执行过程来调试程序

它的两大作用，查看程序执行流程，调试程序。由于目前我们每个程序的代码内容还比较少，

所以，今天重点掌握查看程序执行流程，当代码复杂的时候，我们需要通过debug来调试程序。那么，debug操作的流程是什么样子的呢？

在讲解操作流程前，我们来说一下：

Debug，又被称为 **断点调试** ，断点其实是一个标记，告诉我们从哪里开始查看

知道了Debug被称为断点调试后，我们来讲一下Debug的操作流程：

① 如何加断点

选择要设置断点的代码行，在行号的区域后面单击鼠标左键即可。如图

![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/523d7e9f2d33449ea7621b7eea1c7c08.png)

② 如何运行加了断点的程序

在代码区域右键Debug执行

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/d937e37cfe5747d3858c627e741abeab.png)

③ 看哪里

看Debugger窗口，看 Console 窗口

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/acfcdbb7f953490ea0cfe77d9cf1a1ee.png)

④ 点哪里

点(Step Over F8) 开始，点(Stop)结束

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/6f86d5411923462bab88c306e5c63770.png)

⑤ 如何删除断点

选择要删除的断点，单击鼠标左键即可。也就是把第一步的动作，再做一次即可。

总结一下，Debug的使用流程：

```python
①如何加断点：选择要设置断点的代码行，在行号的区域后面单击鼠标左键即可

②如何运行加了断点的程序：在代码区域右键Debug执行

③看哪里：看Debugger窗口，看Console窗口

④点哪里：点(Step Over F8) 开始，点(Stop)结束

⑤如何删除断点：选择要删除的断点，单击鼠标左键即可
123456789
```

通过Debug的方式看一下，如下代码的执行流程：

```java
/*
    Debug查看程序执行流程
 */
public class DebugDemo {
    public static void main(String[] args) {
        //定义一个int类型的变量，用来表示价格
        int price = 998;

        //输出变量
        System.out.println(price);

        //修改变量的值
        price = 888;

        //再次输出变量的值
        System.out.println(price);
    }
}
123456789101112131415161718
```

#### 5.3 选择语句之if

选择语句有两种结构：

1. if语句
2. switch语句

这里我们先来学习if语句，它会根据判定的结果（真或假）决定执行某个分支的代码

举例说明一下：

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/1d46409b6d5e49d1a1ad1e7a6ceaa14d.png)

无人驾驶的核心就是需要编写大量的判断逻辑，让车辆的行驶变得更加安全。

了解了交通信号灯的基本逻辑后，下面呢，我们通过if语句来实现过马路的信号灯判断，而if语句呢，有三种格式，这里我们首先来学习第一种格式

##### 5.3.1 if语句格式1

**格式：**

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/475b5f28d8d84350bc880bb3c239ada8.png)

**范例：**

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/89d74d7ccc8d46dd9769b721ee667c51.png)

**执行流程：**

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/975b22a09ba7463c8a0deae7e1a226d6.png)

了解完if语句格式1之后，下面我们到IDEA中去使用一下：

```java
/*
    if语句格式1
 */
public class IfDemo01 {
    public static void main(String[] args) {
        //定义一个变量，用来表示绿灯的状态
        boolean isGreen = true;
        isGreen = false;

        if(isGreen) {
            System.out.println("绿灯行");
        }
    }
}
1234567891011121314
```

##### 5.3.2 if语句格式2和格式3

刚才我们通过if语句格式1进行了判断，是绿灯的时候，可以通行，但是不是绿灯的时候，没有告诉我不可以通行啊。所以，这里就产生了if语句的第二种格式，先在代码中演示，再回去总结：

```java
/*
    if语句格式2
 */
public class IfDemo02 {
    public static void main(String[] args) {
        //定义一个变量，用来表示绿灯的状态
        boolean isGreen = true;
        isGreen = false;

        if (isGreen) {
            System.out.println("绿灯行");
        } else {
            System.out.println("不是绿灯，不允许行使");
        }
    }
}
12345678910111213141516
```

演示完毕后，我们来说一下，if语句格式2：

**格式：**

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/9d0a004972e147058a0c5ac64c648c45.png)

**范例：**

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/64b8258f12e543a3b6080524d10dc9d4.png)

**执行流程：**

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/2f4b095f2a044fbaa0169411aaa88381.png)

讲解完if语句格式2之后，我们到IDEA中再去看一段代码：

```java
public class IfDemo03 {
    public static void main(String[] args) {
        //定义三个变量，表示交通信号灯的三种状态
        boolean isRed = true;
        boolean isGreen = true;
        boolean isYellow = true;
        
        if (isRed) {
            System.out.println("红灯停");
        }

        if (isGreen) {
            System.out.println("绿灯行");
        }

        if (isYellow) {
            System.out.println("黄灯亮了等一等");
        }
    }
}
1234567891011121314151617181920
```

很明显，这是不合理的，因为我们把三种状态都设置为true了，而实际生活中，只会有一种状态为true，怎么解决呢多种情况的判断呢？这个时候就产生了if语句的第三种格式，先在代码中演示，再回去总结：

```java
/*
    if语句格式3
 */
public class IfDemo03 {
    public static void main(String[] args) {
        //定义三个变量，表示交通信号灯的三种状态
        boolean isRed = true;
        boolean isGreen = true;
        boolean isYellow = true;

        //红灯
//        isGreen = false;
//        isYellow = false;

        //绿灯
//        isRed = false;
//        isYellow = false;

        //黄灯
//        isRed = false;
//        isGreen = false;

        //出现了故障，信号灯都不亮了
        isRed = false;
        isGreen = false;
        isYellow = false;

        if(isRed) {
            System.out.println("红灯停");
        }else if(isGreen) {
            System.out.println("绿灯行");
        }else if(isYellow) {
            System.out.println("黄灯亮了等一等");
        } else  {
            System.out.println("交通信号灯故障，请在保证安全的情况下通行");
        }
    }
}
123456789101112131415161718192021222324252627282930313233343536373839
```

演示完毕后，我们来说一下，if语句格式3：

if语句格式3：

**格式：**

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/d18972c8a510496a8942b337f536f671.png)

**执行流程：**

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/dcd669e20a4746408c9be10b572ca787.png)

##### 5.3.3 案例1(交通信号灯)

需求：交通信号灯由红灯、绿灯、黄灯组成，请通过程序实现不同的信号灯给出不同的提示。

提示信息：红灯停、绿灯行、黄灯亮了等一等

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/025a46f71378475caa7696bcf671091e.png)

首先，我们来简单的分析一下：

**分析：**

① 用哪种类型来表示信号灯的三种状态呢？

用int类型来表示信号灯的三种状态(1表示红灯，2表示绿灯，3表示黄灯)

② 用if语句的哪种格式来实现该需求呢？

一般来说：1种情况的判断用if格式1,2种情况的判断用if格式2，多种情况的判断用if格式3

③ if语句判断的表达式该怎么写呢？

int light = 1;

if(light == 1) {…}

\==：是关系运算符，用来判断两个数据是否相等，如果相等，结果为true，否则为false

分析完毕后，我们来说一下实现步骤：

**实现步骤：**

① 定义一个int类型的变量用来表示信号灯的状态(1表示红灯，2表示绿灯，3表示黄灯)

② 用if语句格式3进行多种情况的判断

③ 根据不同的情况给出不同的提示信息

知道了实现步骤，下面我们到IDEA中去实现一下：

```java
/*
    需求：交通信号灯由红灯、绿灯、黄灯组成，请通过程序实现不同的信号灯给出不同的提示。
    提示信息：红灯停、绿灯行、黄灯亮了等一等
 */
public class IfTest01 {
    public static void main(String[] args) {
        //1:定义一个int类型的变量用来表示信号灯的状态(1表示红灯，2表示绿灯，3表示黄灯)
        int light = 1;
        light = 2;
        light = 3;
        light = 4;

        //2:用if语句格式3进行多种情况的判断
        //3:根据不同的情况给出不同的提示信息
        if (light == 1) {
            System.out.println("红灯停");
        } else if (light == 2) {
            System.out.println("绿灯行");
        } else if (light == 3) {
            System.out.println("黄灯亮了等一等");
        } else {
            System.out.println("交通信号灯故障，请在保证安全的情况下通行");
        }
    }
}
12345678910111213141516171819202122232425
```

##### 5.3.4 关系运算符

Java中的关系运算符有如下几种：

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/1f74541e999a4f4a8bb4af6778e12c14.png)

了解了Java中的关系运算符之后，下面我们到IDEA中去使用一下：

```java
/*
    关系运算符
 */
public class OperatorDemo01 {
    public static void main(String[] args) {
        //定义三个int类型的变量
        int i = 10;
        int j = 20;
        int k = 10;

        //等于：==
        System.out.println(i == j);//false
        System.out.println(i == k);//true
        System.out.println("--------");

        //不等于：!=
        System.out.println(i != j);//true
        System.out.println(i != k);//false
        System.out.println("--------");

        //大于：>
        System.out.println(i > j);//false
        System.out.println(i > k);//false
        System.out.println("--------");

        //大于等于：>=
        System.out.println(i >= j);//false
        System.out.println(i >= k);//true
        System.out.println("--------");

        //千万不要把==写成了=
        System.out.println(i = j); //20
    }
}
12345678910111213141516171819202122232425262728293031323334
```

最后，我们来总结一下，刚才在演示代码的时候有两个注意事项：

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/fb3d7863e62643fe91f787bd6fc72ba7.png)

##### 5.3.5 案例2(奇偶数)

需求：给定一个整数，请用程序实现判断该整数是奇数还是偶数，并在控制台输出该整数是奇数还是偶数

提示：偶数是能够被2整除的整数

首先，我们来简单的分析一下：

**分析：**

① 如何判断一个整数是奇数还是偶数？

整数对2进行取余，余数为0是偶数，否则为奇数

② 用if语句的哪种格式来实现该需求呢？

该整数要么是偶数，要么是奇数，2种情况，所以用if语句格式2

分析完毕后，我们来说一下实现步骤：

**实现步骤：**

① 定义一个int类型的整数

② 用if语句格式2进行判断

③ 根据是否是偶数给出不同的提示信息

知道了实现步骤，下面我们到IDEA中去实现一下：

```java
/*
    需求：给定一个整数，请用程序实现判断该整数是奇数还是偶数，并在控制台输出该整数是奇数还是偶数
 */
public class IfTest02 {
    public static void main(String[] args) {
        //1:定义一个int类型的整数
        int number = 10;
        number = 9;

        //2:用if语句格式2进行判断
        //3:根据是否是偶数给出不同的提示信息
        if (number % 2 == 0) {
            System.out.println(number + "是偶数");
        } else {
            System.out.println(number + "是奇数");
        }
        
    }
}
12345678910111213141516171819
```

##### 5.3.6 案例3(手机以旧换新)

需求：张三想买一台7988元的新手机，他的旧手机在二手市场能卖1500元，而手机专卖店推出以旧换新优惠，把他旧手机交给店家，新手机就能够打8折优惠。

为了更省钱，要不要以旧换新？请通过程序告诉张三

首先，我们来简单的分析一下：

**分析：**

① 计算不使用以旧换新的花费

7988 - 1500

② 计算使用以旧换新的花费

7988 \* 0.8

③ 用if语句的哪种格式来实现该需求呢？

if语句格式2

分析完毕后，我们来说一下实现步骤：

**实现步骤：**

① 定义变量(money1)纪录不使用以旧换新的花费

② 定义变量(money2)纪录使用以旧换新的花费

③ 用if语句格式2进行判断 money1是否大于money2

④ 根据判断结果，给出相应的提示

知道了实现步骤，下面我们到IDEA中去实现一下：

```java
/*
    需求：张三想买一台7988元的新手机，他的旧手机在二手市场能卖1500元，而手机专卖店推出以旧换新优惠，
        把他的旧手机交给店家，新手机就能够打8折优惠。为了更省钱，要不要以旧换新？请通过程序告诉张三
 */
public class IfTest03 {
    public static void main(String[] args) {
        //1:定义变量(money1)纪录不使用以旧换新的花费
        int money1 = 7988 - 1500;

        //2:定义变量(money2)纪录使用以旧换新的花费
        double money2 = 7988 * 0.8;

        //3:用if语句格式2进行判断 money1是否大于money2
        //4:根据判断结果，给出相应的提示
        if (money1 > money2) {
            System.out.println("使用以旧换新更省钱");
        } else {
            System.out.println("不使用以旧换新更省钱");
        }
        
    }
}
12345678910111213141516171819202122
```

##### 5.3.7 案例4(你是青年人吗)

需求：给出你的年龄，通过程序判断你是否属于青年人？

提示：世界卫生组织，经过对全球人体素质和平均寿命进行测定，对年龄划分标准作出了新的规定

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/bb32cf9a90484c3e82c9f0cac236a6f2.png)

首先，我们来简单的分析一下：

**分析：**

① 如何判断一个年龄是否属于青年人？

年龄要大于等于18，并且小于等于65

② 在Java中如何表示并且的关系呢？

age >=18 && age<=65

**&& ：是逻辑运算符，用来连接两个结果为boolean类型的表达式，都为true，结果为true，否则为false**

分析完毕后，我们来说一下实现步骤：

**实现步骤：**

① 定义一个int类型的变量来表示你的年龄

② 用if语句格式2进行判断看你是否属于青年人

③ 根据是否是青年人给出不同的提示信息

知道了实现步骤，下面我们到IDEA中去实现一下：

```java
/*
    需求：给出你的年龄，通过程序判断你是否属于青年人？
    提示：青年人的年龄范围 18~65
 */
public class IfTest04 {
    public static void main(String[] args) {
        //1:定义一个int类型的变量来表示你的年龄
        int age = 22;
        age = 100;

        //2:用if语句格式2进行判断看你是否属于青年人
        //3:根据是否是青年人给出不同的提示信息
        if(age>=18 && age<=65) {
            System.out.println("你是青年人");
        } else {
            System.out.println("你不是青年人");
        }
        
    }
}
1234567891011121314151617181920
```

##### 5.3.8 逻辑运算符

Java中常用的逻辑运算符有如下几种：

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/303dc035c2e4465b8a9c11840020fc29.png)

了解了Java中的逻辑运算符之后，下面我们到IDEA中去使用一下：

```java
/*
    逻辑运算符
 */
public class OperatorDemo02 {
    public static void main(String[] args) {
        //定义变量
        int i = 10;
        int j = 20;
        int k = 30;

        //逻辑与：&&
        System.out.println((i>j) && (i>k));//false && false
        System.out.println((i<j) && (i>k));//true && false
        System.out.println((i>j) && (i<k));//false && true
        System.out.println((i<j) && (i<k));//true && true
        System.out.println("-----------------------");

        //逻辑或：||
        System.out.println((i>j) || (i>k));//false || false
        System.out.println((i<j) || (i>k));//true || false
        System.out.println((i>j) || (i<k));//false || true
        System.out.println((i<j) || (i<k));//true || true
        System.out.println("-----------------------");

        //逻辑非：!
        System.out.println(!(i>j));//!false
        System.out.println(!!(i>j));//!!false
        System.out.println(!!!(i>j));//!!!false
        System.out.println(!!!!(i>j));//!!!!false
        
    }
}
1234567891011121314151617181920212223242526272829303132
```

##### 5.3.9 三元运算符

下面我们来学习三元运算符：

**格式** ：关系表达式 ？表达式1 ：表达式2；

**范例** ：a > b? a: b;

**执行流程：**

- 首先计算关系表达式的值
- 如果值为true，表达式1的值就是运算结果
	如果值为false，表达式2的值就是运算结果

了解了三元运算符的执行流程后，下面我们到IDEA中去使用一下：

```java
/*
    三元运算符
 */
public class OperatorDemo03 {
    public static void main(String[] args) {
        int a = 10;
        int b = 20;

        int max = a > b ? a : b;

        System.out.println("较大的值是：" + max);
    }
}
12345678910111213
```

##### 5.3.10 三元运算符和if语句格式2的区别

这里呢，我们来讲解一下三元运算符和if语句格式2的区别，它们有什么区别呢？我们先到IDEA中进行讲解，然后再回来总结：

```java
/*
    三元运算符和if语句格式2的区别
 */
public class OperatorTest {
    public static void main(String[] args) {
        //定义两个int类型的变量
        int a = 10;
        int b = 20;

        //需求：获取两个数中的较大值
        //if语句实现
//        int max;
//        if (a > b) {
//            max = a;
//        } else {
//            max = b;
//        }
//        System.out.println("较大的值是：" + max);

        if(a > b) {
            System.out.println("较大的值是：" + a);
        }else {
            System.out.println("较大的值是：" + b);
        }

        //三元运算符实现
        int max = a > b? a: b;
        System.out.println("较大的值是：" + max);
    }
}
123456789101112131415161718192021222324252627282930
```

讲解完毕之后，回来总结一下：

- 如果if语句控制的内容：是用变量纪录数据值，可以通过三元运算符改进

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/faa2d333b5b842ff9e1093b79a719715.png)

- 如果if语句控制的内容是：是通过输出语句直接输出数据值，无法通过三元运算符改进

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/b390519fdd54418298cd200607e09b16.png)

好了，关于三元运算符和if语句格式2的区别我们就讲到这里。这个知识大家先了解一下，方便我们后面在适合的场景选择合适的实现方案。

#### 5.4 选择语句之switch

下面我们来学习选择语句中的switch语句。

**格式：**

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/51d8533f1f9545ce9fb8de54ea59f81f.png)

**格式说明：**

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/ac7d4fedbdb5408caa208f71da42ac16.png)

**执行流程：**

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/4c0d9d6be3614c3c926459ac04b1aa56.png)

了解完switch语句后，下面我们到IDEA中去使用一下：

```java
/*
    switch语句
 */
public class SwitchDemo {
    public static void main(String[] args) {
        //定义一个int类型的变量用来表示信号灯的状态(1表示红灯，2表示绿灯，3表示黄灯)
        int light = 1;
//        light = 2;
//        light = 3;
//        light = 4;

        //用switch语句实现交通信号灯案例
        switch (light) {
            case 1:
                System.out.println("红灯停");
                break;
            case 2:
                System.out.println("绿灯行");
                break;
            case 3:
                System.out.println("黄灯亮了等一等");
                break;
            default:
                System.out.println("交通信号灯故障，请在保证安全的情况下通行");
                break;
        }

    }
}
1234567891011121314151617181920212223242526272829
```

最后，我们来总结一下，刚才在演示代码的时候有个注意事项：

**注意** ：在switch语句中，如果case控制的语句体后面不写break，将出现穿透现象，在不判断下一个case值的情况下，向下运行，直到遇到break，或者整个switch语句结束

## 四、循环语句

**本节目标：**

- 能够理解循环语句的四个组成部分
- 能够知道三种循环的各自格式和执行流程
- 能够知道三种循环的区别
- 能够使用循环语句完成今日案例
- 能够知道跳转语句的使用场景

### 6：for循环结构

下面我们来学习循环结构语句，循环结构有三种语句，分别是：

1. for循环
2. while循环
3. do…while循环

这三种循环可以做相同的事情，当然它们也有小的区别，至于它们的应用及区别，我们后面会详细讲解。这里我们来学习for循环

#### 6.1 for循环结构

而在讲解for循环格式之前，我们先来看一下前面我们讲过的一个内容：这段代码的作用，是用来展示手机信息1000次。

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/5fca53f4c96f4cea8a29f85d67ff950b.png)

还提到了这里的几个部分，分别是定义变量，条件判断，控制变量的变化，展示手机信息(可能被多次执行)

而for循环语句也是由这几部分组成。

**格式：**

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/30923d04ad6144ae93a74bc4592bebc6.png)

**格式说明：**

- 初始化语句：这里可以是一条或者多条语句，这些语句用来完成初始化操作 **(int i=1)**
- 条件判断语句：这里使用一个结果值为boolean类型的表达式，这个表达式能决定是否执行循环体语句 **(i<=1000)**
- 循环体语句：这里可以是任意语句，这些语句可能被多次执行 **(展示手机信息)**
- 条件控制语句：这里通常是使用一条语句来改变变量的值，从而达到控制循环是否继续向下执行的效果 **(i+=1)**

**范例：**

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/ca4eb26a58664be2a136e1f4265e4c4d.png)

**执行流程：**

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/b772ed3b373440158c975031301addfb.png)

知道了for循环的格式和执行流程后，下面我们到IDEA中去演示一下：

```java
/*
    for循环结构
 */
public class ForDemo {
    public static void main(String[] args) {
        for(int i=1; i<=5; i+=1) {
            System.out.println("HelloWorld");
        }
    }
}
12345678910
```

代码演示后，通过Debug查看了一下程序的执行流程，让我们更清晰for循环的执行流程。

#### 6.2 案例1(输出数据)

需求：在控制台输出1-5的数据

首先，我们来简单的分析一下：

**分析：**

① 反复进行输出的动作，使用循环结构

② 从1开始到5结束，设置初始化从1开始

③ 从1开始到5结束，设置判断条件为没有到5的时候继续执行，执行到超过5程序结束

④ 从1到5，每次增加1，设置条件控制每次+1

⑤ 将反复进行的事情写入循环结构内部，打印对应数据

分析完毕之后，我们到IDEA中去实现一下：

```java
/*
    需求：在控制台输出1-5的数据
 */
public class ForTest01 {
    public static void main(String[] args) {
        System.out.println(1);
        System.out.println(2);
        System.out.println(3);
        System.out.println(4);
        System.out.println(5);
        System.out.println("--------------");

        for (int i = 1; i <= 5; i += 1) {
            System.out.println(i);
        }
        System.out.println("--------------");

        for (int i = 1; i <= 5; i += 2) {
            System.out.println(i);
        }
        System.out.println("--------------");

        //自增运算符：++
        //它跟在变量的后面表示变量的值+1
        for (int i = 1; i <= 5; i++) {
            System.out.println(i);
        }
        System.out.println("--------------");

        for (int i = 1; i <= 5; i++,i++) {
            System.out.println(i);
        }
        System.out.println("--------------");

        //我要获取数据5-1该怎么办呢？
        for (int i=5; i>=1; i-=1) {
            System.out.println(i);
        }
        System.out.println("--------------");

        for (int i=5; i>=1; i--) {
            System.out.println(i);
        }

    }
}
12345678910111213141516171819202122232425262728293031323334353637383940414243444546
```

在讲解的过程中，我们还提出了自增运算符：++和自减运算符：–，并且演示了如何获取数据5-1。

#### 6.3 案例2(求和思想)

需求：求1-5之间的数据和，并把求和结果在控制台输出

首先，我们先到IDEA中去实现一下，然后再回来总结。

```java
/*
    需求：求1-5之间的数据和，并把求和结果在控制台输出
 */
public class ForTest02 {
    public static void main(String[] args) {
        //定义一个求和变量，用于保存求和的结果
        int sum = 0;

        //我们通过for循环实现获取数据1-5
        for (int i=1; i<=5; i++) {
            //i,1,2,3,4,5
//            sum = sum + i;
            sum += i;
            /*
                第一次求和：sum = sum + i = 0 + 1 = 1
                第二次求和：sum = sum + i = 1 + 2 = 3
                第三次求和：sum = sum + i = 3 + 3 = 6
                第四次求和：sum = sum + i = 6 + 4 = 10
                第五次求和：sum = sum + i = 10 + 5 = 15
             */
        }

        //输出结果
        System.out.println("1-5的求和结果是：" + sum);
    }
}
1234567891011121314151617181920212223242526
```

最后，我们来总结一下求和思想的实现步骤：

**实现步骤：**

① 求和的最终结果必须保存起来，需要定义一个变量，用于保存求和的结果，初始值为0

② 从1开始到5结束的数据，使用循环结构完成

③ 将反复进行的事情写入循环结构内部

此处反复进行的事情是将数据 i 加到用于保存最终求和的变量 sum 中

④ 当循环执行完毕时，将最终数据打印出来

#### 6.4 案例3(求偶数和)

需求：求1-100之间的偶数和，并把求和结果在控制台输出

首先，我们来简单的分析一下：

**分析：**

① 对1-100的数据求和与1-5的数据求和几乎完全一样，仅仅是结束条件不同

② 对1-100的偶数求和，需要对求和操作添加限制条件

③ 限制条件是偶数才参与运算，因此条件应该是判断是否是偶数

④ 当循环执行完毕时，将最终数据打印出来

分析完毕之后，我们到IDEA中去实现一下：

```java
/*
    需求：求1-100之间的偶数和，并把求和结果在控制台输出
 */
public class ForTest03 {
    public static void main(String[] args) {
        //1:求和的最终结果必须保存起来，需要定义一个变量，用于保存求和的结果，初始值为0
        int sum = 0;

        //2:对1-100的数据求和与1-5的数据求和几乎完全一样，仅仅是结束条件不同
        for (int i=1; i<=100; i++) {
            //3:对1-100的偶数求和，需要对求和操作添加限制条件，判断是否是偶数
            if(i % 2 == 0) {
                sum += i;
            }
        }

        //4:当循环执行完毕时，将最终数据打印出来
        System.out.println("1-100之间的偶数和是：" + sum);
    }
}
1234567891011121314151617181920
```

#### 6.5 案例4(水仙花数)

需求：在控制台输出所有的“水仙花数”

看到这个需求，我们首先要解决的问题就是，什么样的数据是“水仙花数”？它满足如下两个条件：

① 水仙花数是一个三位数

比如： [111 222 333 370 371](https://blog.csdn.net/m0_63815035/article/details/) 520 999

② 水仙花数的个位、十位、百位的数字立方和等于原数

比如：

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/1e2add470ee840559d9a704a1b1baa86.png)

知道了什么是水仙花数后，我们再来回顾一下如何获取一个数据的个位，十位，百位：

假设一个三位数为x，则

- 个位：x%10
- 十位：x/10%10
- 百位：x/100%10

了解了水仙花数相关的基础知识后，下面我们来说一下这个案例的实现步骤：

**实现步骤：**

① 获取三位数，通过循环实现

② 获取每一个三位数的个位，十位，百位

③ 判断该三位数是否是水仙花数

④ 输出水仙花数

知道了实现步骤，下面我们到IDEA中去实现一下：

```java
/*
    需求：在控制台输出所有的“水仙花数”
 */
public class ForTest04 {
    public static void main(String[] args) {
        //1:获取三位数，通过循环实现
//        for (int i=100; i<=999; i++) {
//
//        }

        for (int i = 100; i < 1000; i++) {
            //2:获取每一个三位数的个位，十位，百位
            int ge = i % 10;
            int shi = i / 10 % 10;
            int bai = i / 100 % 10;

            //3:判断该三位数是否是水仙花数
            if ((ge * ge * ge + shi * shi * shi + bai * bai * bai) == i) {
                //4:输出水仙花数
                System.out.println(i);
            }

        }

    }
}
1234567891011121314151617181920212223242526
```

#### 6.6 案例5(统计思想)

需求：统计“水仙花数”一共有多少个，并在控制台输出个数

首先，我们先到IDEA中去实现一下，然后再回来总结。

```java
/*
    需求：统计“水仙花数”一共有多少个，并在控制台输出个数
 */
public class ForTest05 {
    public static void main(String[] args) {
        //定义一个统计变量，用于数据的统计，初始化值为0
        int count = 0;

        for (int i = 100; i < 1000; i++) {
            int ge = i % 10;
            int shi = i / 10 % 10;
            int bai = i / 100 % 10;

            if ((ge * ge * ge + shi * shi * shi + bai * bai * bai) == i) {
//                System.out.println(i);
                //1,2,3,...
                count++;
            }
        }

        //输出水仙花的个数
        System.out.println("水仙花数一共有：" + count + "个");
    }
}
123456789101112131415161718192021222324
```

最后，我们来总结一下统计思想的实现步骤：

**实现步骤：**

① 定义统计变量count，初始化值为0

② 在判定水仙花数的过程中，满足条件不再输出，更改为修改count的值，使count+1

③ 输出统计变量的值

#### 6.7 案例6(回文数)

需求：输出所有五位数的回文数

看到这个需求，我们首先要解决的问题就是，什么样的数据是“回文数”？

那什么是“回文数”呢？一个数，无论是从左往右读,还是从右往左读，读起来都相同的数,叫做“回文数”

举例：

10101，12321：是回文数

12345：不是回文数

规律：

个位 = 万位

十位 = 千位

和百位无关

了解了回文数相关的基础知识后，我们来说一下这个案例的实现步骤：

**实现步骤：**

① 获取五位数，通过循环实现

② 获取每一个五位数的个位，十位，千位，万位

③ 判断该五位数是否是回文数

④ 输出回文数

知道了实现步骤，下面我们到IDEA中去实现一下：

```java
/*
    需求：输出所有五位数的回文数
 */
public class ForTest06 {
    public static void main(String[] args) {
        //1:获取五位数，通过循环实现
        for (int i = 10000; i < 100000; i++) {
            //2:获取每一个五位数的个位，十位，千位，万位
            int ge = i % 10;
            int shi = i / 10 % 10;
            int qian = i / 1000 % 10;
            int wan = i / 10000 % 10;

            //3:判断该五位数是否是回文数
            if ((ge == wan) && (shi == qian)) {
                //4:输出回文数
                System.out.println(i);
            }
        }

        //练习：统计五位数的回文数个数，并在控制台输出个数

    }
}
123456789101112131415161718192021222324
```

在案例的最后，我们留下了一个练习，大家记得完成哦。

#### 6.8 案例7(逢七过)

需求：朋友聚会的时候可能会玩一个游戏：逢七过。

规则是：从任意一个数字开始报数，当你要报的数字包含7或者是7的倍数时都要说：过。

为了帮助大家更好的玩这个游戏，这里我们直接在控制台打印出1-100之间的满足逢七必过规则的数据。

这样，大家将来在玩游戏的时候，就知道哪些数据要说：过。

首先，我们来简单的分析一下：

**分析：**

① 数据的范围1-100之间，用循环很容易实现

② 要满足的条件是：数字包含7(个位是7，或者十位是7)，或者是7的倍数

```java
假如有一个数据：x

判断个位为7：x%10 == 7

判断十位为7：x/10%10 == 7

判断是7的倍数：x%7 == 0
1234567
```

分析完毕后，我们来说一下实现步骤：

**实现步骤：**

① 获取1-100之间的数据，通过循环实现

② 判断数字包含7或者是7的倍数

判断数据：要么个位是7，要么十位是7，要么能够被7整除

③ 在控制台输出满足条件的数据

知道了实现步骤，下面我们到IDEA中去实现一下：

```java
/*
    需求：朋友聚会的时候可能会玩一个游戏：逢七过。
 */
public class ForTest07 {
    public static void main(String[] args) {
        //1:获取1-100之间的数据，通过循环实现
        for (int i = 1; i <= 100; i++) {
            //2:判断数字包含7或者是7的倍数(判断数据：要么个位是7，要么十位是7，要么能够被7整除)
            if ((i % 10 == 7) || (i / 10 % 10 == 7) || (i % 7 == 0)) {
                //3:在控制台输出满足条件的数据
                System.out.println(i);
            }
        }

    }
}
12345678910111213141516
```

### 7：while循环结构

#### 7.1 while循环结构

接下来，我们学习while循环结构语句

**格式：**

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/38035234cc8d4239acd64889efe5b136.png)

**范例：**

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/352daa437ade433ab13b447e77f48c54.png)

知道了while循环的格式后，下面我们到IDEA中去演示一下：

```java
/*
    while循环结构
 */
public class WhileDemo {
    public static void main(String[] args) {
        int i = 1;
        while (i<=5) {
            System.out.println("HelloWorld");
            i++;
        }
    }
}
123456789101112
```

代码演示后，通过Debug查看了一下程序的执行流程，让我们更清晰while循环的执行流程。

最后，我们再来总结一下while循环的执行流程：

**执行流程：**

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/9bc097eedcb1448ba5200af8149341bb.png)

#### 7.2 案例1(求奇数和)

需求：求1-100之间的奇数和，并把求和结果在控制台输出

首先，我们来简单的分析一下：

**分析：**

① 对1-100的奇数求和，和前面讲解的偶数求和几乎是完全一样，仅仅是判断条件不同

② 判断条件是奇数才参与运算，因此条件应该是判断是否是奇数

③ 当循环执行完毕时，将最终数据打印出来

分析完毕之后，我们到IDEA中去实现一下：

```java
/*
    需求：求1-100之间的奇数和，并把求和结果在控制台输出
 */
public class WhileTest01 {
    public static void main(String[] args) {
        //定义求和变量，初始化值为0
        int sum = 0;

        //获取1-100之间的数据
//        int i = 1;
//        while (i<=100) {
//            //判断数据是否是奇数
            if(i%2 != 0) {
                sum += i;
            }
//
//            if(i%2 == 1) {
//                sum += i;
//            }
//
//            i++;
//        }

        int i = 1;
        while (i <= 100) {
            sum += i;
            i += 2; //1,3,5,7...99,101
        }

        //输出结果
        System.out.println("1-100之间的奇数和是：" + sum);
    }
}
123456789101112131415161718192021222324252627282930313233
```

#### 7.3 案例2(珠穆朗玛峰)

需求：世界最高峰珠穆朗玛峰(8848.86m)，我现在有一张足够大的纸张，厚度为：0.001m。请问，我折叠多少次，就可以保证厚度不低于珠穆朗玛峰的高度?

首先，我们来简单的分析一下：

**分析：**

① 因为要反复折叠，所以要使用循环，该选for循环还是while循环呢？

**小技巧：循环次数明确，使用for循环；循环次数不明确，使用while循环**

```java
这里不知道折叠多少次，这种情况下更适合使用while循环
1
```

② 纸张每折叠一次，厚度加倍，因此要先定义纸张厚度，在循环中使厚度加倍

③ 什么时候就停止折叠了呢？直到纸张的厚度大于等于珠峰的高度，反言之，就要折叠

④ 要求的是统计折叠次数，所以会用到统计思想

分析完毕后，我们来说一下实现步骤：

**实现步骤：**

① 定义统计变量，初始化值为0

② 定义纸张厚度变量和珠峰高度变量

③ 用while循环实现反复折叠，判断条件是纸张厚度小于珠峰高度

④ 循环体中要做两件事情：一是纸张厚度加倍，二是统计变量+1

⑤ 当循环结束，输出统计变量的值

知道了实现步骤，下面我们到IDEA中去实现一下：

```java
/*
    需求：世界最高峰珠穆朗玛峰(8848.86m)，我现在有一张足够大的纸张，厚度为：0.001m。
         请问，我折叠多少次，就可以保证厚度不低于珠穆朗玛峰的高度?
 */
public class WhileTest02 {
    public static void main(String[] args) {
        //1:定义统计变量，初始化值为0
        int count = 0;

        //2:定义纸张厚度变量和珠峰高度变量
        double paper = 0.001;
        double zf = 8848.86;

        //3:用while循环实现反复折叠，判断条件是纸张厚度小于珠峰高度
        while (paper < zf) {
            //4:循环体中要做两件事情：一是纸张厚度加倍，二是统计变量+1
            paper *= 2;

            count++;
        }

        //5:当循环结束，输出统计变量的值
        System.out.println("要折叠" + count + "次");
    }
}
12345678910111213141516171819202122232425
```

### 8：do-while循环结构

#### 8.1 do-while循环结构

接下来，我们学习do-while循环结构语句

**格式：**

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/3040d58b86db4e478eca4c9ea142320c.png)

**范例：**

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/d8c552e7a31845ce9e299e67554188f4.png)

知道了do-while循环的格式后，下面我们到IDEA中去演示一下：

```java
/*
    do...while循环结构
 */
public class DoWhileDemo {
    public static void main(String[] args) {
        int i = 1;
        do {
            System.out.println("HelloWorld");
            i++;
        } while (i<=5);
    }
}
123456789101112
```

代码演示后，通过Debug查看了一下程序的执行流程，让我们更清晰do-while循环的执行流程。

最后，我们再来总结一下do-while循环的执行流程：

**执行流程：**

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/dfa210cd399641f49959ddfd1cf3771d.png)

#### 8.2 三种循环的区别

前面我们讲解了三种循环语句的格式和执行流程，下面我们来讲解这三种循环语句的区别。

而关于这三种循环语句的区别，我们先到IDEA中去讲解，然后再回来总结：

```java
/*
    三种循环的区别
 */
public class LoopTest {
    public static void main(String[] args) {
//        //for循环
//        for (int i = 3; i < 3; i++) {
//            System.out.println("我爱Java");
//        }
//        System.out.println("--------");
//
//        //while循环
//        int j = 3;
//        while (j < 3) {
//            System.out.println("我爱Java");
//            j++;
//        }
//        System.out.println("--------");
//
//        //do...while循环
//        int k = 3;
//        do {
//            System.out.println("我爱Java");
//            k++;
//        } while (k < 3);

//        //for循环
//        for (int i = 1; i < 3; i++) {
//            System.out.println("我爱Java");
//        }
        System.out.println(i);
//        System.out.println("--------");
//
//        //while循环
//        int j = 1;
//        while (j < 3) {
//            System.out.println("我爱Java");
//            j++;
//        }
//        System.out.println(j);
//        System.out.println("--------");

        //死循环
//        for (;;) {
//            System.out.println("for...");
//        }

//        while (true) {
//            System.out.println("while...");
//        }

        do {
            System.out.println("do...while...");
        } while (true);

    }
}
123456789101112131415161718192021222324252627282930313233343536373839404142434445464748495051525354555657
```

讲解完毕后，回到资料，我们总结一下：

**三种循环语句的区别：**

for循环和while循环 **先判断条件是否成立** ，然后决定是否执行循环体（先判断后执行）

do…while循环 **先执行一次循环体** ，然后判断条件是否成立，是否继续执行循环体（先执行后判断）

**for和while的区别：**

条件控制语句所控制的自增变量，在for循环结束后，就 **不可以继续使用** 了

条件控制语句所控制的自增变量，在while循环结束后， **还可以继续使用**

**死循环格式：**

for(;; ){}

**while(true) {}**

do{}while(true);

由于循环语句的区别，只是大家需要理解的知识点，故这里不需要练习，我们在后面的使用中，在慢慢体会即可。

### 9：continue和break

#### 9.1 continue和break

下面我们来学习跳转控制语句，为了讲解跳转控制语句，这里我们给出几个场景看一看：

场景一：周一到周五上班，周六日不上班

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/289c08a3f9e8446d9b5c1e750be96a24.png)

场景二：成人后一直工作到60岁，60岁之后就可以退休养老了

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/3d66d148cde34b06a35eba4893212de3.png)

刚才的场景中，重点介绍了两个跳转关键字：

- **continue** 用在循环中，基于条件控制，跳过某次循环体内容的执行，继续下一次的执行
- **break** 用在循环中，基于条件控制，终止循环体内容的执行，也就是说结束当前的整个循环

了解了这两个跳转关键字之后，下面我们到IDEA中去体验一下：

```java
/*
   continue:用在循环中，基于条件控制，跳过某次循环体内容的执行，继续下一次的执行
   break:用在循环中，基于条件控制，终止循环体内容的执行，也就是说结束当前的整个循环
*/
public class ControlDemo {
    public static void main(String[] args) {
        for (int i = 1; i <= 5; i++) {
            if (i % 2 == 0) {
//                continue;
                break;
            }

            System.out.println(i);
        }
    }
}
12345678910111213141516
```

#### 9.2 综合案例(小芳存钱)

需求：小芳的妈妈每天给她2.5元钱，她都会存起来，但是，每当这一天是存钱的第5天或者5的倍数的话，

她都会花去6元钱，请问，经过多少天，小芳才可以存到100元钱。

关于这个案例呢，我们到IDEA中一边分析，一边实现：

```java
/*
    需求：小芳的妈妈每天给她2.5元钱，她都会存起来，但是，每当这一天是存钱的第5天或者5的倍数的话，她都会花去6元钱，请问，经过多少天，小芳才可以存到100元钱。
*/
public class ControlTest {
    public static void main(String[] args) {
        //小芳的妈妈每天给她2.5元钱
        double dayMoney = 2.5;

        //她都会存起来，涉及到了求和思想，定义求和变量，初始化值为0
        double sumMoney = 0;

        //存到100元钱
        int result = 100;

        //定义一个统计变量，用来纪录存钱的天数，初始化值为1
        int dayCount = 1;

        //因为不知道要多少天才能够存到100元，所以，这里我们采用死循环来实现，当存到100元的时候，通过break跳转语句让循环结束
        while (true) {
            //存钱
            sumMoney += dayMoney;

            //判断存的钱是否大于等于100了，如果是，就退出循环
            if(sumMoney >= result) {
                break;
            }

            //每当这一天是存钱的第5天或者5的倍数的话，她都会花去6元钱
            if(dayCount%5 == 0) {
                sumMoney -= 6;
                System.out.println("第" + dayCount + "天花了6元");
            }

            dayCount++;
        }

        //输出统计天数的变量
        System.out.println("共花了" + dayCount + "天存了100元");
    }
}
12345678910111213141516171819202122232425262728293031323334353637383940
```

## 五、方法

**本节目标：**

- 能够知道方法的好处
- 能够根据两个明确分析方法的参数和返回值
- 能够编写方法完成授课案例，并在主方法中完成方法的调用
- 能够知道方法重载及其特点

### 10：方法的定义和使用

#### 10.1 方法概述和课程安排

下面我们来学习Java中很重要的一个知识，就是方法，那什么是方法呢？我们一起来说一下：

**方法(method)：** 就是完成特定功能的代码块

如何理解这句话呢?来，我们看一段代码，相信这个大家应该已经很熟悉了

这就是我们的main方法，也就是我们说的主方法。它里面的代码的功能：是在控制台输出一个字符串数据：HelloWorld

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/b90bf6d00dfc4708b0365bfa21005351.png)

我们再来看另一段代码：

这里出现了三个方法，主方法的作用，还是在控制台输出一个字符串数据：HelloWorld。而后面这两个方法的作用：分别是在控制台输出字符串数据：method1和method2

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/dc1a601b5a844440b05da4ab49a6266f.png)

这些代码都是用一对大括号括起来的，所以我们说，方法就是完成特定功能的代码块。

知道了什么是方法后，我们来说一下为什么要学习方法，也就是方法的好处

看这里，植物大战僵尸这个游戏，估计有人玩过。

外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传

没玩过的，回去下载下来玩一下，我一直觉得玩游戏，对学编程是有帮助的，它能够打开我们的思维， 当然前提是适度的玩游戏，你天天玩，不好好学习，那肯定是不行的。

回到这里，我们继续，在这个游戏中，有这样的一些射手，它们通过发射炮弹去消灭僵尸

假如，现在我们来编写代码，实现发射炮弹的动作。

首先，我们来看豌豆射手要发射炮弹，而发射炮弹呢？需要20行代码实现。

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/b5a5f20862aa49d583ba3a8a83381023.png)

这里代码我们就省略了啊，知道这个意思就行。

接着，寒冰射手要发射炮弹，我们还是要编写20行代码实现。

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/8f872f0b6d2d473e829bdc815cd327a1.png)

再接着，大头菜射手也要发射炮弹，我们还得再编写20行代码实现。

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/53ecbc01812e4b5ca118a47daeeaa16a.png)

写到这里，我们发现太麻烦了，每个射手发射炮弹，我们都要写发射炮弹的代码。

而发射炮弹的代码是相同的，所以，目前我们的代码就出现问题了。

问题是：代码的重复度很高，复用性太差了。

**那怎么解决呢？**

看这里，关于这三个射手要发射炮弹的代码，我们不用针对每个射手都写，

而是把发射炮弹的代码打包，定义一个方法：叫做发射。

将来这三个射手要发射炮弹的时候，直接调用发射的方法就可以了。

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/80ec39cb0ec149c594af5d43238e56a7.png)

而且，再加入一个新的射手，这个射手也要发射炮弹，我们也是直接调用发射的方法就可以了。

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/49af25367f17411686d557292c0ff084.png)

这样新的射手也可以发射炮弹了。

这样我们就减少了代码的编写，所以说，方法一个非常大的好处就是提高了代码的复用性。

了解了什么是方法，以及方法的好处后。我们来说一下方法这一节的课程安排：

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/e8afa304061a4bd3b7ee932502f861d4.png)

首先，我们会讲解基本的方法的定义和调用

接着讲解带参方法和带返回值方法的定义和调用

方法的定义和调用完毕之后，讲解方法的注意事项，避免大家在定义方法时出现一些小问题。

注意事项讲解完毕之后，讲解方法的通用格式，给大家总结，其实方法就一种格式，

并非有上面那么多种方法格式，上面之所以这样讲解，是想通过循序渐进的方式，让大家更好的掌握方法的定义和使用

在方法通用格式这一块，还会重点讲解如何设计方法，并通过多个练习来强化方法的定义和使用，

只要大家能够跟着完成这些练习，方法我们基本上就算掌握了。

最后，我们会讲解方法中一个重要的特性：方法重载。

好了，到此关于方法的概述和课程安排我们就先讲到这里

#### 10.2 方法的定义和调用

下面呢我们来学习方法的定义和调用。

**格式：**

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/46f7d8770cc74424ae8284cf64d508bf.png)

**范例：**

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/4e9eb8c5a2ff40a38824a8bda1b61e34.png)

知道了方法的定义格式后，我们到IDEA中去演示一下：

```java
/*
    定义格式：
        public static void 方法名() {
           //方法体
       }
 */
public class MethodDemo {
    public static void main(String[] args) {
        //调用方法
        isEvenNumber();
    }

    //需求：定义一个方法，在方法中定义一个变量，判断该数据是否是偶数
    public static void isEvenNumber() {
        //在方法中定义一个变量
        int number = 10;
        number = 9;

        //判断该数据是否是偶数
        if (number % 2 == 0) {
            System.out.println(number + "是偶数");
        } else {
            System.out.println(number + "不是偶数");
        }
    }
}
1234567891011121314151617181920212223242526
```

演示完毕之后，回到资料我们总结一下方法的调用和注意事项：

**格式：**

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/024d2a3d01d546f481c9c8cb9939ed45.png)

**范例：**

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/4439352fcff44e9a9e1b99cc2c8193ac.png)

**注意事项：**

- 方法定义完毕后， **需要调用才能执行**
- 方法必须 **先定义后调用** ，否则程序将报错

#### 10.3 Debug查看方法调用

按照 Debug 的正常使用即可，但是要注意如下事项：

- 进入一个方法的时候，需要用 Step Into F7
- 在方法内部，看每一行代码的执行流程，使用 Step Over F8
- 注意观察方法的出现和消失，以及变量的变化

#### 10.4 练习1(输出较大值)

需求：设计一个方法用于打印两个数中的较大数

首先，我们来简单的分析一下：

**分析：**

① 定义一个方法，用于打印两个数字中的较大数，例如：getMax()

② 方法中定义两个变量，用于保存两个数字

③ 使用if语句对两个数字的大小关系进行处理

④ 在main()方法中调用定义好的方法

分析完毕之后，我们到IDEA中去实现一下：

```java
/*
    需求：设计一个方法用于打印两个数中的较大数

    分析：
        1:定义一个方法，用于打印两个数字中的较大数，例如：getMax()
        2:方法中定义两个变量，用于保存两个数字
        3:使用if语句对两个数字的大小关系进行处理
        4:在main()方法中调用定义好的方法
 */
public class MethodTest {
    public static void main(String[] args) {
        //在main()方法中调用定义好的方法
        getMax();
    }

    //定义一个方法，用于打印两个数字中的较大数，例如：getMax()
    public static void getMax() {
        //方法中定义两个变量，用于保存两个数字
        int a = 10;
        int b = 20;

        //使用if语句对两个数字的大小关系进行处理
        if(a >= b) {
            System.out.println("较大的数是：" + a);
        } else {
            System.out.println("较大的数是：" + b);
        }
    }
}
1234567891011121314151617181920212223242526272829
```

#### 10.5 带参数方法的定义和调用

下面呢我们来学习带参数方法的定义和调用。

**格式：**

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/b49914f5c21f4a29aedf79d6eb462d1d.png)

**范例：**

![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/be60a8c57494457abbaebe06b9af4a17.png)  
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/003390ac7c6f4a9c9b10c1be6b2f6646.png)

**注意事项：**

- 带参方法定义时，参数中的 **数据类型** 与 **变量名** 都不能缺少，缺少任意一个程序将报错
- 带参方法定义时，多个参数之间使用 **逗号** (,)分隔

知道了带参数方法的定义格式后，我们到IDEA中去演示一下：

```java
/*
    带参数方法的定义和调用

    定义格式：
        public static void 方法名(参数) { … … }
 */
public class MethodDemo {
    public static void main(String[] args) {
        //字面量值调用
        isEvenNumber(10);
        isEvenNumber(9);

        //变量的调用
        int number = 11;
        isEvenNumber(number);
        number = 12;
        isEvenNumber(number);
    }

    //需求：定义一个方法，该方法接收一个参数，判断该数据是否是偶数
    public static void isEvenNumber(int number) {
        if (number % 2 == 0) {
            System.out.println(true);
        } else {
            System.out.println(false);
        }
    }
}
12345678910111213141516171819202122232425262728
```

演示完毕之后，回到资料我们总结一下带参数方法的调用和注意事项：

**格式：**

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/cedf8f64db8a4bd2b92013d688e5ee31.png)

**范例：**

![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/b664c5c8d7fa4f0e951254014b75e947.png)

![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/e242347b5e84491ea22e410985bc1983.png)

**注意事项：**

- 带参方法调用时，参数的 **数量与类型** 必须与方法定义中的设置相匹配，否则程序将报错

#### 10.6 形参和实参

这里我们讲解一个小知识点，形参和实参，那什么是形参和实参呢？

形参：方法定义中的参数

等同于变量定义格式，例如：int number

实参：方法调用中的参数

等同于使用变量或字面量，例如： 10 number

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/c0eff96189764955a25449b9fa6e90cc.png)

大家能够知道形参和实参分别表示哪里的参数就可以了。

#### 10.7 练习2(输出较大值)

需求：设计一个方法用于打印两个数中的较大数，数据来自于方法参数

首先，我们来简单的分析一下：

**分析：**

① 定义一个方法，用于打印两个数字中的较大数，例如：getMax()

② 为方法定义两个参数，用于接收两个数字

③ 使用if语句对两个数字的大小关系进行处理

④ 在main()方法中调用定义好的方法（使用字面量）

⑤ 在main()方法中调用定义好的方法（使用变量）

分析完毕之后，我们到IDEA中去实现一下：

```java
/*
    需求：设计一个方法用于打印两个数中的较大数，数据来自于方法参数

    分析：
        1:定义一个方法，用于打印两个数字中的较大数，例如：getMax()
        2:为方法定义两个参数，用于接收两个数字
        3:使用if语句对两个数字的大小关系进行处理
        4:在main()方法中调用定义好的方法（使用字面量）
        5:在main()方法中调用定义好的方法（使用变量）
 */
public class MethodTest {
    public static void main(String[] args) {
        //在main()方法中调用定义好的方法（使用字面量）
        getMax(10,20);
//        getMax(a:10,b:20); //idea的智能提示，不要手动的去写a,b
//        getMax(30);
//        getMax(10.0,20,0);
        //调用方法的时候，人家要几个，你就给几个，人家要什么类型，你就给什么类型

        //在main()方法中调用定义好的方法（使用变量）
//        int a = 10;
//        int b = 20;
//        getMax(a,b);
        int x = 10;
        int y = 20;
        getMax(x,y);
    }

    //定义一个方法，用于打印两个数字中的较大数，例如：getMax()
    //为方法定义两个参数，用于接收两个数字
    public static void getMax(int a, int b) {
        //使用if语句对两个数字的大小关系进行处理
        if(a >= b) {
            System.out.println("较大的数是：" + a);
        }else {
            System.out.println("较大的数是：" + b);
        }
    }
}
123456789101112131415161718192021222324252627282930313233343536373839
```

#### 10.8 带返回值方法的定义和调用

下面呢我们来学习带返回值方法的定义和调用。

**格式：**

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/9d943cf65e6d4daa8847f1637742820c.png)

**范例：**

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/7f8eb775b4804927b21a0d04e868ed6f.png)

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/0342baa8d92548f084cadbc1b0da8c0b.png)

**注意事项：**

- 方法定义时return后面的返回值与方法定义上的 **数据类型要匹配** ，否则程序将报错

知道了带返回值方法的定义格式后，我们到IDEA中去演示一下：

```java
/*
    带返回值方法的定义和调用

    定义格式：
        public static 数据类型 方法名(参数) {
           return 数据;
       }
 */
public class MethodDemo {
    public static void main(String[] args) {
//        isEvenNumber(10);
//        //true;

        boolean flag = isEvenNumber(10);
        //boolean flag = true;
        System.out.println(flag);

//        if(flag) {
//            System.out.println("是偶数就输出这句话");
//        }
    }

    //需求：定义一个方法，该方法接收一个参数，判断该数据是否是偶数，并返回真假值
    public static boolean isEvenNumber(int number) {
        if (number % 2 == 0) {
            return true;
        } else {
            return false;
        }
    }
}
12345678910111213141516171819202122232425262728293031
```

演示完毕之后，回到资料我们总结一下带返回值方法的调用和注意事项：

**格式：**

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/920a0f2552ac489c8f8cfcbb0a430d06.png)

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/71320e68348e450aaf3320969c721ec8.png)

**注意事项：**

- 方法的返回值 **通常会使用变量接收** ，否则该返回值将无意义

#### 10.9 练习3(输出较大值)

需求：设计一个方法可以获取两个数的较大值，数据来自于参数

首先，我们来简单的分析一下：

**分析：**

① 定义一个方法，用于获取两个数字中的较大数，例如：getMax()

② 使用if语句对两个数字的大小关系进行处理

③ 根据题设分别设置两种情况下对应的返回结果

④ 在main()方法中调用定义好的方法并使用变量保存

分析完毕之后，我们到IDEA中去实现一下：

```java
/*
    需求：设计一个方法可以获取两个数的较大值，数据来自于参数

    分析：
        1:定义一个方法，用于获取两个数字中的较大数，例如：getMax()
        2:使用if语句对两个数字的大小关系进行处理
        3:根据题设分别设置两种情况下对应的返回结果
        4:在main()方法中调用定义好的方法并使用变量保存
 */
public class MethodTest {
    public static void main(String[] args) {
        //在main()方法中调用定义好的方法并使用变量保存
//        int max = getMax(10,20);
//        System.out.println(max);

        int max = getMax(10, 20); //.var的使用，它能够帮我们自动补齐左边的内容
        System.out.println(max); //max.sout，能够把max变量放到输出语句中

        System.out.println(getMax(10,20));
        System.out.println(getMax(10, 20));
    }

    //定义一个方法，用于获取两个数字中的较大数，例如：getMax()
    public static int getMax(int a,int b) {
        //使用if语句对两个数字的大小关系进行处理
        //根据题设分别设置两种情况下对应的返回结果
        if(a >= b) {
            return a;
        } else {
            return b;
        }
    }
}
123456789101112131415161718192021222324252627282930313233
```

#### 10.10 方法的注意事项

下面我们来说一下方法的注意事项，讲解注意事项，是为了让我们以后能够避免类似的问题，这里呢我们讲解两个注意事项：

1. 方法不能嵌套定义
	![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/1553bfc905364f01ae953e62bad4c6af.png)
2. void表示无返回值，可以省略return，也可以单独的书写return，后面不加数据
	![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/03a8f472181447ab8e7c33671a20c29a.png)

讲解完毕后，到IDEA中去演示一下：

```java
/*
    方法注意事项：
        方法不能嵌套定义
        void表示无返回值，可以省略return，也可以单独的书写return，后面不加数据
 */
public class MethodDemo {
    public static void main(String[] args) {

    }

    public static void methodOne() {
        return;
    }

    public static void methodTwo() {
//        return 100;

        return;

//        System.out.println("HelloWorld");
    }
}
12345678910111213141516171819202122
```

到此，方法的注意事项，我们就讲解完毕了。大家了解即可，自己定义方法的时候，注意就好。

### 11：方法的通用格式

#### 11.1 方法通用格式

前面呢，我们讲解了方法定义的多种格式，其实呢，方法定义只有一种格式，这里我们来看一下方法定义的通用格式：

**格式：**

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/243ff0f66ad74ccb9cd7fa65fbebcaf4.png)

**格式说明：**

- public static 修饰符，目前先记住这个格式
- 返回值类型 方法操作完毕之后返回的数据的数据类型，如果方法操作完毕，没有数据返回，这里写void，而且方法体中一般不写return
- 方法名 调用方法时候使用的标识
- 参数 由数据类型和变量名组成，多个参数之间用逗号隔开
- 方法体 完成功能的代码块
- return 如果方法操作完毕，有数据返回，用于把数据返回给调用者

现在我们就知道了一个完整的方法格式了，那后续我们在自己编写方法的时候，如何正确的编写一个方法呢？这里给大家说一个小技巧：

定义方法时，要做到 **两个明确**

- 明确返回值类型： 主要是明确方法操作完毕之后是否有数据返回，如果没有，写void；如果有，写对应的数据类型
- 明确参数： 主要是明确参数的类型和数量

而在调用方法时，我们要知道下面两种不同返回值类型的方法调用：

- void类型的方法，直接调用即可
- 非void类型的方法，推荐用变量接收调用

这里我们总结了一下方法的通用格式和对应的说明。以及告诉了大家以后自己如何定义方法，并进行方法调用。下面我们就需要通过练习来强化方法的定义和调用。

#### 11.2 练习1(求和)

需求：设计一个方法用于求1-n之间的数据和(n>1)，返回求和结果。调用方法，把结果在控制台输出。

首先，我们来简单的分析一下：

**分析：**

① 方法定义

```java
使用两个明确分析该方法的参数和返回值

参数：int n

返回值类型：int
12345
```

② 方法调用

```java
变量接收调用
1
```

分析完毕之后，我们到IDEA中去实现一下：

```java
/*
    需求：设计一个方法用于求1-n之间的数据和(n>1)，返回求和结果。调用方法，把结果在控制台输出。
 */
public class MethodTest01 {
    public static void main(String[] args) {
        int result = sum(5);
        System.out.println("1-5的和是：" + result);

        result = sum(100);
        System.out.println("1-100的和是：" + result);
    }

    /*
       使用两个明确分析该方法的参数和返回值
        参数：int n
        返回值类型：int
     */
    public static int sum(int n) {
        int sum = 0;

        for (int i=1; i<=n; i++) {
            sum += i;
        }

        return sum;
    }
}
123456789101112131415161718192021222324252627
```

#### 11.3 练习2(比较相等)

需求：设计一个方法用于比较两个整数是否相等，调用方法，把结果在控制台输出。

首先，我们来简单的分析一下：

**分析：**

① 方法定义

```java
使用两个明确分析该方法的参数和返回值

参数：int a,int b

返回值类型：boolean
12345
```

② 方法调用

```java
变量接收调用
1
```

分析完毕之后，我们到IDEA中去实现一下：

```java
/*
    需求：设计一个方法用于比较两个整数是否相等，调用方法，把结果在控制台输出。
 */
public class MethodTest02 {
    public static void main(String[] args) {
        boolean flag = compare(10, 20);
        System.out.println("10和20相等吗：" + flag);

        flag = compare(10,10);
        System.out.println("10和10相等吗：" + flag);
    }

    /*
        使用两个明确分析该方法的参数和返回值
        参数：int a,int b
        返回值类型：boolean
     */
    public static boolean compare(int a,int b) {
        //比较两个整数是否相等
//        if(a == b) {
//            return true;
//        } else {
//            return false;
//        }

//        boolean flag = (a == b) ? true : false;
//        return flag;

//        boolean flag = (a == b);
//        return flag;

        return a == b;
    }
}
12345678910111213141516171819202122232425262728293031323334
```

#### 11.4 练习3(较大值)

需求：设计一个方法用于获取三个整数较大值，调用方法，把结果在控制台输出。

首先，我们来简单的分析一下：

**分析：**

① 方法定义

```java
使用两个明确分析该方法的参数和返回值

参数：int a,int b,int c

返回值类型：int
12345
```

② 方法调用

```java
变量接收调用
1
```

分析完毕之后，我们到IDEA中去实现一下：

```java
/*
    需求：设计一个方法用于获取三个整数较大值，调用方法，把结果在控制台输出。
 */
public class MethodTest03 {
    public static void main(String[] args) {
        int max = getMax(10, 20, 30);
        System.out.println("10,20,30中的较大值是：" + max);
    }

    /*
        使用两个明确分析该方法的参数和返回值
        参数：int a,int b,int c
        返回值类型：int
     */
    public static int getMax(int a, int b, int c) {
        //获取三个整数较大值
//        if (a >= b) {
//            if (a >= c) {
//                return a;
//            } else {
//                return c;
//            }
//        } else {
//            if (b >= c) {
//                return b;
//            } else {
//                return c;
//            }
//        }

        int tempMax = a > b ? a : b;
        int max = tempMax > c ? tempMax : c;
        return max;
    }
}
1234567891011121314151617181920212223242526272829303132333435
```

#### 11.5 练习4(水仙花)

需求：设计一个方法用于判断一个整数是否是水仙花数，调用方法，把结果在控制台输出。

首先，我们来简单的分析一下：

**分析：**

① 方法定义

```java
使用两个明确分析该方法的参数和返回值

参数：int number

返回值类型：boolean
12345
```

② 方法调用

```java
变量接收调用
1
```

分析完毕之后，我们到IDEA中去实现一下：

```java
/*
    需求：设计一个方法用于判断一个整数是否是水仙花数，调用方法，把结果在控制台输出。
 */
public class MethodTest04 {
    public static void main(String[] args) {
//        boolean flag = isFlower(111);
//        System.out.println(flag);
//
//        flag = isFlower(153);
//        System.out.println(flag);

        for (int i=100; i<1000; i++) {
            //i
//            boolean flag = isFlower(i);
//            if(flag) {
//                System.out.println(i);
//            }
            if(isFlower(i)) {
                System.out.println(i);
            }
        }
    }

    /*
       使用两个明确分析该方法的参数和返回值
        参数：int number
        返回值类型：boolean
     */
    public static boolean isFlower(int number) {
        //判断一个整数是否是水仙花数
        int ge = number % 10;
        int shi = number / 10 % 10;
        int bai = number / 100 % 10;

        if ((ge * ge * ge + shi * shi * shi + bai * bai * bai) == number) {
            return true;
        } else {
            return false;
        }
    }
}
1234567891011121314151617181920212223242526272829303132333435363738394041
```

### 12：方法重载

#### 12.1 方法重载

我们学习方法中一个非常重要的特性：方法重载。

首先，我们来说一下，什么是方法重载。

\*\*方法重载：\*\*指同一个类中定义的多个方法之间的关系，满足下列条件的多个方法相互构成重载

- 多个方法在同一个类中
- 多个方法具有相同的方法名
- 多个方法的参数不相同，类型不同或者数量不同

如下图：

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/65ac9147f95c46fdb4a88f63fcd46ed8.png)

知道了什么是方法重载后，我们来说一下 **方法重载的特点：**

- 类型不同或者数量不同重载仅对应方法的定义，与方法的调用无关，调用方式参照标准格式
- 重载仅针对同一个类中方法的名称与参数进行识别，与返回值无关，换句话说不能通过返回值来判定两个方法是否相互构成重载

如下图：

![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/b6d172fe86d64b17a64348af8aa368f0.png)

知道了方法重载及其特点后，我们到IDEA中去体验一下：

```java
/*
    方法重载：
        多个方法在同一个类中
        多个方法具有相同的方法名
        多个方法的参数不相同，类型不同或者数量不同

        调用方法的时候，Java虚拟机会通过参数的不同来区分同名的方法
 */
public class MethodDemo {
    public static void main(String[] args) {
        //调用方法
        int result = sum(10, 20);
        System.out.println(result);

        double result2 = sum(10.0, 20.0);
        System.out.println(result2);

        int result3 = sum(10, 20, 30);
        System.out.println(result3);
    }

    //需求1：求两个int类型数据和的方法
    public static int sum(int a,int b) {
        return a + b;
    }

    //需求2：求两个double类型数据和的方法
    public static double sum(double a,double b) {
        return a + b;
    }

    //需求3：求三个int类型数据和的方法
    public static int sum(int a,int b,int c) {
        return a + b + c;
    }
}
123456789101112131415161718192021222324252627282930313233343536
```

#### 12.2 练习(比较相等)

需求：使用方法重载的思想，设计比较两个整数是否相等的方法，兼容全整数类型（byte,short,int,long）

比较整数是否想等，前面我们已经做过了，这里只不过是写几个重载的方法而已，基本思路讲解过了，这里就不在讲解了，我们直接到idea中去实现

```java
/*
    需求：使用方法重载的思想，设计比较两个整数是否相等的方法，兼容全整数类型（byte,short,int,long）
 */
public class MethodTest {
    public static void main(String[] args) {
        System.out.println(compare(10,20));
        System.out.println(compare((byte) 10,(byte) 20));
        System.out.println(compare((short) 10,(short) 20));
        System.out.println(compare(10L,20L));
    }

    //int
    public static boolean compare(int a,int b) {
        System.out.println("int");
        return a == b;
    }

    //byte
    public static boolean compare(byte a,byte b) {
        System.out.println("byte");
        return a == b;
    }

    //short
    public static boolean compare(short a,short b) {
        System.out.println("short");
        return a == b;
    }

    //long
    public static boolean compare(long a,long b) {
        System.out.println("long");
        return a == b;
    }

}
123456789101112131415161718192021222324252627282930313233343536
```

## 六、数组

**本节目标：**

- 能够知道数组的作用
- 能够根据需求完成数组的定义和初始化
- 能够使用数组完成授课案例
- 能够理解数组内存图

### 13：一维数组

#### 13.1 数组概述和课程安排

下面我们来学习数组。

那什么是数组呢？为了帮助大家理解，这里我们来看这样的一个场景：

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/f84c4606ada9411d914b47bd7eb37a1d.png)

看这里，有一个学员的考试成绩，为了存储这个学员的考试成绩，我们可以采用一个变量进行存储。

但是，假如这里有很多个学员的考试成绩，我们要存储该怎么办呢？

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/f0e6f3a94270403caf212bdd77d5da2f.png)

估计有同学就想到了，采用多个变量存储不就行了吗。对，想的没错。

确实可以采用多个变量进行存储，只不过将来要对这多个变量进行操作就比较麻烦了，

比如说：找到成绩最高的学员。按照我们学过的获取两个数的较大值，需要编写大量的判断逻辑才能完成这个操作。

很明显，采用多个变量存储不是好的解决方案。

那怎么办呢？我们再来回顾一下，目前出现的问题是：

1：一次性声明大量的用于存储数据的变量，

2：要存储的数据通常都是同类型数据，例如：考试成绩。

为了解决这种大量的同类型的数据存储，Java就提供了数组供我们使用。

比如说：下面这种格式，就是定义了一个存储多个考试成绩的数组。

- int\[\] scores = {100,100,100,100,100,100,100…};

对比一下，比定义多个变量要方便多了，而且操作起来也是很方便的，至于怎么操作，一会我们详细讲解。

好了，知道了数组可以解决这种问题后，我们给数组下一个定义：

- \*\*数组(array)：\*\*是一种用于存储 **多个相同数据类型** 的存储模型(可以理解为容器)。

知道了什么是数组后，我们来说一下数组这一节的安排：

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/5f0382923ffd416d8db09ed3d4453235.png)

首先，我们讲解数组的定义格式，这样我们就能够定义数组了。

接着，我们讲解数组的初始化，这样我们就能够给数组中的元素赋值了。

然后，我们讲解数组元素的访问和常见操作，这样我们就能够应用数组解决常见的问题了。

最后，我们讲解数组内存图，这样我们就能够对数组在内存中的存储和操作做到知其然也知其所以然。

好了，到此关于数组的概述和课程安排我们就先讲到这里。

#### 13.2 数组定义和静态初始化

数组有两种定义格式：

- **格式1：** 数据类型\[\] 变量名;
- 范例： int\[\] arr;
- 定义了一个int类型的数组，数组名是arr
- **格式2：** 数据类型 变量名\[\];
- 范例： int arr\[\];
- 定义了一个int类型的变量，变量名是arr数组

这两种格式在使用上是没有区别的，但是在阅读的时候是有一个小区别的？

我们先来看格式1：定义了一个int类型的数组，数组名是arr；再来看格式2：定义了一个int类型的变量，变量名是arr数组

很明显，格式1明确的告诉了我们定义的是一个数组，所以，在定义数组的时候，我们 **推荐使用格式1** 。

现在我们会定义数组了，但是数组中没有数据。而Java中的数组必须先初始化，然后才能使用。

所以，接着，我们来说一下数组的初始化。

- **所谓初始化：** 就是为数组中的数组元素分配内存空间，并为每个数组元素赋值
- 注意：数组中的每一个数据，我们称之为数组中的 **元素**

知道了什么是初始化后，我们来说一下数组中的初始化。

数组的初始化分为两种方式：一种是静态初始化，一种是动态初始化。

它们有各自的使用场景，后面我们会讲解到。

这里我们先讲解数组的静态初始化

- **静态初始化：** 初始化时指定每个数组元素的初始值，由系统决定数组长度
- **格式：** 数据类型\[\] 变量名 = new 数据类型\[\]{数据1,数据2,数据3,…};
- **范例：** int\[\] arr = new int\[\]{1,2,3};

针对这种格式呢？Java提供了一种简化的格式，让我们使用起来更方便

- **简化格式：** 数据类型\[\] 变量名 = {数据1,数据2,数据3,…};
- **范例：** int\[\] arr = {1,2,3};

这样呢，我们就能够定义并初始化一个数组了。

好了，关于数组的定义和静态初始化我们就先讲到这里。

#### 13.3 数组元素访问(获取和修改)

下面我们来学习数组元素访问。

而在数组元素访问这一块，我们要学习两个知识：

1. 一个是数组变量的访问方式
2. 一个是数组内部保存的数据的访问方式

我们先来说，数组变量访问方式

- 它的格式是这样的： **数组名**

我们可以通过输出语句，输出数组名，就能够得到一个数据。那这个数据是什么呢？不着急，一会我们会演示的。

接着，我们来说，数组内部保存的数据的访问方式

- 它的格式是： **数组名\[索引\]**

这个格式没有什么问题，但是这里的索引是什么呢？为了讲解这个索引，我们来看一下这样的一个场景：

在这里有一排人，在这排着队呢，为了知道他们站的位置，给他们进行1,2,3.。。。的编号。

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/bab28e94e206436fb56cbb78e0f38ae7.png)

这里的编号是从1开始的。

而计算机中编号习惯从0开始，这个 **从0开始的编号，我们就称之为索引** 。

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/d006d25758644154a1f1c68ca94fa462.png)

接着，我们来说一下：

- 索引是数组中数据的编号方式
- 作用：用于访问数组中的数据使用，数组名\[索引\]等同于变量名，是一种特殊的变量名
- 它还有这样的几个特征：
	- 特征①：索引从0开始
	- 特征②：索引是连续的
	- 特征③：索引逐一增加，每次加1

知道了如何访问数组变量以及数组中的元素后，下面我们到idea中去演示一下。

```java
/*
    数组变量访问方式
        格式：数组名

    数组内部保存的数据的访问方式
        格式：数组名[索引]
 */
public class ArrayDemo {
    public static void main(String[] args) {
        //定义一个数组，并进行初始化
//        int[] scores = new int[]{93,96,99};
        int[] scores = {93,96,99};

        //输出数组名
        System.out.println(scores); //[I@776ec8df

        //输出数组中的元素
        System.out.println(scores[0]);
        System.out.println(scores[1]);
        System.out.println(scores[2]);
        System.out.println("-----------");

        //修改数组中的元素
        scores[0] = 100;
        scores[1] = 98;
        scores[2] = 95;
        //再次输出数组中的元素
        System.out.println(scores[0]);
        System.out.println(scores[1]);
        System.out.println(scores[2]);
    }
}
1234567891011121314151617181920212223242526272829303132
```

#### 13.4 案例1(数组常见操作之遍历)

下面我们来学习数组常见操作，数组常见操作有很多，这里我们先讲解下面这几个：

- 遍历
- 获取最大值
- 元素打乱

其他的操作，后续我们会进行讲解。

首先，我们来讲解数组遍历，那什么是数组遍历？我们一起来说一下：

- 数组遍历指的是： **获取数组中的每一个元素** ，我们可以把获取到的元素输出在控制台

知道了什么是数组遍历后，我们到IDEA中去实现一下，然后再回来总结。

```java
/*
    遍历
 */
public class ArrayTest01 {
    public static void main(String[] args) {
        //定义数组并初始化
        int[] arr = {77, 88, 99, 66, 55, 44};

        //获取数组中的元素
//        System.out.println(arr[0]);
//        System.out.println(arr[1]);
//        System.out.println(arr[2]);
//        System.out.println(arr[3]);
//        System.out.println(arr[4]);

        //用循环改进
//        for (int i=0; i<5; i++) {
//            System.out.println(arr[i]);
//        }

        //格式：数组名.length
//        System.out.println(arr.length);

        for (int i=0; i<arr.length; i++) {
            System.out.println(arr[i]);
        }
    }
}
12345678910111213141516171819202122232425262728
```

最后，我们回到资料总结一下：

**什么是数组遍历：**

- 获取数组中的每一个元素，我们可以把获取到的元素输出在控制台

**获取数组长度(元素个数)：**

- 格式：数组名.length
- 范例： **arr.length**

**数组遍历 通用格式 ：**

![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/4765cf79a9e54d7387a76890973b8bc3.png)

**注意：** 数组遍历指的是把数组中的元素取出来，取出来之后可以(打印，求和，判断…)

数组遍历通用格式：  
for (int i = 0; i < scores.length; i++) {  
scores\[i\]  
}  
注意：数组遍历指的是把数组中的元素取出来，取出来之后可以(打印，求和，判断…)。  
选择哪种操作，得根据我们的实际需求来看。

好了，关于数组常见操作之遍历我们就先讲到这里

#### 13.5 案例2(数组常见操作之获取最大值)

下面我们来学习数组中获取最大值：

而在讲解具体的实现之前，我们先通过一个场景，让大家对最值有一个认知：

看这里，这是一组家庭成员：

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/5c78cc437f2b4469a4c2ccc580182be4.png)

给出一组数据，这些数据表示的是他们的年龄。68是最大年龄，4是最小年龄，所以，68和4就可以被称之为最值。

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/20dc66cd3ea34010921ac10f783d4125.png)

再给出一组数据，这些数据表示的是他们的身高，171是最高身高，81是最低身高，所以，171和81就可以被称之为最值。

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/1a8a48b62c2347c98919b9039e62fea5.png)

那这里的171为什么就是最高身高呢？

很明显，要想说171是最高身高，我们就要把这些数据从头到尾比较了一遍，最终找到了最高身高171。

而要进行比较，我们的先把这些数据保存起来。这里我们就采用数组把这些数据给保存起来。

知道了大量同类型数据用数组保存和最值的知识后，我们来看一下我们的需求：

- 我这里有一个数组，我现在要获取数组中的最大值

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/393d26275de349e09da9458378a75f3c.png)

如何实现呢？接下来，我们说一下思路：

1：因为我们最终，要得到最大值，所以，这里我们定义一个变量，用于保存最大值。

但是，它没有初始值，给多少比较合适呢？我总不能拿数组以外的数据进来吧，因为我们最终获取的是数组中的最大值。所以，我们就要从数组中找一个值作为初始值。

一般来说，我们取数组中第一个元素作为参照值。

2：这样我们的最大值变量就有初始值了，接下来，我们与数组中剩余的数据逐个比较，比完之后，max中最终保存的是最大值。

这个动作怎么实现呢？我们来说一下：获取索引1-4，为什么不从0开始呢？因为0索引位置的值已经作为初始值了。

3：我们每次比较，需要把最大值保存到max变量中，这个动作，我们可以通过if语句实现。

4：当循环结束后，打印max变量就可以了，这个max里面保存的就是最大值。

说完了数组获取最大值的思路后，我们到idea中去实现一下：

```java
/*
    获取最大值
 */
public class ArrayTest02 {
    public static void main(String[] args) {
        //定义数组
        int[] arr = {12, 45, 98, 73, 60};

        //定义变量max存储最大值，取第一个数据为变量的初始值
        int max = arr[0];

        //与数组中剩余数据逐个比对，每次比对将最大值保存到变量max中
        for (int i=1; i<arr.length; i++) {
            if(arr[i] > max) {
                max = arr[i];
            }
        }

        //循环结束后输出变量max的值
        System.out.println("max:" + max);
    }
}
12345678910111213141516171819202122
```

#### 13.6 案例3(数组常见操作之元素打乱)

下面我们来学习数组中元素打乱。

那什么是元素打乱呢？

- 元素打乱就是把数组中的元素随机交换位置，每次运行都可能产生不一样的结果

比如： **arr** **\= {12, 45, 98, 73, 60};**

**遍历：**

- 正常情况下：12,45,98,73,60
- 元素打乱后：45,73,12,60,98

**涉及到的操作：**

- 获取数组中元素的随机索引
	- Random r = new Random();
	- int index = r.nextInt(arr.length);
- 数组中元素交换

获取随机索引比较好实现，但是元素交换该如何实现呢？

这里为了帮助大家更好的理解，我们给出这样的一个场景来理解数据交换：

把啤酒杯和红酒杯里面的酒进行交换

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/91a3c78156454752ab9420e81dbece20.png)

如何实现呢？

第一步：找来一个同类型的空酒杯

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/557dfee01f204073bce725bf70faed76.png)

第二步：把红酒倒入到空酒杯中

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/7c2bc37a756a49d5a68ff408c0b46395.png)

第三步：把啤酒倒入到曾经装红酒的杯子中

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/8a73ba6a8a00426a82f6ff0a9f962c63.png)

第四步：把红酒从临时找来的杯子中倒入到曾经装啤酒的杯子中

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/2d417a536e7645c8a77843aa9d5e01ee.png)

这样我们就实现了啤酒杯和红酒杯里面的酒进行交换。这种思想同样也适合我们程序中的数据交换。

下面我们到IDEA中去演示一下数据的交换：

```java
/*
    数据交换
 */
public class DataSwap {
    public static void main(String[] args) {
//        int a = 10;
//        int b = 20;
//        System.out.println("交换前：a=" + a + ",b=" + b);
//        int temp = a;
//        a = b;
//        b = temp;
//        System.out.println("交换后：a=" + a + ",b=" + b);

        int[] arr = {11, 22, 33, 44, 55};
        System.out.println("交换前：arr[0]=" + arr[0] + ",arr[4]=" + arr[4]);
        int temp = arr[0];
        arr[0] = arr[4];
        arr[4] = temp;
        System.out.println("交换后：arr[0]=" + arr[0] + ",arr[4]=" + arr[4]);
    }
}
123456789101112131415161718192021
```

数据的交换演示完毕后，下面我们就可以来实现把数组中的元素打乱了：

```java
import java.util.Random;

/*
    元素打乱
 */
public class ArrayTest03 {
    public static void main(String[] args) {
        //定义数组
        int[] arr = {12, 45, 98, 73, 60};

//        Random r = new Random();
//        int index = r.nextInt(arr.length);
//
//        //第一次交换
//        int temp = arr[0];
//        arr[0] = arr[index];
//        arr[index] = temp;
//
//        //第二次交换
//        index = r.nextInt(arr.length);
//        temp = arr[1];
//        arr[1] = arr[index];
//        arr[index] = temp;

        Random r = new Random();
        for (int i = 0; i < arr.length; i++) {
            int index = r.nextInt(arr.length);

            int temp = arr[i];
            arr[i] = arr[index];
            arr[index] = temp;
        }

        //遍历数组
        for (int i = 0; i < arr.length; i++) {
            System.out.println(arr[i]);
        }
    }
}
123456789101112131415161718192021222324252627282930313233343536373839
```

#### 13.7 数组动态初始化

下面我们来学习数组初始化之动态初始化。

前面呢，我们已经学习过了静态初始化，也就是初始化时指定每个数组元素的初始值。

而动态初始化呢？初始化时只指定数组长度，由系统为数组分配初始值

这里我们来看一下动态初始化的格式：

- **格式：** 数据类型\[\] 变量名 = new 数据类型\[数组长度\];
- **范例：** int\[\] arr = new int\[3\];

表示我们定义了一个int类型的数组，初始化为3个元素。

知道了如何对数组进行动态初始化之后，下面我们到IDEA中去使用一下：

```java
/*
    动态初始化：初始化时只指定数组长度，由系统为数组分配初始值
    格式：数据类型[] 变量名 = new 数据类型[数组长度];
    范例：int[] arr = new int[3];
 */
public class ArrayDemo {
    public static void main(String[] args) {
        //格式：数据类型[] 变量名 = new 数据类型[数组长度];
        int[] arr = new int[3];

        //输出数组名
        System.out.println(arr); //[I@776ec8df

        //输出数组中的元素
        System.out.println(arr[0]);
        System.out.println(arr[1]);
        System.out.println(arr[2]);
        System.out.println("------------");

        //修改数组中的元素
        arr[0] = 10;
        arr[1] = 20;
        arr[2] = 30;

        //再次输出数组中的元素
        System.out.println(arr[0]);
        System.out.println(arr[1]);
        System.out.println(arr[2]);
    }
}
123456789101112131415161718192021222324252627282930
```

演示完毕之后，回到资料我们总结一下数组初始化的两种方式的 **各自使用场景：**

- **静态初始化：** 开始就存入元素值，适合一开始就能确定元素值的业务场景
- **动态初始化：** 指定数组长度，后期赋值，适合开始知道数据的数量，但是不确定具体元素值的业务场景
- **注意：** 两种初始化的方式是独立的，不可以混用

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/dffa8b3a3e4741c1af4c3d99ef2a86b8.png)

好了，关于数组初始化之动态初始化我们就先讲到这里。

#### 13.8 案例4(数组元来自键盘录入)

下面我们来做一个案例：数组元素来自键盘录入

首先呢，我们来看一下具体的需求：

- **需求：** 定义一个可以存储5个元素的int数组，数据来自于键盘录入，最后遍历数组，把元素输出在控制台

首先，我们来简单的分析一下：

这个数组可以存储5个int类型的元素，但是数据来自于键盘录入，也就是先指定数组长度，后期赋值。

这很明显适合使用数组的动态初始化，所以，这里我们将采用动态初始化对数组进行初始化。

接着，数据来自于键盘录入，我们得知道这里要使用Scanner来实现。

明确了这两个内容后，下面我们到IDEA中一起去实现一下：

```java
import java.util.Scanner;

/*
    需求：定义一个可以存储5个元素的int数组，数据来自于键盘录入，最后遍历数组，把元素输出在控制台
 */
public class ArrayTest {
    public static void main(String[] args) {
        //定义一个数组，并进行动态初始化
        int[] arr = new int[5];

        //创建键盘录入对象
        Scanner sc = new Scanner(System.in);

//        //录入第1个数据
//        System.out.println("请输入第1个数据：");
        int i = sc.nextInt();
        arr[0] = i;
//        arr[0] = sc.nextInt();
//
//        //录入第2个数据
//        System.out.println("请输入第2个数据：");
//        arr[1] = sc.nextInt();

        for (int i = 0; i < arr.length; i++) {
            System.out.println("请输入第" + (i + 1) + "个元素：");
            arr[i] = sc.nextInt();
        }

        printArray(arr);

            //输出内容并换行
//        System.out.println("hello");
//        System.out.println("world");
            //输出内容不换行
//        System.out.print("hello");
//        System.out.print("world");
    }

    public static void printArray(int[] arr) {
        System.out.print("[");
        for (int i = 0; i < arr.length; i++) {
            if(i==arr.length-1) {
                System.out.print(arr[i]);
            }else {
                System.out.print(arr[i] + ", ");
            }
        }
        System.out.println("]");
    }

    /*
        参数：int[] arr
        返回值：void
     */
//    public static void printArray(int[] arr) {
//        for (int i = 0; i < arr.length; i++) {
//            System.out.println(arr[i]);
//        }
//    }
}
123456789101112131415161718192021222324252627282930313233343536373839404142434445464748495051525354555657585960
```

在讲解过程中，我们讲到了一个新的输出语句，不带ln的方法，它只输出内容，不换行。

而以前我们使用的输出语句，不仅仅把内容输出，而且在输出内容后，会加一个换行。

好了，关于案例数组元素来自键盘录入我们就先讲到这里。

#### 13.9 数组内存图

下面我们来学习数组内存图。

这里呢，我们通过单个数组的内存图让大家了解一下数组在内存中的存储和使用就可以了。

整个过程讲解的是下图代码的执行流程，大家能够听懂即可。

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/610b700dd64449809230715004e43cb6.png)

最后，我们自己编写代码验证一下：

```java
/*
    数组内存图代码
 */
public class ArrayTest01 {
    public static void main(String[] args) {
        int[] arr = new int[3];

        //输出数组名及元素
        System.out.println(arr);
        System.out.println(arr[0]);
        System.out.println(arr[1]);
        System.out.println(arr[2]);

        //给数组中的元素赋值
        arr[0] = 100;
        arr[2] = 200;

        //再次输出数组名及元素
        System.out.println(arr);
        System.out.println(arr[0]);
        System.out.println(arr[1]);
        System.out.println(arr[2]);
    }
}
123456789101112131415161718192021222324
```

由于仅仅是验证讲解的结论，故不需要练习。

#### 13.10 数组使用中的两个小问题

下面我们来讲解一下数组使用中的两个小问题。

先来看第一个问题：请问下列代码有问题吗？如果有，是什么问题？如何解决？

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/0d80b82e4b964d5782107322ea9927ed.png)

通过内存图进行讲解：

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/f0b3bcaf657f43deb69a1e7feb9d9f70.png)

最终结论是：

- 有问题
- 访问了不存在的索引位置元素
- 修改不存在的索引为正确的索引。范围(0~数组长度-1)

再来看第二个问题：请问下列代码有问题吗？如果有，是什么问题？如何解决？

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/17d832ee34b6474ebd01441d5d6a7677.png)

通过内存图进行讲解：

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/1830a54922fb4602bf13b24b0199262a.png)

最终结论是：

- 有问题
- 对象设置为null，不在指向堆内存数据了，还想继续访问堆内存数据
- 对象在使用前，进行不为null的判断

讲解完毕后，到IDEA中再去通过代码验证一下：

```java
/*
    数组使用中的两个小问题
        1：索引越界：访问了数组中不存在的索引对应的元素，造成索引越界问题
            ArrayIndexOutOfBoundsException

        2：空指针异常：对象不再指向堆内存，还想继续访问数据，访问失败
            NullPointerException

        null：空值，引用数据类型的默认值，表示不指向任何有效对象
 */
public class ArrayTest02 {
    public static void main(String[] args) {
        int[] arr = new int[3];
        //输出元素
        //Exception in thread "main" java.lang.ArrayIndexOutOfBoundsException: Index 3 out of bounds for length 3
//        System.out.println(arr[3]);
        System.out.println(arr[2]);

        //把null赋值给arr
        arr = null;
        //输出元素
        //Exception in thread "main" java.lang.NullPointerException: Cannot load from int array because "arr" is null
        if(arr != null) {
            System.out.println(arr[0]);
        }
    }
}
123456789101112131415161718192021222324252627
```

由于仅仅是验证讲解的结论，故不需要练习。

### 14：二维数组

#### 14.1 二维数组概述和课程安排

下面我们来学习二维数组。前面我们讲解的数组，一般称之为一维数组。

为了帮助大家理解二维数组呢？这里我们来看这样的一个场景：

需求：我们要存储多个班级的学生的考试成绩，该怎么办呢？

如果要存储一个班级中多个学生的考试成绩，我们就可以采用数组来存储。

现在的问题是？多个班级的考试成绩，我们针对每个班级都采用数组存储。

第一个班级：数组1

第二个班级：数组2

第三个班级：数组3  
…

但是多个班级，也可以采用数组存储啊。所以，Java就提供了二维数组供我们使用。

这里我们给二维数组一个简单的定义：

- **二维数组：** 元素为一维数组的数组

知道了什么是二维数组后，我们再说一下二维数组的定义格式：

它有这样的三个格式，用\[\]\[\]表示二维数组：

1. 数据类型\[\] \[\] 变量名; int\[\] \[\] arr; **推荐**
2. 数据类型 变量名\[\] \[\]; int arr\[\] \[\];
3. 数据类型\[\] 变量名\[\]; int\[\] arr\[\];

推荐使用第一种格式。

知道了什么是二维数组以及二维数组的定义格式后，我们来说一下二维数组安排：

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/d3a034a6f2f94e679376dcea5b4f34e6.png)

首先，我们讲解二维数组初始化，这样我们就能够给二维数组中的元素赋值了。

接着，我们讲解二维数组元素访问，这样我们就能够获取到二维数组中的数据了。

然后，我们讲解二维数组内存图，这样我们就能够对二维数组在内存中的存储和操作做到知其然也知其所以然。

最后，我们讲解二维数组常见操作，这样我们就能够应用二维数组解决常见的问题了。

好了，到此关于二维数组的概述和课程安排我们就先讲到这里。

#### 14.2 二维数组初始化

下面我们来学习二维数组初始化，和一维数组一样，二维数组初始化也有两种格式：

1. 静态初始化
2. 动态初始化

首先来看 **静态初始化：**

- **格式：** 数据类型\[\] \[\] 变量名 = new 数据类型\[\] \[\]{{元素…},{元素…},{元素…},…};
- **范例：** int\[\] \[\] arr = new int\[\] \[\]{{1,2,3},{4,5,6},{7,8,9}};

**解读：**

- 定义了一个二维数组
- 二维数组中有三个元素(一维数组)
- 每一个一维数组有三个元素(int类型数据)
- 注意：一维数组中元素的个位可以是不同的
- 比如： int\[\] \[\] arr = new int\[\] \[\]{{1,2,3},{4,5},{6,7,8,9}};

同样，针对静态初始化，二维数组也给出了简化格式：

- **简化格式：** 数据类型\[\]\[\] 变量名 = {{元素…},{元素…},{元素…},…};
- **范例：** int\[\] \[\] arr = {{1,2,3},{4,5,6},{7,8,9}};

再来看 **动态初始化：**

- **格式：** 数据类型\[\] \[\] 变量名 = new 数据类型\[m\] \[n\];
- **范例：** int\[\] \[\] arr = new int\[2\] \[3\];

**解读：**

- 定义了一个二维数组
- 二维数组中有2个元素(一维数组)
- 每一个一维数组有3个元素(int类型数据)

他们的各自使用场景和一维数组中讲解的是一样的：

静态初始化：适合一开始就能确定元素值的业务场景

动态初始化：适合开始知道数据的数量，但是不确定具体元素值的业务场景

好了，关于二维数组的初始化我们就先讲到这里

#### 14.3 二维数组元素访问

下面我们来学习二维数组元素访问。

关于二维数组的元素访问，我们先到idea中去讲解，然后再回来总结：

```java
/*
    静态初始化简化格式：数据类型[][] 数组名 = {{元素...},{元素...},{元素...},...};
 */
public class ArrayDemo {
    public static void main(String[] args) {
        //静态初始化简化格式：数据类型[][] 数组名 = {{元素...},{元素...},{元素...},...};
        int[][] arr = {{1, 2, 3}, {4, 5, 6}};

        //输出数组名
        System.out.println(arr); //[[I@776ec8df

        System.out.println(arr[0]); //[I@4eec7777
        System.out.println(arr[1]); //[I@3b07d329

        //如何获取到数据1,2,3呢？
        System.out.println(arr[0][0]);
        System.out.println(arr[0][1]);
        System.out.println(arr[0][2]);
    }
}
1234567891011121314151617181920
```

讲解完毕后，回到资料总结一下：

- 获取二维数组： **数组名**
- 获取每一个一维数组： **数组名\[索引\]**
- 获取每一个二维数组元素： **数组名\[索引\] \[索引\]**

好了，关于二维数组的元素访问我们就先讲到这里。

#### 14.4 二维数组内存图

下面我们来学习二维数组的内存图。

这里呢，我们通过内存图的方式让大家了解一下二维数组在内存中的存储和使用就可以了。

整个过程讲解的是下图代码的执行流程，大家能够听懂即可。

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/48c54fac642045bd816dbb1cf9ffe9eb.png)

最后，我们自己编写代码验证一下：

```java
/*
    二维数组内存图代码
 */
public class ArrayTest {
    public static void main(String[] args) {
        //定义二维数组
        int[][] arr = {{1, 2, 3}, {4, 5, 6}};

        //输出数组中的元素
        System.out.println(arr[0][1]);
        System.out.println(arr[1][1]);

        //修改数组中的元素
        arr[0][1] = 10;
        arr[1][1] = 20;

        //再次输出数组中的元素
        System.out.println(arr[0][1]);
        System.out.println(arr[1][1]);
    }
}
123456789101112131415161718192021
```

由于仅仅是验证讲解的结论，故不需要练习。

#### 14.5 案例5(二维数组常见操作之遍历)

下面我们来学习二维数组常见操作：

这里我们讲解两个操作：

- 遍历
- 元素打乱

首先，我们来看二维数组遍历。

这里有一个需求：已知一个二维数组 arr = {{1,2,3},{4,5,6},{7,8,9}}; 请把元素在控制台输出。

看完需求之后，我们到IDEA中一起去实现一下，然后再回来总结：

```java
/*
    需求：已知一个二维数组 arr = {{1,2,3},{4,5,6},{7,8,9}}; 请把元素在控制台输出
 */
public class ArrayTest01 {
    public static void main(String[] args) {
        //定义二维数组，并进行静态初始化
        int[][] arr = {{1, 2, 3}, {4, 5, 6}, {7, 8, 9}};

        //获取数据1,2,3
//        System.out.println(arr[0][0]);
//        System.out.println(arr[0][1]);
//        System.out.println(arr[0][2]);
//        for (int i = 0; i < arr[0].length; i++) {
//            System.out.println(arr[0][i]);
//        }
//
//        //获取数据4,5,6
        System.out.println(arr[1][0]);
        System.out.println(arr[1][1]);
        System.out.println(arr[1][2]);
//        for (int i = 0; i < arr[1].length; i++) {
//            System.out.println(arr[1][i]);
//        }
//
//        //获取数据7,8,9
        System.out.println(arr[2][0]);
        System.out.println(arr[2][1]);
        System.out.println(arr[2][2]);
//        for (int i = 0; i < arr[2].length; i++) {
//            System.out.println(arr[2][i]);
//        }

        for (int i = 0; i < arr.length; i++) {
            //arr[i]
            for (int j = 0; j < arr[i].length; j++) {
                System.out.print(arr[i][j]+" ");
            }
            System.out.println();
        }
    }
}
1234567891011121314151617181920212223242526272829303132333435363738394041
```

在代码讲解过程中，我们讲解了循环嵌套：for循环的语句体是循环语句，这种现象被称为循环嵌套。

讲解完毕后，回到资料中我们去总结一下：

在实现的过程中，我们在二维数组中使用了循环嵌套：

① 循环嵌套：循环语句中嵌套循环语句

② 通过外层循环可以得到一维数组

③ 在通过内存循环可以得到每一个二维数组元素

好了，关于二维数组常见操作之遍历我们就先讲到这里。

#### 14.6 案例6(二维数组常见操作之元素打乱)

下面我们来学习二维数组中元素打乱。

在前面呢，我们讲解过一维数组中的元素打乱，这里的思路和前面是一样的，也是要随机产生二维数组中元素的索引，并进行元素交换。

只不过呢，二维数组元素的索引是两个值，所以，这里要产生两个随机数。

知道了二维数组元素打乱的基本思路后，下面我们到IDEA中去实现一下：

```java
import java.util.Random;

/*
    需求：已知二维数组 arr = {{1,2,3},{4,5,6},{7,8,9}};用程序实现把数组中的元素打乱,并在控制台输出打乱后的数组元素
 */
public class ArrayTest02 {
    public static void main(String[] args) {
        //定义二维数组，并进行静态初始化
        int[][] arr = {{1, 2, 3}, {4, 5, 6}, {7, 8, 9}};

        //创建随机数对象
        Random r = new Random();

        //遍历二维数组，进行元素打乱
        for (int i = 0; i < arr.length; i++) {
            for (int j = 0; j < arr[i].length; j++) {
                //arr[i][j]
                int x = r.nextInt(arr.length);
                int y = r.nextInt(arr[x].length);

                //元素交换
                int temp = arr[i][j];
                arr[i][j] = arr[x][y];
                arr[x][y] = temp;
            }
        }

        for (int i = 0; i < arr.length; i++) {
            for (int j = 0; j < arr[i].length; j++) {
                System.out.print(arr[i][j] + " ");
            }
            System.out.println();
        }
    }
}
1234567891011121314151617181920212223242526272829303132333435
```

好了，关于二维数组常见操作之元素打乱我们就先讲到这里

#### 14.7 案例7(图片展示)

下面我们来做一个案例图片展示。

关于图片展示呢？前面我们是学习过的，通过JLable组件就可以实现图片展示了。

看一下，我们这里的需求，我有很多小的图片，它们拼在一起就成了这样的一张美女美图。

外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传

下面我们要做的事情就是把这些图片一张张的给展示出来。

这里的窗体我们已经准备好了，我们要做的事情就是在窗体上显示这些图片。

下面我们到IDEA中去实现一下：

图片素材在今天的资料里面，复制到当前的模块目录下。

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/63ea3647e87f4aa9942a6b8db93538dd.png)

```java
import javax.swing.*;

/*
    图片展示
 */
public class ArrayTest03 {
    public static void main(String[] args) {
        //创建窗体对象
        JFrame jf = new JFrame();

        jf.setTitle("图片展示");
        jf.setSize(380, 400);
        jf.setDefaultCloseOperation(3);
        jf.setLocationRelativeTo(null);
        jf.setAlwaysOnTop(true);
        jf.setLayout(null);

//        JLabel jLabel1 = new JLabel(new ImageIcon("itheima-array2\\images\\1.png"));
//        jLabel1.setBounds(0, 0, 90, 90);
//        jf.add(jLabel1);
//
//        JLabel jLabel2 = new JLabel(new ImageIcon("itheima-array2\\images\\2.png"));
//        jLabel2.setBounds(90, 0, 90, 90);
//        jf.add(jLabel2);
//
//        JLabel jLabel3 = new JLabel(new ImageIcon("itheima-array2\\images\\3.png"));
//        jLabel3.setBounds(180, 0, 90, 90);
//        jf.add(jLabel3);
//
//        JLabel jLabel4 = new JLabel(new ImageIcon("itheima-array2\\images\\4.png"));
//        jLabel4.setBounds(270, 0, 90, 90);
//        jf.add(jLabel4);

//        for (int i=0; i<4; i++) {
//            JLabel jLabel = new JLabel(new ImageIcon("itheima-array2\\images\\"+(i+1)+".png"));
//            jLabel.setBounds(i*90,0,90,90);
//            jf.add(jLabel);
//        }
//
        JLabel jLabel5 = new JLabel(new ImageIcon("itheima-array2\\images\\5.png"));
        jLabel5.setBounds(0, 90, 90, 90);
        jf.add(jLabel5);

        JLabel jLabel6 = new JLabel(new ImageIcon("itheima-array2\\images\\6.png"));
        jLabel6.setBounds(90, 90, 90, 90);
        jf.add(jLabel6);

        JLabel jLabel7 = new JLabel(new ImageIcon("itheima-array2\\images\\7.png"));
        jLabel7.setBounds(180, 90, 90, 90);
        jf.add(jLabel7);

        JLabel jLabel8 = new JLabel(new ImageIcon("itheima-array2\\images\\8.png"));
        jLabel8.setBounds(270, 90, 90, 90);
        jf.add(jLabel8);
//        for (int i=0; i<4; i++) {
//            JLabel jLabel = new JLabel(new ImageIcon("itheima-array2\\images\\"+(i+5)+".png"));
//            jLabel.setBounds(i*90,90,90,90);
//            jf.add(jLabel);
//        }
//
        JLabel jLabel9 = new JLabel(new ImageIcon("itheima-array2\\images\\9.png"));
        jLabel9.setBounds(0, 180, 90, 90);
        jf.add(jLabel9);

        JLabel jLabel10 = new JLabel(new ImageIcon("itheima-array2\\images\\10.png"));
        jLabel10.setBounds(90, 180, 90, 90);
        jf.add(jLabel10);

        JLabel jLabel11 = new JLabel(new ImageIcon("itheima-array2\\images\\11.png"));
        jLabel11.setBounds(180, 180, 90, 90);
        jf.add(jLabel11);

        JLabel jLabel12 = new JLabel(new ImageIcon("itheima-array2\\images\\12.png"));
        jLabel12.setBounds(270, 180, 90, 90);
        jf.add(jLabel12);
//        for (int i=0; i<4; i++) {
//            JLabel jLabel = new JLabel(new ImageIcon("itheima-array2\\images\\"+(i+9)+".png"));
//            jLabel.setBounds(i*90,180,90,90);
//            jf.add(jLabel);
//        }
//
        JLabel jLabel13 = new JLabel(new ImageIcon("itheima-array2\\images\\13.png"));
        jLabel13.setBounds(0, 270, 90, 90);
        jf.add(jLabel13);

        JLabel jLabel14 = new JLabel(new ImageIcon("itheima-array2\\images\\14.png"));
        jLabel14.setBounds(90, 270, 90, 90);
        jf.add(jLabel14);

        JLabel jLabel15 = new JLabel(new ImageIcon("itheima-array2\\images\\15.png"));
        jLabel15.setBounds(180, 270, 90, 90);
        jf.add(jLabel15);

        JLabel jLabel16 = new JLabel(new ImageIcon("itheima-array2\\images\\16.png"));
        jLabel16.setBounds(270, 270, 90, 90);
        jf.add(jLabel16);
//        for (int i=0; i<4; i++) {
//            JLabel jLabel = new JLabel(new ImageIcon("itheima-array2\\images\\"+(i+13)+".png"));
//            jLabel.setBounds(i*90,270,90,90);
//            jf.add(jLabel);
//        }

        //定义图片编号的数组
        int[][] datas = {
                {1,2,3,4},
                {5,6,7,8},
                {9,10,11,12},
                {13,14,15,16}
        };

        for (int i = 0; i < datas.length; i++) {
            for (int j = 0; j < datas[i].length; j++) {
                //datas[i][j]
                JLabel jLabel = new JLabel(new ImageIcon("itheima-array2\\images\\"+datas[i][j]+".png"));
                jLabel.setBounds(j*90,i*90,90,90);
                jf.add(jLabel);
            }
        }

        jf.setVisible(true);
    }
}
123456789101112131415161718192021222324252627282930313233343536373839404142434445464748495051525354555657585960616263646566676869707172737475767778798081828384858687888990919293949596979899100101102103104105106107108109110111112113114115116117118119120121122
```

在代码的讲解过程中，我们先一张张的展示图片，后面通过二维数组的方式改进了图片的存储，最终优化了图片展示。

好了，关于案例图片展示我们就先讲到这里

#### 14.8 案例8(图片打乱)

下面我们来做一个案例图片打乱。

刚才我们讲解了图片展示的案例，现在呢，要在图片展示的基础上，把图片打乱，我们可以看一下打乱后的效果，其实就是对二维数组中的图片的编号打乱，然后再显示出来就可以了。

下面呢，我们到IDEA中一起去实现一下：

```java
import javax.swing.*;
import java.util.Random;

/*
    图片打乱
 */
public class ArrayTest04 {
    public static void main(String[] args) {
        //创建窗体对象
        JFrame jf = new JFrame();

        jf.setTitle("图片打乱");
        jf.setSize(380, 400);
        jf.setDefaultCloseOperation(3);
        jf.setLocationRelativeTo(null);
        jf.setAlwaysOnTop(true);
        jf.setLayout(null);

        //图片打乱
        int[][] datas = {
                {1,2,3,4},
                {5,6,7,8},
                {9,10,11,12},
                {13,14,15,16}
        };

        Random r = new Random();
        for (int i = 0; i < datas.length; i++) {
            for (int j = 0; j < datas[i].length; j++) {
                int x = r.nextInt(datas.length);
                int y = r.nextInt(datas[x].length);

                int temp = datas[i][j];
                datas[i][j] = datas[x][y];
                datas[x][y] = temp;
            }
        }

        for (int i = 0; i < datas.length; i++) {
            for (int j = 0; j < datas[i].length; j++) {
                JLabel jLabel = new JLabel(new ImageIcon("itheima-array2\\images\\"+datas[i][j]+".png"));
                jLabel.setBounds(j*90,i*90,90,90);
                jf.add(jLabel);
            }
        }

        jf.setVisible(true);
    }
}
12345678910111213141516171819202122232425262728293031323334353637383940414243444546474849
```

## 七、常用API(1)

**本节目标：**

- 能够知道什么是API
- 能够使用帮助文档学习API
- 能够理解包和导包
- 能够知道Scanner的作用和基本使用
- 能够知道Random的作用和基本使用
- 能够知道GUI的作用和基本使用
- 能够完成GUI相关的授课案例
- 能够理解事件监听机制
- 能够对按钮添加事件

### 15：API 概述

#### 15.1 API概述和课程安排

我们在讲解面向对象的时候，提到了学习面向对象重点就是学习两块内容：

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/3b8c59ce5b2d473d845cac6607000e1b.png)

第一块：学习如何自己设计对象并使用

第二块：学习获取已有对象并使用

而关于第一块知识：学习如何自己设计对象并使用，我们现在已经有一些基础了。

通过前面的学习呢，我们知道了如何定义类，并通过构造方法创建对象，然后通过对象使用成员变量和成员方法。

接下来，我们要学习的是第二块知识：获取已有对象并使用。而获取已有对象并使用呢，在Java中我们习惯称之为常用API的学习。

所以下面我们来学习常用API。首先，我们来说一下什么是API：

- **API(Application Programming Interface)** ：应用程序编程接口

那如何理解应用程序编程接口呢？这里我们通过下面的场景给大家解释一下。

看这里，我想编写一个机器人踢足球的程序，那么程序就要向机器人发出向前跑、向后跑、射门、抢球等各种命令。

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/59bb4cafb72e45e498ae947db06db3f4.png)

如果我自己来编写呢，就会比较麻烦，因为机器人不是我设计的。所以，为了方便其他的开发者使用机器人，

机器人厂商呢就会提供一些用于控制机器人的类，这些类中会定义好操作机器人各种动作的方法。

有了这些类之后，开发一个机器人踢足球的程序就会非常的方便了。

其实，这些类就是机器人厂商提供给开发者的应用程序编程接口，而这些类我们称之为：API

知道了什么是API之后呢，我们来说一下，Java的API。

- **Java API** ：指的就是 JDK 中提供的各种功能的 Java类。

这些类将底层的实现封装了起来，我们不需要关心这些类是如何实现的，只需要学习这些类如何使用即可，

为了帮助我们使用这些类，Java还提供了对应的帮助文档。我们可以通过帮助文档来学习这些API如何使用

下面呢，我们一起来学习一下 **帮助文档的使用** ：

要想使用帮助文档，首先我们得有一个帮助文档：来，打开课程资料下面，我们这里有一个帮助文档。

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/e89aa38fbf34408c86214caef7f946e1.png)

这个文档对应的是JDK11版本的，是目前比较新的中文版的帮助文档。

有了文档之后呢，我们来打开帮助文档。

文档打开后，找到索引这里，下面有一个输入框，在这个框框里输入我们要学习的API。

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/51b217b033e74808aa5609a9a410c601.png)

这里，我们拿字符串类做一个说明：在这个框框里面我们输入：String，然后一回车，看到一个新的界面

这个界面中，就是关于String相关的知识了。

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/3cb980a8dc81476098b0458367f6106b.png)

接着，我们来说一下，在学习一个API的时候， **我们重点要看四个地方：**

**第一个地方：看类所在的包**

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/a2ed5ecdffc34420a87521145659a62b.png)

为什么要看这里呢，因为java.lang包下的类，我们是可以直接使用的，不需要导包。

其他包下的类，我们都是要导包后才能使用的，至于如何导包，下个知识我们会讲解。

很明显，String类在使用的时候，我们是不需要导包的。

**第二个地方：看类的描述**

也就是看这里，这里一般描述了类是干什么的。

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/7b924f49cf1445c5b8c043704fee9b3b.png)

比如说：String类表示字符串。 Java程序中的所有字符串文字（例如"abc" ）都实现为此类的实例。

告诉了我们String就是用来表示字符串的类，直接写一个字符串数据：abc就是String类的一个对象。

**第三个地方：看类的构造方法**

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/57dcf7c582b041b882a353e43c10eb01.png)

往下滑，这就是String类的构造方法，为什么要看构造方法呢？因为我们在使用一个类的时候，其实使用的是该类的对象，

而创建对象，我们是需要通过构造方法实现的，所以，我们得看看它提供了哪些构造方法。

这里的构造方法提供的比较多，至于用哪个，后面我们用到的时候再讲解，目前知道看哪里就行了

**第四个地方：看类的成员方法**

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/34091b5cdb424b0c99aeca7d99a40fc3.png)

这是我们学习一个API的重点，我们之所以学习一个API，重点就是为了使用该API来完成某些功能。

而API的功能，都是通过一个个方法实现的，所以我们重点得看看类的成员方法。往下滑，这就是String提供的成员方法，有很多。

而一个方法，我们重点又看什么呢？回到第一个方法，我们说一下：

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/106a4ac7c9be45c49db749a009d85a0f.png)

先看描述，通过描述，我们就知道了方法是干什么的。

再看方法名和参数，这样我们就知道调用哪个方法，以及参数的类型和个数。

最后，我们看返回值类型，这样我们就知道调用该方法后，最终给我们返回了一个什么类型结果

通过这些步骤，我们就知道了所学习的API该如何使用了，然后就可以到IDEA中去使用API了。

知道了帮助文档的使用步骤后，回到资料我们总结一下 **帮助文档的使用流程：**

① 打开帮助文档

② 找到索引选项，输入要学习的API，然后回车

③ 看类所在包：因为java.lang包下的类在使用的时候不需要导包

④ 看类的描述：这样我们就知道了类是干什么的

⑤ 看类的构造方法：这样我们就可以创建对象了

⑥ 看类的成员方法：这样我们就可以通过这些方法完成某些功能了

知道了什么是API，以及通过帮助文档如何学习API后，我们来说一下常用API这部分的安排：

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/3f8d078fd03748f2add3703e643a196b.png)

首先，我们学习一下包和导包的基本概念和操作，为API的使用做一个基础铺垫

接着我们来学习两个API：Scanner和Random

Scanner：是用来实现键盘录入数据的

Random：是用来产生随机数的

通过这两个API的学习，可以让我们熟悉帮助文档的使用

再接着我们来学习GUI相关的API，这里不是一个API的学习，而是多个API的学习，通过这部分内容的学习，可以让我们的操作可视化，也就是有界面了，不在仅仅是在控制台输出数据了。

最后，我们学习这几个API，学习这几个API的目的，是为了完成我们在GUI部分未完成的案例。

好了，到此关于API概述和常用API的课程安排我们就先讲到这里

#### 15.2 包和导包

下面我们来学习一下，包和导包。

那什么是包呢？

- 包其实就是文件夹
- 作用：对类进行分类管理

**包的定义格式：**

- 格式：package 包名;
- 注意：包名一般是公司域名反写，并且多级包用.分开
- 举例：www.itheima.com
- 范例：package com.itheima;

知道了如何定义包之后，下面我们来定义两个包，并且在不同包下定义同名的类。

```java
package com.itheima_01;

public class Student {
    public void study() {
        System.out.println("好好学习天天向上");
    }
}
1234567
```
```java
package com.itheima_01;

public class StudentTest {
    public static void main(String[] args) {
        Student s = new Student();
        s.study();
    }
}
123456789
```
```java
package com.itheima_02;

public class StudentTest {
    public static void main(String[] args) {
        com.itheima_01.Student s = new com.itheima_01.Student();
        s.study();

        com.itheima_01.Student s2 = new com.itheima_01.Student();
        s2.study();
    }
}
1234567891011
```

在这里我们讲解了同一个包下类的使用，以及不同包下类的使用。发现不同包下类的使用太麻烦了，所以，这个时候，我们就要学习一下导包了。

使用不同包下的类时，使用的时候要写类的全路径，写起来太麻烦了。

为了简化带包的操作，Java就提供了导包的功能。

**导包的格式：**

- 格式：import 包名;
- 范例：import com.itheima.Student;

知道了如何导包后，我们再来修改一下不同包下类的使用代码：

```java
package com.itheima_02;

import com.itheima_01.Student;
//Alt+Enter 快捷键导包

public class StudentTest {
    public static void main(String[] args) {
        Student s = new Student();
        s.study();

        Student s2 = new Student();
        s2.study();

//        com.itheima_01.Student s = new com.itheima_01.Student();
//        s.study();
//
//        com.itheima_01.Student s2 = new com.itheima_01.Student();
//        s2.study();
    }
}
123456789101112131415161718192021
```

在这里我们讲解了导包的三种方式：

1. 手动导包
2. 快捷键导包
3. 写一个类，写一部分的时候，如果给出了对应的提示，回车后会自动导包

### 16：Scanner

#### 16.1 Scanner基本使用

了解了API相关的知识后，下面我们来学习一下Scanner的使用。

通过查看帮助文档，我们知道了如下的信息：

**Scanner：**

- 一个简单的文本扫描程序，可以获取基本类型数据和字符串数据

**构造方法：**

- Scanner(InputStream source)：创建 Scanner 对象
- System.in：对应的是InputStream类型，可以表示键盘输入
- Scanner sc = new Scanner(System.in);

**成员方法：**

- int nextInt()：获取一个int类型的数据
- int i = sc.nextInt();

知道了Scanner的构造方法和成员方法后，我们到IDEA中去使用一下：

```java
import java.util.Scanner;

/*
    Scanner的基本使用
 */
public class ScannerDemo {
    public static void main(String[] args) {
        //Scanner(InputStream source)：创建 Scanner 对象
        Scanner sc = new Scanner(System.in);

        //int nextInt()：获取一个int类型的数据
        System.out.println("请输入一个整数：");
        int i = sc.nextInt();

        //输出获取到的数据
        System.out.println("你输入的数据是：" + i);
    }
}
123456789101112131415161718
```

#### 16.2 练习(数据求和)

需求：键盘录入两个整数，求两个数据和，并在控制台输出求和结果

首先，我们来简单的分析一下：

**分析：**

① 创建键盘录入数据对象

② 通过键盘录入数据对象调用nextInt()方法获取数据

③ 对获取的两个整数求和

④ 在控制台输出求和结果

分析完毕后，我们到IDEA中去实现一下：

```java
/*
    需求：键盘录入两个整数，求两个数据和，并在控制台输出求和结果
    分析：
        1:创建键盘录入数据对象
        2:通过键盘录入数据对象调用nextInt()方法获取数据
        3:对获取的两个整数求和
        4:在控制台输出求和结果
 */
public class ScannerTest {
    public static void main(String[] args) {
        //创建键盘录入数据对象
        Scanner sc = new Scanner(System.in);

        //通过键盘录入数据对象调用nextInt()方法获取数据
        System.out.println("请输入第一个整数：");
        int firstNumber = sc.nextInt();

        System.out.println("请输入第二个整数：");
        int secondNumber = sc.nextInt();

        //对获取的两个整数求和
        int sum = firstNumber + secondNumber;

        //在控制台输出求和结果
        System.out.println("求和结果是：" + sum);
    }
}
123456789101112131415161718192021222324252627
```

### 17：Random

#### 17.1 Random基本使用

下面我们来学习一下Random的使用。

通过查看帮助文档，我们知道了如下的信息：

**Random：**

- 该类的实例用于生成随机数

**构造方法：**

- Random()：创建一个新的随机数生成器

**成员方法：**

- int nextInt(int bound)：获取一个int类型的随机数，参数bound表示获取到的随机数在\[0,bound)之间

知道了Random的构造方法和成员方法后，我们到IDEA中去使用一下：

```java
import java.util.Random;

/*
    Random的基本使用
 */
public class RandomDemo {
    public static void main(String[] args) {
        //Random()：创建一个新的随机数生成器
        Random r = new Random();

        //int nextInt(int bound)：获取一个int类型的随机数，参数bound表示获取到的随机数在[0,bound)之间
//        int i = r.nextInt(10);
//        System.out.println(i);

//        for (int i=1; i<=10; i++) {
//            int j = r.nextInt(10);
//            System.out.println(j);
//        }

        //需求：如何获取1-100之间的随机数呢？
//        int number = r.nextInt(100);//0-99
//        int number = r.nextInt(101);//0-100
        int number = r.nextInt(100) + 1;
        System.out.println(number);
    }
}
1234567891011121314151617181920212223242526
```

#### 17.2 练习(猜数字游戏)

需求：系统自动产生一个1-100之间的整数，使用程序实现猜这个数字是多少？

```java
猜的时候根据不同情况给出相应的提示

如果猜的数字比真实数字大，提示你猜的数据大了

如果猜的数字比真实数字小，提示你猜的数据小了

如果猜的数字与真实数字相等，提示恭喜你猜中了
1234567
```

首先，我们来简单的分析一下：

**分析：**

① 使用Random获取一个1-100之间的整数

② 使用Scanner实现键盘录入猜的数据值

③ 使用if…else if…else 的格式实现猜数字，并给出对应的提示

分析完毕后，我们到IDEA中去实现一下：

```java
import java.util.Random;
import java.util.Scanner;

/*
    需求：系统自动产生一个1-100之间的整数，使用程序实现猜这个数字是多少？
        猜的时候根据不同情况给出相应的提示
        如果猜的数字比真实数字大，提示你猜的数据大了
        如果猜的数字比真实数字小，提示你猜的数据小了
        如果猜的数字与真实数字相等，提示恭喜你猜中了
    分析：
        1:使用Random获取一个1-100之间的整数
        2:使用Scanner实现键盘录入猜的数据值
        3:使用if…else if…else 的格式实现猜数字，并给出对应的提示
 */
public class RandomTest {
    public static void main(String[] args) {
        //使用Random获取一个1-100之间的整数
        Random r = new Random();
        int number = r.nextInt(100) + 1;
        System.out.println("系统已经产生了一个1-100之间的整数");

        while (true) {
            //使用Scanner实现键盘录入猜的数据值
            Scanner sc = new Scanner(System.in);
            System.out.println("请输入你要猜的数字：");
            int guessNumber = sc.nextInt();

            //使用if…else if…else 的格式实现猜数字，并给出对应的提示
            if (guessNumber > number) {
                System.out.println("你猜的数据" + guessNumber + "大了");
            } else if (guessNumber < number) {
                System.out.println("你猜的数据" + guessNumber + "小了");
            } else {
                System.out.println("恭喜你猜中了");
                break;
            }
        }
    }
}
123456789101112131415161718192021222324252627282930313233343536373839
```

### 18：GUI

#### 18.1 GUI概述

下面呢我们来学习GUI相关的API。

首先呢，我们来说一下，什么是GUI：

- **GUI：** Graphical User Interface(图形用户接口)
- 用图形的方式，来显示计算机操作的界面

怎么理解呢？我们把后面要做的案例拿来举例说明一下：

看这里：

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/a67b7e113310485cb531e5faa2c9c8c1.png)

这是用户登录的案例，在这个界面上，有显示文本的标签，显示输入内容的文本框以及按钮。

再来看一个：

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/010f84b4f3d440ee936dfd07d4dc2d9e.png)

聊天室的案例，在这个界面上，有显示聊天内容的文本域，显示输入内容的文本框以及操作的按钮。

给出这样的界面，我们自己就能够看明白，非常的方便直观，这就是使用GUI相关的API来实现的。

而Java为GUI提供的API都存在java.awt和javax.Swing两个包中，我们分别来看一下这两个包：

- **java.awt 包：**
	- awt是这三个单词首字母的缩写，翻译过来是抽象窗口工具包，只不过这个包的API，需要调用本地系统方法实现功能，和本地系统有关联，不利于代码移植，属重量级控件
- **javax.swing 包：**
	- 它是在awt的基础上，建立的一套图形界面系统，提供了更多的组件，而且完全由Java实现。增强了移植性，属轻量级控件

所以，我们做图形界面开发使用的是swing包下的类。

这里出现了一个名词：组件。那什么是组件呢？

- **组件** 是具有图形表示的对象，该图形表示可以显示在屏幕上并且可以与用户交互

比如说，在用户登录中，文本框和按钮等，都是能够表示图形的对象，所以它们都称为组件。

最后，我们来说一下，我们会用到的常用组件，

看这里：

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/674182f45d4040ddbf5c8844a908d330.png)

**组件：**

- **基本组件：** 具有图形表示的对象
- **容器组件：** 是可以添加组件的组件。也就是在容器中可以通过add方法添加组件，既可以添加基本组件，也可以添加容器组件。

我们先来看常用的基本组件：

- JButton，这是按钮
- JLabel，这是用来显示文本内容的，或者展示图片使用
- JTextFile，这是文本框，用来输入内容的
- JTextArea，这是文本域，用来输入多行多列的数据的

接着，我们再来看容器组件：

- 面板也是一个容器，我们常用JPanel，后面用到在具体讲解
- 窗体，下面是Frame，这是awt包下，而我们使用的是JFrame，这是swing包下。

看到这里，我要说一下，由于我们使用的都是swing包下的，所以将来使用的组件，都是以J开头的。

好了，GUI相关的基础知识我们就先讲到这里

#### 18.2 常用组件

##### 18.2.1 JFrame(初识窗体)

下面我们来学习JFrame窗体类。

在学习JFrame之前，先说一下，在学习GUI相关的API的时候，我就不带着大家到帮助文档中查看了。

在资料中，我们会把要讲解的类的作用，构造方法，和成员方法给大家展示出来，简单的分析后，到IDEA中去实现。

首先，我们来看一下JFrame：

**JFrame：**

- 是一个顶层窗口

**构造方法：**

- JFrame()：构造一个最初不可见的新窗体

**成员方法：**

- void setVisible(boolean b)：显示或隐藏此窗体具体取决于参数b的值
- void setSize(int width, int height)：调整此组件的大小，使其宽度为width，高度为height，单位是像素

知道了JFrame的构造方法和成员方法后，我们到IDEA中去使用一下：

```java
import javax.swing.*;

/*
    构造方法
        JFrame()：构造一个最初不可见的新窗体

    成员方法
        void setVisible(boolean b)：显示或隐藏此窗体具体取决于参数b的值
        void setSize(int width, int height)：调整此组件的大小，使其宽度为width，高度为height，单位是像素
 */
public class JFrameDemo01 {
    public static void main(String[] args) {
        //JFrame()：构造一个最初不可见的新窗体
        JFrame jf = new JFrame();

        //void setSize(int width, int height)：调整此组件的大小，使其宽度为width，高度为height，单位是像素
        jf.setSize(400,300);

        //void setVisible(boolean b)：显示或隐藏此窗体具体取决于参数b的值
        jf.setVisible(true);
    }
}
12345678910111213141516171819202122
```

##### 18.2.2 JFrame(常用设置)

下面呢，我们再来学习几个JFrame窗体的常用方法：

- void setTitle(String title)：设置窗体标题
- void setLocationRelativeTo(Component c)：设置位置，值为null，则窗体位于屏幕中央
- void setDefaultCloseOperation(int operation)：设置窗体关闭时默认操作
	- 整数3表示：窗口关闭时退出应用程序
- void setAlwaysOnTop(boolean alwaysOnTop)：设置此窗口是否应始终位于其他窗口之上

了解了这几个方法后，我们到IDEA中去使用一下：

```java
import javax.swing.*;

/*
    void setTitle(String title)：设置窗体标题
    void setLocationRelativeTo(Component c)：设置位置，值为null，则窗体位于屏幕中央
    void setDefaultCloseOperation(int operation)：设置窗体关闭时默认操作(整数3表示：窗口关闭时退出应用程序)
    void setAlwaysOnTop(boolean alwaysOnTop)：设置此窗口是否应始终位于其他窗口之上
 */
public class JFrameDemo02 {
    public static void main(String[] args) {
        //创建窗体对象
        JFrame jf = new JFrame();

        //void setTitle(String title)：设置窗体标题
        jf.setTitle("百度一下，你就知道");
        //设置窗体大小
        jf.setSize(400, 300);
        //void setDefaultCloseOperation(int operation)：设置窗体关闭时默认操作(整数3表示：窗口关闭时退出应用程序)
        jf.setDefaultCloseOperation(3);
        //void setLocationRelativeTo(Component c)：设置位置，值为null，则窗体位于屏幕中央
        jf.setLocationRelativeTo(null);
        //void setAlwaysOnTop(boolean alwaysOnTop)：设置此窗口是否应始终位于其他窗口之上
        jf.setAlwaysOnTop(true);

        //设置窗体可见
        jf.setVisible(true);
    }
}
12345678910111213141516171819202122232425262728
```

##### 18.2.3 JButton(窗口中添加按钮)

下面我们来学习JButton，它是按钮的实现。

**JButton：**

- 按钮的实现

**构造方法：**

- JButton(String text)：创建一个带文本的按钮

**成员方法：**

- void setSize(int width, int height)：设置大小
- void setLocation(int x, int y)：设置位置(x坐标，y坐标)

知道了JButton的构造方法和成员方法后，我们到IDEA中去使用一下：

```java
import javax.swing.*;

/*
    构造方法
        JButton(String text)：创建一个带文本的按钮

    成员方法
        void setSize(int width, int height)：设置大小
        void setLocation(int x, int y)：设置位置(x坐标，y坐标)
 */
public class JButtonDemo {
    public static void main(String[] args) {
        //创建窗体对象
        JFrame jf = new JFrame();

        jf.setTitle("窗口中添加按钮");
        jf.setSize(400, 300);
        jf.setDefaultCloseOperation(3);
        jf.setLocationRelativeTo(null);
        jf.setAlwaysOnTop(true);
        jf.setLayout(null); //取消窗体的默认布局

        //JButton(String text)：创建一个带文本的按钮
        JButton btn = new JButton("我是按钮");
//        //void setSize(int width, int height)：设置大小
//        btn.setSize(100,20);
//        //void setLocation(int x, int y)：设置位置(x坐标，y坐标)
        btn.setLocation(0,0);
//        btn.setLocation(100,100);
        btn.setBounds(100,100,100,20);

        JButton btn2 = new JButton("我是按钮2");
        btn2.setBounds(100,120,100,20);

        jf.add(btn);
        jf.add(btn2);

        //设置窗体可见
        jf.setVisible(true);
    }
}
1234567891011121314151617181920212223242526272829303132333435363738394041
```

演示完毕之后，回到资料再总结一下：

**JButton：**

- 按钮的实现

**构造方法：**

- JButton(String text)：创建一个带文本的按钮

**成员方法：**

- void setSize(int width, int height)：设置大小
- void setLocation(int x, int y)：设置位置(x坐标，y坐标)
- **void setBounds(int x, int y, int width, int height)：设置位置和大小**

**和窗体相关操作：**

- 取消窗体默认布局： **窗体对象.setLayout(null);**
- 把按钮添加到窗体： **窗体对象.add(按钮对象);**

##### 18.2.4 JLabel(显示文本和图像)

下面呢，我们来学习JLable，它是用来做短文本字符串或图像的显示的。

**JLable：**

- 短文本字符串或图像的显示区域

**构造方法：**

- JLabel(String text)：使用指定的文本创建 JLabel实例
- JLabel(Icon image)：使用指定的图像创建 JLabel实例
	- ImageIcon(String filename)：从指定的文件创建ImageIcon
	- 文件路径：绝对路径和相对路径
	- 绝对路径：完整的路径名，不需要任何其他信息就可以定位它所表示的文件
		- 例如：D:\\IdeaProjects\\javase\_code\\itheima-api-gui\\images\\mn.png
	- 相对路径：必须使用取自其他路径名的信息进行解释
		- 例如：itheima-api-gui\\images\\mn.png

**成员方法：**

- void setBounds(int x, int y, int width, int height)：设置位置和大小

知道了JLabel的构造方法和成员方法后，我们到IDEA中去使用一下：

```java
import javax.swing.*;

/*
    构造方法
        JLabel(String text)：使用指定的文本创建 JLabel实例
        JLabel(Icon image)：使用指定的图像创建 JLabel实例
            ImageIcon(String filename)：从指定的文件创建ImageIcon
    成员方法
        void setBounds(int x, int y, int width, int height)：设置位置和大小
 */
public class JLabelDemo {
    public static void main(String[] args) {
        //创建窗体对象
        JFrame jf = new JFrame();

        jf.setTitle("显示文本和图像");
        jf.setSize(400, 300);
        jf.setDefaultCloseOperation(3);
        jf.setLocationRelativeTo(null);
        jf.setAlwaysOnTop(true);
        jf.setLayout(null);

        //JLabel(String text)：使用指定的文本创建 JLabel实例
        JLabel jLabel = new JLabel("好好学习");
        jLabel.setBounds(0,0,100,20);

        //JLabel(Icon image)：使用指定的图像创建 JLabel实例
        //ImageIcon(String filename)：从指定的文件创建ImageIcon
        //D:\IdeaProjects\javase_code\itheima-api-gui\images\mn.png
//        ImageIcon imageIcon = new ImageIcon("D:\\IdeaProjects\\javase_code\\itheima-api-gui\\images\\mn.png");
//        JLabel jLabel2 = new JLabel(imageIcon);
//        JLabel jLabel2 = new JLabel(new ImageIcon("D:\\IdeaProjects\\javase_code\\itheima-api-gui\\images\\mn.png"));
        JLabel jLabel2 = new JLabel(new ImageIcon("itheima-api-gui\\images\\mn.png"));
        jLabel2.setBounds(50,50,100,143);

        jf.add(jLabel);
        jf.add(jLabel2);

        //设置窗体可见
        jf.setVisible(true);
    }
}
123456789101112131415161718192021222324252627282930313233343536373839404142
```

**注意：** 在实际开发中，大家不用担心每个组件的位置和大小。因为这些都是前端人员设计好的。

#### 18.3 案例

下面呢，我们通过几个案例，来使用一下GUI中的常用组件。目前呢，我们仅仅是把界面做出来，下一次课呢，我们就要把最终的功能给实现了。首先，我们来看第一个案例。

##### 18.3.1 案例1(用户登录)

需求：如图所示，做出界面

提示：给出的数据就是按照组件位置和大小给出的

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/df90a1ee288b4b14a8f00ce699bcb355.png)

首先，我们来简单的分析一下：

**分析：**

① 2个JLabel

② 2个JTextField

③ 1个JButton

分析完毕后，我们到IDEA中去实现一下：

```java
import javax.swing.*;

/*
    用户登录
 */
public class UserLogin {
    public static void main(String[] args) {
        //创建窗体对象
        JFrame jf = new JFrame();

        jf.setTitle("用户登录");
        jf.setSize(400, 300);
        jf.setDefaultCloseOperation(3);
        jf.setLocationRelativeTo(null);
        jf.setAlwaysOnTop(true);
        jf.setLayout(null);

        //显示用户名文本
        JLabel usernameLable = new JLabel("用户名");
        usernameLable.setBounds(50,50,50,20);
        jf.add(usernameLable);

        //用户名输入框
        JTextField usernameField = new JTextField();
        usernameField.setBounds(150,50,180,20);
        jf.add(usernameField);

        //显示密码文本
        JLabel passwordLable = new JLabel("密码");
        passwordLable.setBounds(50,100,50,20);
        jf.add(passwordLable);

        //密码输入框
//        JTextField passwordField = new JTextField();
//        passwordField.setBounds(150,100,180,20);
//        jf.add(passwordField);

        JPasswordField passwordField = new JPasswordField();
        passwordField.setBounds(150,100,180,20);
        jf.add(passwordField);

        //登录按钮
        JButton loginButton = new JButton("登录");
        loginButton.setBounds(50,200,280,20);
        jf.add(loginButton);

        jf.setVisible(true);
    }
}
12345678910111213141516171819202122232425262728293031323334353637383940414243444546474849
```

在讲解的过程中，引入了一个新的组件JPasswordField，用来表示密码框。

##### 18.3.2 案例2(聊天室)

需求：如图所示，做出界面

提示：给出的数据就是按照组件位置和大小给出的

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/aafbaa2ec0a84759b2ddc815c9323bbd.png)

首先，我们来简单的分析一下：

**分析：**

① 1个JTextArea

② 1个JTextField

③ 2个JButton

分析完毕后，我们到IDEA中去实现一下：

```java
import javax.swing.*;

/*
    聊天室
 */
public class ChatRoom {
    public static void main(String[] args) {
        //创建窗体对象
        JFrame jf = new JFrame();

        jf.setTitle("聊天室");
        jf.setSize(400, 300);
        jf.setDefaultCloseOperation(3);
        jf.setLocationRelativeTo(null);
        jf.setAlwaysOnTop(true);
        jf.setLayout(null);

        //显示聊天信息的文本域
        JTextArea messageArea = new JTextArea();
        messageArea.setBounds(10,10,360,200);
        jf.add(messageArea);

        //输入聊天信息的文本框
        JTextField messageField = new JTextField();
        messageField.setBounds(10,230,180,20);
        jf.add(messageField);

        //发送按钮
        JButton sendButton = new JButton("发送");
        sendButton.setBounds(200,230,70,20);
        jf.add(sendButton);

        //清空聊天按钮
        JButton clearButton = new JButton("清空聊天");
        clearButton.setBounds(280,230,100,20);
        jf.add(clearButton);

        jf.setVisible(true);
    }
}
12345678910111213141516171819202122232425262728293031323334353637383940
```

##### 18.3.3 案例3(猜数字)

需求：如图所示，做出界面

提示：给出的数据就是按照组件位置和大小给出的

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/a4c51638b9fc4df582c45ddd739ac983.png)

首先，我们来简单的分析一下：

**分析：**

① 1个JLabel

② 1个JTextField

③ 1个JButton

分析完毕后，我们到IDEA中去实现一下：

```java
import javax.swing.*;

/*
    猜数字
 */
public class GuessNumber {
    public static void main(String[] args) {
        //创建窗体对象
        JFrame jf = new JFrame();

        jf.setTitle("猜数字");
        jf.setSize(400, 300);
        jf.setDefaultCloseOperation(3);
        jf.setLocationRelativeTo(null);
        jf.setAlwaysOnTop(true);
        jf.setLayout(null);

        //提示信息
        JLabel messageLable = new JLabel("系统产生了一个1-100之间的数据，请猜一猜");
        messageLable.setBounds(70,50,350,20);
        jf.add(messageLable);

        //输入要猜的数字
        JTextField numberField = new JTextField();
        numberField.setBounds(120,100,150,20);
        jf.add(numberField);

        //猜数字的按钮
        JButton guessButton = new JButton("我猜");
        guessButton.setBounds(150,150,100,20);
        jf.add(guessButton);

        jf.setVisible(true);
    }
}
1234567891011121314151617181920212223242526272829303132333435
```

##### 18.3.4 案例4(手机日期和时间显示)

需求：如图所示，做出界面

提示：给出的数据就是按照组件位置和大小给出的

参照图：

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/77392ce16647416da8dc5ab7b452ba64.png)

我们要实现的图：

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/b3020d705ebf44f9af9fd3ab4b4daac4.png)

首先，我们来简单的分析一下：

**分析：**

① 4个JLabel

分析完毕后，我们到IDEA中去实现一下：

```java
import javax.swing.*;

/*
    手机日期和时间显示
 */
public class ShowDateTime {
    public static void main(String[] args) {
        //创建窗体对象
        JFrame jf = new JFrame();

        jf.setTitle("手机日期和时间显示");
        jf.setSize(400, 300);
        jf.setDefaultCloseOperation(3);
        jf.setLocationRelativeTo(null);
        jf.setAlwaysOnTop(true);
        jf.setLayout(null);

        //提示日期
        JLabel dateLable = new JLabel("日期");
        dateLable.setBounds(50,50,100,20);
        jf.add(dateLable);

        //按照格式显示日期的字符串
        JLabel showDateLable = new JLabel("xxxx年xx月xx日");
        showDateLable.setBounds(50,80,200,20);
        jf.add(showDateLable);

        //提示时间
        JLabel timeLable = new JLabel("时间");
        timeLable.setBounds(50,150,100,20);
        jf.add(timeLable);

        //按照格式显示时间的字符串
        JLabel showTimeLable = new JLabel("xx:xx");
        showTimeLable.setBounds(50,180,200,20);
        jf.add(showTimeLable);

        jf.setVisible(true);
    }
}
12345678910111213141516171819202122232425262728293031323334353637383940
```

##### 18.3.5 案例5(考勤查询)

需求：如图所示，做出界面

提示：给出的数据就是按照组件位置和大小给出的

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/9a1f057445ef4dde82e4ee25a831a454.png)

首先，我们来简单的分析一下：

**分析：**

① 3个JLabel

② 2个JTextField

③ 1个JButton

分析完毕后，我们到IDEA中去实现一下：

```java
import javax.swing.*;

/*
    考勤查询
 */
public class AttendanceQuery01 {
    public static void main(String[] args) {
        //创建窗体对象
        JFrame jf = new JFrame();

        jf.setTitle("考勤查询");
        jf.setSize(400, 300);
        jf.setDefaultCloseOperation(3);
        jf.setLocationRelativeTo(null);
        jf.setAlwaysOnTop(true);
        jf.setLayout(null);

        //显示考勤日期的文本
        JLabel dateLable = new JLabel("考勤日期");
        dateLable.setBounds(50,20,100,20);
        jf.add(dateLable);

        //显示开始时间文本
        JLabel startDateLable = new JLabel("开始时间");
        startDateLable.setBounds(50,70,100,20);
        jf.add(startDateLable);

        //开始时间输入框
        JTextField startDateField = new JTextField();
        startDateField.setBounds(50,100,100,20);
        jf.add(startDateField);

        //显示结束时间文本
        JLabel endDateLable = new JLabel("结束时间");
        endDateLable.setBounds(250,70,100,20);
        jf.add(endDateLable);

        //结束时间输入框
        JTextField endDateField = new JTextField();
        endDateField.setBounds(250,100,100,20);
        jf.add(endDateField);

        //确定按钮
        JButton confirmButton = new JButton("确定");
        confirmButton.setBounds(250,180,60,20);
        jf.add(confirmButton);

        jf.setVisible(true);
    }
}
1234567891011121314151617181920212223242526272829303132333435363738394041424344454647484950
```

##### 18.3.6 案例5(考勤查询之日历控件)

需求：用日历控件改进考勤查询的日期字符串填写

下面我们来学习考勤查询之日历控件

首先，我们看一下需求：用日历控件改进考勤查询的日期字符串填写

什么意思呢？我们刚在做的考勤查询系统，是需要手动输入日期字符串的，而在实际开发中，我们一般会选择使用日历控件来实现，

也就是下面这个样子的，我们点击一下，就会出现日历控件，我们选择日期就可以了。

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/75874a08616e4930ac935e637f0f7ff5.png)

这个相信大家有见过。

知道了要做什么之后，下面我们来说一下，怎么做。

我们可以自己写这个日历控件，也可以使用别人写好的日历控件。鉴于目前所学知识有限，我们先使用别人提供的日历控件。

这里呢，我准备好了一个 **日历控件类(DateChooser.java)** ，我们到IDEA中一起去看一下如何使用：

```java
public static void main(String[] args) {
    //创建窗体
    JFrame jf = new JFrame();

    //设置窗体大小
    jf.setSize(400, 300);
    //设置窗体标题
    jf.setTitle("日历控件");
    //设置位置，值为null，则窗体位于屏幕中央
    jf.setLocationRelativeTo(null);
    //设置窗体关闭时默认操作，窗口关闭时退出应用程序
    jf.setDefaultCloseOperation(3);
    //设置此窗口是否应始终位于其他窗口之上
    jf.setAlwaysOnTop(true);
    //取消窗体默认布局：窗体对象.setLayout(null);
    jf.setLayout(null);

    //创建日期选择器对象，指定日期字符串格式
    DateChooser dateChooser = DateChooser.getInstance("yyyy-MM-dd");

    JTextField showDateField = new JTextField("单击选择日期");
    showDateField.setBounds(50, 50, 100, 20);

    //把日历控件和文本框进行绑定
    dateChooser.register(showDateField);

    jf.add(showDateField);

    jf.setVisible(true);
}
123456789101112131415161718192021222324252627282930
```

了解了如何使用日历控件后，我们把开始写的代码改进一下：

```java
import javax.swing.*;

/*
    考勤查询
 */
public class AttendanceQuery02 {
    public static void main(String[] args) {
        //创建窗体对象
        JFrame jf = new JFrame();

        jf.setTitle("考勤查询");
        jf.setSize(400, 300);
        jf.setDefaultCloseOperation(3);
        jf.setLocationRelativeTo(null);
        jf.setAlwaysOnTop(true);
        jf.setLayout(null);

        //显示考勤日期的文本
        JLabel dateLable = new JLabel("考勤日期");
        dateLable.setBounds(50,20,100,20);
        jf.add(dateLable);

        //显示开始时间文本
        JLabel startDateLable = new JLabel("开始时间");
        startDateLable.setBounds(50,70,100,20);
        jf.add(startDateLable);

        DateChooser dateChooser1 = DateChooser.getInstance("yyyy/MM/dd");
        DateChooser dateChooser2 = DateChooser.getInstance("yyyy/MM/dd");
        //开始时间输入框
        JTextField startDateField = new JTextField();
        startDateField.setBounds(50,100,100,20);
        dateChooser1.register(startDateField);
        jf.add(startDateField);

        //显示结束时间文本
        JLabel endDateLable = new JLabel("结束时间");
        endDateLable.setBounds(250,70,100,20);
        jf.add(endDateLable);

        //结束时间输入框
        JTextField endDateField = new JTextField();
        endDateField.setBounds(250,100,100,20);
        dateChooser2.register(endDateField);
        jf.add(endDateField);

        //确定按钮
        JButton confirmButton = new JButton("确定");
        confirmButton.setBounds(250,180,60,20);
        jf.add(confirmButton);

        jf.setVisible(true);
    }
}
123456789101112131415161718192021222324252627282930313233343536373839404142434445464748495051525354
```

#### 18.4 事件监听机制

目前呢，我们做好了几个GUI的界面，但是具体的功能，我们没法实现。因为要想实现功能，就必须要学习一下事件监听机制。

这里，我们一起来说一下 **事件监听机制的组成：**

- \*\*事件源：\*\*事件发生的地方。可以是按钮，窗体，图片等
- \*\*事件：\*\*发生了什么事情。例如：鼠标点击事件，键盘按下事件等
- \*\*事件绑定：\*\*把事件绑定到事件源上，当发生了某个事件，则触发对应的处理逻辑
	- 事件源对象. addXXXListener(事件);

GUI中的事件比较多，这里呢，我们先告诉一下大家如何给按钮添加事件，能够把我们前面的案例给实现就可以了。至于其他事件，后面我们用到的时候再去学习。

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/eb4fc209e6544e648826387349fc2e90.png)

了解了如何给按钮添加事件后，我们到IDEA中去体验一下：

```java
import javax.swing.*;
import java.awt.event.ActionEvent;
import java.awt.event.ActionListener;

/*
    事件监听机制
 */
public class ActionListenerDemo {
    public static void main(String[] args) {
        //创建窗体对象
        JFrame jf = new JFrame();

        jf.setTitle("事件监听机制");
        jf.setSize(400, 300);
        jf.setDefaultCloseOperation(3);
        jf.setLocationRelativeTo(null);
        jf.setAlwaysOnTop(true);
        jf.setLayout(null);

        //创建按钮
        JButton jButton = new JButton("你点我啊");
        jButton.setBounds(0, 0, 100, 100);
        jf.add(jButton);

        jButton.addActionListener(new ActionListener() {
            @Override
            public void actionPerformed(ActionEvent e) {
                System.out.println("你点我啊");
            }
        });

        jf.setVisible(true);
    }
}
12345678910111213141516171819202122232425262728293031323334
```

## 八、常用API(2)

**本节目标：**

- 能够使用String类的功能完成用户登录案例
- 能够使用String类的功能完成聊天室案例
- 能够使用Integer类的功能完成猜数字案例
- 能够使用Date类和SimpleDateFormat类的功能完成手机日期和时间显示案例
- 能够使用Date类和SimpleDateFormat类的功能完成考勤查询案例

### 19：String

#### 19.1 String(构造方法)

前面我们做过了GUI中的案例，也就是把一些小应用的界面做好了，但是具体功能并没有实现。接下来呢，我们就来一起实现一下。

首先，我们先来学习String类，它涉及到两个案例：用户登录和聊天室。

先来看用户登录案例：需要输入用户名和密码，和已知的用户名和密码进行比较，涉及到比较的方法，

一般来说，用户名和密码的长度可能会有一定限制，涉及到获取字符串长度的方法，

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/80b5102397e346cab33572e958a6e40e.png)

再来看聊天室案例，这里输入聊天的内容，然后把聊天内容显示到上面的文本域。

在聊天的时候，可能不小心打了空格，我们不需要的，需要去掉前后空格，

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/afe11e16561e42aab4ab05f3225fbb5b.png)

当然了，还有很多其他的成员方法，只不过，目前我们暂时用不上，后面用的时候再讲。

下面，我们就来学习一下字符串类String，最后完成用户登录案例和聊天室案例。

而关于String类呢，我们先到帮助文档中去查看，然后回来总结，最后到IDEA中去演示。

来，打开我们准备好的帮助文档，关于通过帮助文档查看String，大家按照老师讲解的API的使用步骤看看即可。

通过文档了解了String类之后，下面我们回到资料中总结一下：

**String：**

- String类表示字符串。 Java程序中的所有字符串文字（例如"abc" ）都实现为此类的实例

**构造方法：**

- String()：初始化新创建的 String对象，使其表示空字符序列
- String(String original)：初始化新创建的String对象，使其表示与参数相同的字符序列

知道了String的构造方法后，我们到IDEA中去使用一下：

```java
/*
    String类表示字符串。 Java程序中的所有字符串文字（例如"abc" ）都实现为此类的实例

    构造方法：
        String()：初始化新创建的 String对象，使其表示空字符序列
        String(String original)：初始化新创建的String对象，使其表示与参数相同的字符序列
 */
public class StringDemo01 {
    public static void main(String[] args) {
        //String()：初始化新创建的 String对象，使其表示空字符序列
        String s1 = new String();
        System.out.println(s1);
        //int length() 返回此字符串的长度
        System.out.println(s1.length());
        System.out.println("------------");

        //String(String original)：初始化新创建的String对象，使其表示与参数相同的字符序列
        String s2 = new String("itheima");
        System.out.println(s2);
        System.out.println(s2.length());
        System.out.println("------------");

        //Java程序中的所有字符串文字（例如"abc" ）都实现为此类的实例
        String s3 = "itheima";
        System.out.println(s3);
        System.out.println(s3.length());
    }
}
12345678910111213141516171819202122232425262728
```

#### 19.2 String(成员方法)

下面我们来学习String类中常用的成员方法：

- int length()：返回此字符串的长度
- boolean equals(Object anObject)：将此字符串与指定的对象进行比较
- boolean equalsIgnoreCase(String anotherString)：将此 String与另一个 String比较，忽略了大小写
- String trim()：返回一个字符串，其值为此字符串，删除了所有前导和尾随空格

而关于这几个成员方法呢，我们到IDEA中一边使用，一边讲解。

```java
/*
    int length()：返回此字符串的长度
    boolean equals(Object anObject)：将此字符串与指定的对象进行比较
    boolean equalsIgnoreCase(String anotherString)：将此 String与另一个 String比较，忽略了大小写
    String trim()：返回一个字符串，其值为此字符串，删除了所有前导和尾随空格
 */
public class StringDemo02 {
    public static void main(String[] args) {
        String s1 = "itheima";
        String s2 = "itheima";
        String s3 = "Itheima";

        //boolean equals(Object anObject)：将此字符串与指定的对象进行比较
        System.out.println(s1.equals(s2));
        System.out.println(s1.equals(s3));

        //boolean equalsIgnoreCase(String anotherString)：将此 String与另一个 String比较，忽略了大小写
        System.out.println(s1.equalsIgnoreCase(s2));
        System.out.println(s1.equalsIgnoreCase(s3));
        System.out.println("-------------------");

        String s4 = " itheima ";
        //String trim()：返回一个字符串，其值为此字符串，删除了所有前导和尾随空格
        System.out.println(s4);
        System.out.println(s4.trim());

        String s5 = "it heima";
        System.out.println(s5.trim());
    }
}
123456789101112131415161718192021222324252627282930
```

#### 19.3 GUI案例1(用户登录实现)

需求：根据下列要求，完成用户登录的逻辑，并给出相应的提示

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/a2b2a7dab565401cbda464d1f1d8f9bf.png)

要求：

① 已知的用户名和密码

```java
用户名：itheima

密码：123456
123
```

② 用户名和密码的长度都是6-12位

③ 点击登录按钮

```java
先判断输入的用户名和密码是否符合要求

再判断用户登录是否成功
123
```

知道了用户登录案例的需求和要求后，下面我们到IDEA中去实现一下：

```java
import javax.swing.*;
import java.awt.event.ActionEvent;
import java.awt.event.ActionListener;

/*
    1:已知的用户名和密码
        用户名：itheima
       密码：123456
    2:用户名和密码的长度都是6-12位
    3:点击登录按钮
       先判断输入的用户名和密码是否符合要求
       再判断用户登录是否成功
 */
public class UserLogin {
    public static void main(String[] args) {
        //创建窗体对象
        JFrame jf = new JFrame();

        jf.setTitle("用户登录");
        jf.setSize(400, 300);
        jf.setDefaultCloseOperation(3);
        jf.setLocationRelativeTo(null);
        jf.setAlwaysOnTop(true);
        jf.setLayout(null);

        //显示用户名文本
        JLabel usernameLable = new JLabel("用户名");
        usernameLable.setBounds(50, 50, 50, 20);
        jf.add(usernameLable);

        //用户名输入框
        JTextField usernameField = new JTextField();
        usernameField.setBounds(150, 50, 180, 20);
        jf.add(usernameField);

        //显示密码文本
        JLabel passwordLable = new JLabel("密码");
        passwordLable.setBounds(50, 100, 50, 20);
        jf.add(passwordLable);

        //密码输入框
        JPasswordField passwordField = new JPasswordField();
        passwordField.setBounds(150, 100, 180, 20);
        jf.add(passwordField);

        //登录按钮
        JButton loginButton = new JButton("登录");
        loginButton.setBounds(50, 200, 280, 20);
        jf.add(loginButton);

        //已知的用户名和密码
        String name = "itheima";
        String pwd = "123456";

        loginButton.addActionListener(new ActionListener() {
            @Override
            public void actionPerformed(ActionEvent e) {
                //获取用户输入的用户名和密码
                String username = usernameField.getText();
                String password = passwordField.getText();

                //先判断输入的用户名和密码是否符合要求
                //用户名和密码的长度都是6-12位
                if(username.length()<6 || username.length()>12) {
//                    System.out.println("用户名的长度是6-12位，请重新输入");
                    //静态的成员方法和成员变量是可以通过类名访问的
                    JOptionPane.showMessageDialog(jf,"用户名的长度是6-12位，请重新输入");
                    usernameField.setText("");
                    return;
                }

                //再判断用户登录是否成功
                if(username.equals(name) && password.equals(pwd)) {
//                    System.out.println("登录成功");
                    JOptionPane.showMessageDialog(jf,"登录成功");
                    usernameField.setText("");
                    passwordField.setText("");
                } else {
//                    System.out.println("用户名或者密码有误");
                    JOptionPane.showMessageDialog(jf,"用户名或者密码有误");
                }
            }
        });

        jf.setVisible(true);
    }
}
123456789101112131415161718192021222324252627282930313233343536373839404142434445464748495051525354555657585960616263646566676869707172737475767778798081828384858687
```

#### 19.4 GUI案例2(聊天室实现)

需求：根据下列要求，完成聊天室的逻辑

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/a0e4cb66fc034df9b8dd632b3e147b19.png)

要求：

① 把文本框的内容发送到文本域中

② 每次发送的文本内容不带前后空格

③ 多次发送的内容在文本域以追加的方式呈现

④ 清空聊天就是把文本域的内容设置为空

知道了聊天室案例的需求和要求后，下面我们到IDEA中去实现一下：

```java
import javax.swing.*;
import java.awt.event.ActionEvent;
import java.awt.event.ActionListener;

/*
    1:把文本框的内容发送到文本域中
    2:每次发送的文本内容不带前后空格
    3:多次发送的内容在文本域以追加的方式呈现
    4:清空聊天就是把文本域的内容设置为空
 */
public class ChatRoom {
    public static void main(String[] args) {
        //创建窗体对象
        JFrame jf = new JFrame();

        jf.setTitle("聊天室");
        jf.setSize(400, 300);
        jf.setDefaultCloseOperation(3);
        jf.setLocationRelativeTo(null);
        jf.setAlwaysOnTop(true);
        jf.setLayout(null);

        //显示聊天信息的文本域
        JTextArea messageArea = new JTextArea();
        messageArea.setBounds(10, 10, 360, 200);
        jf.add(messageArea);

        //输入聊天信息的文本框
        JTextField messageField = new JTextField();
        messageField.setBounds(10, 230, 180, 20);
        jf.add(messageField);

        //发送按钮
        JButton sendButton = new JButton("发送");
        sendButton.setBounds(200, 230, 70, 20);
        jf.add(sendButton);

        //清空聊天按钮
        JButton clearButton = new JButton("清空聊天");
        clearButton.setBounds(280, 230, 100, 20);
        jf.add(clearButton);

        sendButton.addActionListener(new ActionListener() {
            @Override
            public void actionPerformed(ActionEvent e) {
                //获取文本框的内容
//                String message = messageField.getText();
//                messageField.setText("");

                //每次发送的文本内容不带前后空格
//                String message = messageField.getText();
//                message = message.trim();
                String message = messageField.getText().trim(); //链式调用
                messageField.setText("");

                //把文本框的内容发送到文本域中
//                messageArea.setText(message);
                //多次发送的内容在文本域以追加的方式呈现
                messageArea.append(message+"\n");
            }
        });

        clearButton.addActionListener(new ActionListener() {
            @Override
            public void actionPerformed(ActionEvent e) {
                //清空聊天就是把文本域的内容设置为空
                messageArea.setText("");
            }
        });

        jf.setVisible(true);
    }
}
1234567891011121314151617181920212223242526272829303132333435363738394041424344454647484950515253545556575859606162636465666768697071727374
```

### 20：Integer

#### 20.1 Integer(构造方法)

下面我们来学习基本类型包装类，它涉及到1个案例：猜数字。

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/a9b76f1911cf4e5b93fdc4afc0c78bc7.png)

来，我们一起看一下，在这个输入框里，我们要输入一个猜的数据，然后点击我猜这个按钮，和已经产生的数据进行比对，给出相应的提示即可。

而且呢，猜数字案例的基本逻辑，我们前面是讲解过的，只不过当时使用的是键盘录入数据，而这里我们采用的是在输入框里输入数据而已。

那我们为什么要学习基本类型包装类呢？

因为，在输入框里输入的数据，我们得到的是一个字符串数据，而实际比较的时候我们需要的是一个int类型的数据，所以，我们得想办法把字符串数据转换为int类型的数据。

为了实现这个效果，Java就提供了基本类型包装类供我们使用。所以，我们说，将基本数据类型封装成对象的好处就是可以通过对象调用方法操作数据。

而我们常用的操作之一呢：就是用于基本数据类型与字符串之间的转换。

在这里呢，我们一起来看一下，八种基本数据类型和其对应的包装类类型

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/771931894600436cb837049cf6813da6.png)

从名字上看，包装类类型就是把基本类型的第一个单词改为大写即可。

当然，这里也有两个比较特殊的，一个是int类型的包装类，一个是字符类型的包装类，它们的包装类名称是这个样子的，大家了解一下即可。

下面呢，我们以Integer举例来讲解字符串和int类型之间的相互转换，其他基本类型和字符串的转换方式类似，在使用的时候，大家参照Integer的使用即可。

而关于Integer类的学习呢，我们先到帮助文档中去查看，然后回来总结，最后到IDEA中去演示。

来，打开我们准备好的帮助文档，关于通过帮助文档查看Integer，大家按照老师讲解的API的使用步骤看看即可。

通过文档了解了Integer类之后，下面我们回到资料中总结一下：

**Integer：**

- Integer类在对象中包装基本类型int的值

**构造方法：**

- Integer(int value)：根据 int 值创建 Integer 对象(过时)
- Integer(String s)：根据 String 值创建 Integer 对象(过时)

**成员方法：**

- static Integer valueOf(int i)：返回表示指定的 int 值的 Integer 实例
- static Integer valueOf(String s)：返回一个保存指定值的 Integer 对象 String

知道了Integer的构造方法后，我们到IDEA中去使用一下：

```java
/*
    构造方法
        Integer(int value)：根据 int 值创建 Integer 对象(过时)
        Integer(String s)：根据 String 值创建 Integer 对象(过时)

    成员方法
        static Integer valueOf(int i)：返回表示指定的 int 值的 Integer 实例
        static Integer valueOf(String s)：返回一个保存指定值的 Integer 对象 String
 */
public class IntegerDemo01 {
    public static void main(String[] args) {
//        //Integer(int value)：根据 int 值创建 Integer 对象(过时)
//        Integer i1 = new Integer(100);
//        System.out.println(i1);
//
//        //Integer(String s)：根据 String 值创建 Integer 对象(过时)
//        Integer i2 = new Integer("100");
//        System.out.println(i2);

//        static Integer valueOf(int i)：返回表示指定的 int 值的 Integer 实例
//        static Integer valueOf(String s)：返回一个保存指定值的 Integer 对象 String
        Integer i1 = Integer.valueOf(100);
        Integer i2 = Integer.valueOf("100");
        System.out.println(i1);
        System.out.println(i2);
    }
}
123456789101112131415161718192021222324252627
```

#### 20.2 Integer(int和String的相互转换)

下面我们来学习int类型数据和String类型数据的相互转换，关于它们之间的相互转换，我们先到IDEA中去讲解，然后回来总结。

```java
/*
    int和String的相互转换
 */
public class IntegerDemo02 {
    public static void main(String[] args) {
        //int --- String
        int number = 100;
        //方式1
        String s1 = number + "";
        System.out.println(s1);
        //方式2
        //static String valueOf(int i)
        String s2 = String.valueOf(number);
        System.out.println(s2);
        System.out.println("---------------");

        //String --- int
        String s = "100";
        //方式1：String --- Integer --- int
        Integer i = Integer.valueOf(s);
        //int intValue() 返回此值 Integer为 int
        int x = i.intValue();
        System.out.println(x);
        //方式2
        //static int parseInt(String s)
        int y = Integer.parseInt(s);
        System.out.println(y);
    }
}
1234567891011121314151617181920212223242526272829
```

讲解完毕int类型和String类型的相互转换后，回到资料总结一下：

- **int 转换为 String**
	- **static String valueOf(int i)：** 返回 int 参数的字符串表示形式。该方法是 String 类中的方法
- **String 转换为 int**
	- **static int parseInt(String s)：** 将字符串解析为 int 类型。该方法是 Integer 类中的方法

好了，int类型数据和String类型数据的相互转换我们就先讲到这里。

#### 20.3 GUI案例3(猜数字实现)

需求：根据下列要求，完成猜数字的逻辑

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/c087ace72b5c4e0191bcd859f19275df.png)

要求：

① 系统产生一个1-100之间的随机数

② 猜的内容不能为空

③ 每次根据猜的数字给出相应的提示

知道了猜数字案例的需求和要求后，下面我们到IDEA中去实现一下：

```java
import javax.swing.*;
import java.awt.event.ActionEvent;
import java.awt.event.ActionListener;
import java.util.Random;

/*
    1:系统产生一个1-100之间的随机数
    2:猜的内容不能为空
    3:每次根据猜的数字给出相应的提示
*/
public class GuessNumber {
    public static void main(String[] args) {
        //创建窗体对象
        JFrame jf = new JFrame();

        jf.setTitle("猜数字");
        jf.setSize(400, 300);
        jf.setDefaultCloseOperation(3);
        jf.setLocationRelativeTo(null);
        jf.setAlwaysOnTop(true);
        jf.setLayout(null);

        //系统产生一个1-100之间的随机数
        Random r = new Random();
        int number = r.nextInt(100) + 1;

        //提示信息
        JLabel messageLable = new JLabel("系统产生了一个1-100之间的数据，请猜一猜");
        messageLable.setBounds(70, 50, 350, 20);
        jf.add(messageLable);

        //输入要猜的数字
        JTextField numberField = new JTextField();
        numberField.setBounds(120, 100, 150, 20);
        jf.add(numberField);

        //猜数字的按钮
        JButton guessButton = new JButton("我猜");
        guessButton.setBounds(150, 150, 100, 20);
        jf.add(guessButton);

        guessButton.addActionListener(new ActionListener() {
            @Override
            public void actionPerformed(ActionEvent e) {
                //猜的内容不能为空
                String stringNumber = numberField.getText().trim();
                if(stringNumber.equals("")) {
                    JOptionPane.showMessageDialog(jf,"猜的数字不能为空");
                    return;
                }

                //每次根据猜的数字给出相应的提示
                int guessNumber = Integer.parseInt(stringNumber);

                if(guessNumber > number) {
                    JOptionPane.showMessageDialog(jf,"你猜的数字"+guessNumber+"大了");
                    numberField.setText("");
                } else if(guessNumber < number) {
                    JOptionPane.showMessageDialog(jf,"你猜的数字"+guessNumber+"小了");
                    numberField.setText("");
                } else  {
                    JOptionPane.showMessageDialog(jf,"恭喜你猜中了");
                }
            }
        });

        jf.setVisible(true);
    }
}
123456789101112131415161718192021222324252627282930313233343536373839404142434445464748495051525354555657585960616263646566676869
```

#### 20.4 Integer(自动装箱和拆箱)

下面我们来学习自动装箱和拆箱。

首先，我们来说一下什么是装箱和拆箱：

- \*\*装箱：\*\*把基本数据类型转换为对应的包装类类型
- \*\*拆箱：\*\*把包装类类型转换为对应的基本数据类型

了解了装箱和拆箱后，下面我们到IDEA中去演示一下：

```java
/*
    装箱：把基本数据类型转换为对应的包装类类型
    拆箱：把包装类类型转换为对应的基本数据类型
 */
public class IntegerDemo03 {
    public static void main(String[] args) {
        //装箱：把基本数据类型转换为对应的包装类类型
//        Integer i = Integer.valueOf(100);
        Integer ii = 100; //Integer.valueOf(100);

        //拆箱：把包装类类型转换为对应的基本数据类型
        ii += 200;
        /*
            ii = ii + 200;
            ii = ii.intValue() + 200;   //自动拆箱
            ii = 300; //Integer.valueOf(300);
         */
        System.out.println(ii);
    }
}
1234567891011121314151617181920
```

好了，自动装箱和拆箱我们就先讲到这里。

### 21：Date和SimpleDateFormat

#### 21.1 Date(构造方法)

下面我们来学习Date类和SimpleDateFormat类，它们涉及到两个案例：手机日期和时间显示和考勤查询

先来看手机日期和时间显示案例：获取当前时间，按照指定的格式显示在窗体上。

也就是在这里我们要进行把一个Date类型的数据，按照指定的格式，变成一个字符串数据显示出来。

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/21bb5c627b33437ba5bfe827b32e0df1.png)

再来看考勤查询案例，我们要通过输入的指定格式的日期字符串数据，得到Date类型的数据。

所以，我们学习Date类和SimpleDateFormat类的重点就是为了把Date类型数据和String类型数据之间进行按照指定格式进行转换。

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/9be96c152a3241a4a038f679801716da.png)

首先呢，我们先来学习一下Date类，而关于Date类呢，我们先到帮助文档中去查看，然后回来总结，最后到IDEA中去演示。

来，打开我们准备好的帮助文档，关于通过帮助文档查看Date，大家按照老师讲解的API的使用步骤看看即可。

通过文档了解了Date类之后，下面我们回到资料中总结一下：

**Date：**

- Date类表示特定的时刻，精度为毫秒

**构造方法：**

- Date()：分配 Date对象并对其进行初始化，使其表示分配时间，测量 Date到毫秒
- Date(long date)：分配 Date对象并初始化它以表示自 **标准基准时间** 以来的指定毫秒数，即 **1970年1月1日00:00:00**

知道了(的构造方法后，我们到IDEA中去使用一下：

```java
import java.util.Date;

/*
    构造方法：
        Date()：分配 Date对象并对其进行初始化，使其表示分配时间，测量 Date到毫秒
        Date(long date)：分配 Date对象并初始化它以表示自标准基准时间以来的指定毫秒数，即1970年1月1日00:00:00
 */
public class DateDemo {
    public static void main(String[] args) {
        //Date()：分配 Date对象并对其进行初始化，使其表示分配时间，测量 Date到毫秒
        Date d1 = new Date();
        System.out.println(d1);

        //Date(long date)：分配 Date对象并初始化它以表示自标准基准时间以来的指定毫秒数，即1970年1月1日00:00:00
        Date d2 = new Date(1000 * 60 * 60);
        System.out.println(d2);
    }
}
123456789101112131415161718
```

而目前呢，Date类中没有我们要使用的成员方法，所以，我们也就不看它的成员方法了。

#### 21.2 SimpleDateFormat(Date和String的相互转换)

下面我们来学习SimpleDateFormat这个类。

打开我们准备好的帮助文档，关于通过帮助文档查看SimpleDateFormat，大家按照老师讲解的API的使用步骤看看即可。

通过文档了解了SimpleDateFormat类之后，下面我们回到资料中总结一下：

**SimpleDateFormat：**

- SimpleDateFormat 是一个用于以区域设置敏感的方式格式化和解析日期的具体类。我们重点学习日期格式化和解析
- 日期和时间格式由日期和时间模式字符串指定，在日期和时间模式字符串中，从‘A’到‘Z’以及从‘a’到‘z’引号的字母被解释为表示日期或时间字符串的组成部分的模式字母

常用的模式字母及对应关系如下：

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/15598b5ed3c544c0952f4c5bf39854b9.png)

- **举例：** 2021年10月27日 11:11:11
- **模式：** yyyy年MM月dd日 HH:mm:ss

**构造方法：**

- SimpleDateFormat()：构造一个SimpleDateFormat，使用默认模式和日期格式
- SimpleDateFormat(String pattern)：构造一个SimpleDateFormat使用给定的模式和默认的日期格式

**格式化(从 Date 到 String )：**

- String format(Date date)：将日期格式化成日期/时间字符串

**解析(从 String 到 Date )：**

- Date parse(String source)：从给定字符串的开始解析文本以生成日期

了解了SimpleDateFormat类，以及Date和String相互转换的方法后，我们到IDEA中去体验一下：

```java
import java.text.ParseException;
import java.text.SimpleDateFormat;
import java.util.Date;

/*
    构造方法
        SimpleDateFormat()：构造一个SimpleDateFormat，使用默认模式和日期格式
        SimpleDateFormat(String pattern)：构造一个SimpleDateFormat使用给定的模式和默认的日期格式

    格式化(从 Date 到 String )
        String format(Date date)：将日期格式化成日期/时间字符串

    解析(从 String 到 Date )
        Date parse(String source)：从给定字符串的开始解析文本以生成日期
 */
public class SimpleDateFormatDemo {
    public static void main(String[] args) throws ParseException {
        //格式化(从 Date 到 String )
        Date d = new Date();
        //SimpleDateFormat()：构造一个SimpleDateFormat，使用默认模式和日期格式
//        SimpleDateFormat sdf = new SimpleDateFormat();
        //SimpleDateFormat(String pattern)：构造一个SimpleDateFormat使用给定的模式和默认的日期格式
        SimpleDateFormat sdf = new SimpleDateFormat("yyyy年MM月dd日 HH:mm:ss");
        String s = sdf.format(d);
        System.out.println(s);
        System.out.println("-----------------");

        //解析(从 String 到 Date )
        String ss = "2021-10-27 11:11:11";
//        SimpleDateFormat sdf2 = new SimpleDateFormat("yyyy年MM月dd日 HH:mm:ss");
        SimpleDateFormat sdf2 = new SimpleDateFormat("yyyy-MM-dd HH:mm:ss");

        Date dd = sdf2.parse(ss);
        System.out.println(dd);
    }
}
123456789101112131415161718192021222324252627282930313233343536
```

#### 21.3 GUI案例4(手机日期和时间显示实现)

需求：根据下列要求，完成手机日期和时间显示

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/a549715fdf334f91871cd5d64fd9b39e.png)

要求：以当前时间根据格式分别获取日期和时间显示

知道了手机日期和时间显示案例的需求和要求后，下面我们到IDEA中去实现一下：

```java
import javax.swing.*;
import java.text.SimpleDateFormat;
import java.util.Date;

/*
    手机日期和时间显示
 */
public class ShowDateTime {
    public static void main(String[] args) {
        //创建窗体对象
        JFrame jf = new JFrame();

        jf.setTitle("手机日期和时间显示");
        jf.setSize(400, 300);
        jf.setDefaultCloseOperation(3);
        jf.setLocationRelativeTo(null);
        jf.setAlwaysOnTop(true);
        jf.setLayout(null);

        //提示日期
        JLabel dateLable = new JLabel("日期");
        dateLable.setBounds(50, 50, 100, 20);
        jf.add(dateLable);

        Date d = new Date();

        SimpleDateFormat sdf = new SimpleDateFormat("yyyy年MM月dd日");
        String dateString = sdf.format(d);

        //按照格式显示日期的字符串
        JLabel showDateLable = new JLabel(dateString);
        showDateLable.setBounds(50, 80, 200, 20);
        jf.add(showDateLable);

        //提示时间
        JLabel timeLable = new JLabel("时间");
        timeLable.setBounds(50, 150, 100, 20);
        jf.add(timeLable);

        SimpleDateFormat sdf2 = new SimpleDateFormat("HH:mm");
        String timeString = sdf2.format(d);

        //按照格式显示时间的字符串
        JLabel showTimeLable = new JLabel(timeString);
        showTimeLable.setBounds(50, 180, 200, 20);
        jf.add(showTimeLable);

        jf.setVisible(true);
    }
}
1234567891011121314151617181920212223242526272829303132333435363738394041424344454647484950
```

#### 21.4 GUI案例5(考勤查询实现)

需求：根据下列要求，完成考勤查询的逻辑

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://i-blog.csdnimg.cn/direct/dc6eb65b2ed0482f99663eec93819c21.png)

要求：根据开始时间和结束时间的字符串解析为日期提示出来

知道了考勤查询案例的需求和要求后，下面我们到IDEA中去实现一下：

**这里用到了日历控件类，需要大家把DateChooser.java类准备好**

```java
import javax.swing.*;
import java.awt.event.ActionEvent;
import java.awt.event.ActionListener;
import java.text.ParseException;
import java.text.SimpleDateFormat;
import java.util.Date;

/*
    考勤查询
 */
public class AttendanceQuery {
    public static void main(String[] args) {
        //创建窗体对象
        JFrame jf = new JFrame();

        jf.setTitle("考勤查询");
        jf.setSize(400, 300);
        jf.setDefaultCloseOperation(3);
        jf.setLocationRelativeTo(null);
        jf.setAlwaysOnTop(true);
        jf.setLayout(null);

        //显示考勤日期的文本
        JLabel dateLable = new JLabel("考勤日期");
        dateLable.setBounds(50, 20, 100, 20);
        jf.add(dateLable);

        //显示开始时间文本
        JLabel startDateLable = new JLabel("开始时间");
        startDateLable.setBounds(50, 70, 100, 20);
        jf.add(startDateLable);

        DateChooser dateChooser1 = DateChooser.getInstance("yyyy/MM/dd");
        DateChooser dateChooser2 = DateChooser.getInstance("yyyy/MM/dd");
        //开始时间输入框
        JTextField startDateField = new JTextField();
        startDateField.setBounds(50, 100, 100, 20);
        dateChooser1.register(startDateField);
        jf.add(startDateField);

        //显示结束时间文本
        JLabel endDateLable = new JLabel("结束时间");
        endDateLable.setBounds(250, 70, 100, 20);
        jf.add(endDateLable);

        //结束时间输入框
        JTextField endDateField = new JTextField();
        endDateField.setBounds(250, 100, 100, 20);
        dateChooser2.register(endDateField);
        jf.add(endDateField);

        //确定按钮
        JButton confirmButton = new JButton("确定");
        confirmButton.setBounds(250, 180, 60, 20);
        jf.add(confirmButton);

        confirmButton.addActionListener(new ActionListener() {
            @Override
            public void actionPerformed(ActionEvent e) {
                SimpleDateFormat sdf = new SimpleDateFormat("yyyy/MM/dd");

                //获取开始时间和结束时间的字符串
                String startDateString = startDateField.getText();
                String endDateString = endDateField.getText();

                try {
                    Date startDate = sdf.parse(startDateString);
                    Date endDate = sdf.parse(endDateString);

                    JOptionPane.showMessageDialog(jf,startDate+"\n"+endDate);
                } catch (ParseException ex) {
                    ex.printStackTrace();
                }
            }
        });

        jf.setVisible(true);
    }
}
12345678910111213141516171819202122232425262728293031323334353637383940414243444546474849505152535455565758596061626364656667686970717273747576777879
```

这里我们仅仅是演示了考勤查询的日期数据处理，将来呢，我们就可以根据这两个日期数据到考勤查询系统中去查询考勤信息了。

## 结尾：

![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/d3fd284e254d4469a2363c79d2d7abdf.gif#pic_center)

> 这篇文章就到这里了也算结束了，学完这些，基础知识也算全部学完了，大厦之成，非一木之材也；大海之阔，非一流之归也。感谢大家观看本文

![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/b09e988f928a4e0eaabcc069217b6030.png#pic_center)

微信名片

打赏作者

¥1 ¥2 ¥4 ¥6 ¥10 ¥20

扫码支付： ¥1

获取中

扫码支付

您的余额不足，请更换扫码支付或 [充值](https://i.csdn.net/#/wallet/balance/recharge?utm_source=RewardVip)

打赏作者

实付 元

[使用余额支付](https://blog.csdn.net/m0_63815035/article/details/)

点击重新获取

扫码支付

钱包余额 0

抵扣说明：

1.余额是钱包充值的虚拟货币，按照1:1的比例进行支付金额的抵扣。  
2.余额无法直接购买下载，可以购买VIP、付费专栏及课程。

[余额充值](https://i.csdn.net/#/wallet/balance/recharge)

举报

 [![](https://csdnimg.cn/release/blogv2/dist/pc/img/toolbar/Group.png) 点击体验  
DeepSeekR1满血版](https://ai.csdn.net/?utm_source=cknow_pc_blogdetail&spm=1001.2101.3001.10583) ![程序员都在用的中文IT技术交流社区](https://g.csdnimg.cn/side-toolbar/3.6/images/qr_app.png)

程序员都在用的中文IT技术交流社区

![专业的中文 IT 技术社区，与千万技术人共成长](https://g.csdnimg.cn/side-toolbar/3.6/images/qr_wechat.png)

专业的中文 IT 技术社区，与千万技术人共成长

![关注【CSDN】视频号，行业资讯、技术分享精彩不断，直播好礼送不停！](https://g.csdnimg.cn/side-toolbar/3.6/images/qr_video.png)

关注【CSDN】视频号，行业资讯、技术分享精彩不断，直播好礼送不停！

客服 返回顶部

微信名片

![](https://img-blog.csdnimg.cn/cb493c3fb7434b76bc131f177a02a780.jpeg) 微信 ID：Yangxs5820 微信扫码添加好友或搜索 ID

复制微信 ID

![](https://i-blog.csdnimg.cn/direct/cf41e32d3b3649ce9a543afd4d31abba.gif#pic_center) ![](https://i-blog.csdnimg.cn/direct/70ea780b77344481b63611d5663fb56c.png) ![](https://i-blog.csdnimg.cn/direct/2708655af1894c1db7be02326adb9074.png) ![](https://i-blog.csdnimg.cn/direct/585d718cc9f8419285f96b385481ba2f.png) ![](https://i-blog.csdnimg.cn/direct/d781f829d3d54c50afca125666fd6779.png) ![](https://i-blog.csdnimg.cn/direct/fbc764e6249b4bf3a0c24ddec32cdc76.png) ![](https://i-blog.csdnimg.cn/direct/7ab4eb6921494237ac1dd4c1b352c899.png) ![](https://i-blog.csdnimg.cn/direct/7a830c3e40be471b830c538243200541.png) ![](https://i-blog.csdnimg.cn/direct/ab5dcdfc403b4b1aaa420a0b4760e331.png) ![](https://i-blog.csdnimg.cn/direct/da4dec53695a4145af6f980950178e55.png) ![](https://i-blog.csdnimg.cn/direct/3a640c336d794ac2831e885a31de4608.png) ![](https://i-blog.csdnimg.cn/direct/00e2f528936d421d82e1f24fbe8dc663.png) ![](https://i-blog.csdnimg.cn/direct/7d30150da4bf42749a74030305e7fa76.png) ![](https://i-blog.csdnimg.cn/direct/6a23b5b00bce4fc7907b6480d439fc08.png) ![](https://i-blog.csdnimg.cn/direct/52e28143b5c44ea08fb4e0c9aceb55cd.png) ![](https://i-blog.csdnimg.cn/direct/61eb6ed734c94d59bc461bb46f86161b.png) ![](https://i-blog.csdnimg.cn/direct/23dfd2e933ba4f7fa7a1add95591b159.png) ![](https://i-blog.csdnimg.cn/direct/6cb3448e7909462cb832b08584e87bc5.png) ![](https://i-blog.csdnimg.cn/direct/8e2dbe29607b4ad580f940221dd59c74.png) ![](https://i-blog.csdnimg.cn/direct/ea36d9be20dd41c097facea1a3b15223.png) ![](https://i-blog.csdnimg.cn/direct/195d4496256f43a497bd70dba278707e.png) ![](https://i-blog.csdnimg.cn/direct/ba8660ff265b4217a41289b278bc1f04.png) ![](https://i-blog.csdnimg.cn/direct/bfc740d7789b4a1a85330f15f7011df0.png) ![](https://i-blog.csdnimg.cn/direct/c60d267814fc4c2f8d98180aecf2b1c8.png) ![](https://i-blog.csdnimg.cn/direct/0571eea10eeb4a49bcaa110f463c3c85.png) ![](https://i-blog.csdnimg.cn/direct/daec5dbbd7c0452e9a2080080761d05e.png) ![](https://i-blog.csdnimg.cn/direct/391c96b3034447648901b8f44658deb6.png) ![](https://i-blog.csdnimg.cn/direct/fbd295363b924e4a8565c4678b11766f.png) ![](https://i-blog.csdnimg.cn/direct/9a570e589adc4d08b6b8bdd0268b6272.png) ![](https://i-blog.csdnimg.cn/direct/b73586f985e54646b124dbdd90b0e300.png) ![](https://i-blog.csdnimg.cn/direct/d48084f67c9146b28f9772a920d216d9.png) ![](https://i-blog.csdnimg.cn/direct/76579922ba4b4b5695384a9b9ea059e3.png) ![](https://i-blog.csdnimg.cn/direct/0c61f5ebe08c4f8099d1193f74068365.png) ![](https://i-blog.csdnimg.cn/direct/67c6662f943b44caaeea9f3a88898930.png) ![](https://i-blog.csdnimg.cn/direct/05620bde65b443f6afdfad7e228f350e.png) ![](https://i-blog.csdnimg.cn/direct/282c77d6405a42cd8241c26c258f1230.png) ![](https://i-blog.csdnimg.cn/direct/22538fffaebd44fbb8863d07c3d5a9fb.png) ![](https://i-blog.csdnimg.cn/direct/ccf4cc56b3194dc78f5fac4f45e8f798.png) ![](https://i-blog.csdnimg.cn/direct/c99afe70d51e420bb46465bf5c2e0dfa.png) ![](https://i-blog.csdnimg.cn/direct/e250ae519712438ca06ea72ac5056fd9.png) ![](https://i-blog.csdnimg.cn/direct/384686c6d76f4f9896a1fd478ff9d635.png) ![](https://i-blog.csdnimg.cn/direct/92292997fa6e4cb08ab6a49f069749b7.png) ![](https://i-blog.csdnimg.cn/direct/e8ebb95181a943cb87571a8ad0d64ceb.png) ![](https://i-blog.csdnimg.cn/direct/fa2e64cef1784f058c9fecf052cbfe3b.png) ![](https://i-blog.csdnimg.cn/direct/a2f5af805f814ef3acaed9f8f05c5b2d.png) ![](https://i-blog.csdnimg.cn/direct/26747ae54873416ead41767b7055c6e1.png) ![](https://i-blog.csdnimg.cn/direct/bc85fd401e584c9fbaad8dffc3087b00.png) ![](https://i-blog.csdnimg.cn/direct/c517511673644e758e71129d813500d4.png) ![](https://i-blog.csdnimg.cn/direct/816d8308e0284ceb92783a8158c83450.png) ![](https://i-blog.csdnimg.cn/direct/36bcd536a4b0475fb28b6a040464180d.png) ![](https://i-blog.csdnimg.cn/direct/f2ef184f4e1e4e329c40607ecfbd7902.png) ![](https://i-blog.csdnimg.cn/direct/451932ef115d4ba680dbd2318bde4321.png) ![](https://i-blog.csdnimg.cn/direct/bdb37521627d4cb181d4552fafed0398.png) ![](https://i-blog.csdnimg.cn/direct/e9e5e3ca6204475bb1da8af58c1b22b2.png) ![](https://i-blog.csdnimg.cn/direct/186a04f36b4f4afea7d5df46c7b5ce49.png) ![](https://i-blog.csdnimg.cn/direct/25ac9e7f9656481094b4393fcee849a4.png) ![](https://i-blog.csdnimg.cn/direct/be9250a29b564a1ba276dd3bbbd51628.png) ![](https://i-blog.csdnimg.cn/direct/28d4e8bb67c54f728b9d888a3ee14d18.png) ![](https://i-blog.csdnimg.cn/direct/1a2da322c29d45b38be1d5cd668af610.png) ![](https://i-blog.csdnimg.cn/direct/d86eec8a1fc54889b91322f0aa017851.png) ![](https://i-blog.csdnimg.cn/direct/93b2a55b6f8a4466afa31a384bcec418.png) ![](https://i-blog.csdnimg.cn/direct/5f648f6799894e9d8549d731c797084b.png) ![](https://i-blog.csdnimg.cn/direct/47c88a9dd1194f77b3f122f2c075b5bf.png) ![](https://i-blog.csdnimg.cn/direct/46f8768491064b9183f3a3ec1d107fa4.png) ![](https://i-blog.csdnimg.cn/direct/4ae549036e7b40fda9d29fd7f9f801f3.png) ![](https://i-blog.csdnimg.cn/direct/69669b46d669441da08773481afdb43a.png) ![](https://i-blog.csdnimg.cn/direct/4adfc27db8e047348bcbb8da13ee1b48.png) ![](https://i-blog.csdnimg.cn/direct/33c294c7695c4b47a4ad86e5d781feef.png) ![](https://i-blog.csdnimg.cn/direct/1b74f423a02c475ab878a1e2a2dbabb3.png) ![](https://i-blog.csdnimg.cn/direct/0eba5043a8f04c0591fe0839bb99de08.png) ![](https://i-blog.csdnimg.cn/direct/c8d1aa18d72d4d20adc145af49858b9a.png) ![](https://i-blog.csdnimg.cn/direct/d003df6c1e9743d7b4ea2cbc381933a9.png) ![](https://i-blog.csdnimg.cn/direct/49671d9f866a48c2addfb4b098e7c147.png) ![](https://i-blog.csdnimg.cn/direct/a0ca63e856944692a665dbf002955fae.png) ![](https://i-blog.csdnimg.cn/direct/cbda38e86ece465e82f94924f73a4b91.png) ![](https://i-blog.csdnimg.cn/direct/c3aa0a4e290d444892ba6d154c382e9d.png) ![](https://i-blog.csdnimg.cn/direct/684f6445e6a54d6f9aefcc47b5dfaaff.png) ![](https://i-blog.csdnimg.cn/direct/189925a78e0e412ab6a3feec8683f785.png) ![](https://i-blog.csdnimg.cn/direct/46efaa76d33c492d94a3942a98495323.png) ![](https://i-blog.csdnimg.cn/direct/d2bb9532d5704be897827eb6bf74c207.png) ![](https://i-blog.csdnimg.cn/direct/e8929d5a993946c3a4a33da3bdeeaeb4.png) ![](https://i-blog.csdnimg.cn/direct/a2abfb2453224a0ea0b78ed35f2a8426.png) ![](https://i-blog.csdnimg.cn/direct/a4911e6872fc4671837d18a19d267790.png) ![](https://i-blog.csdnimg.cn/direct/a3df9e257b6c4e6a97344e8d9f82d11d.png) ![](https://i-blog.csdnimg.cn/direct/7eb01f78f8084b78939bbede8b5d9123.png) ![](https://i-blog.csdnimg.cn/direct/1055e439868a41748e5c864f20a6cef1.png) ![](https://i-blog.csdnimg.cn/direct/627d016c7745494e9b38036dfc36b10b.png) ![](https://i-blog.csdnimg.cn/direct/b88fa74fd0d947028195ca63cfc28eb3.png) ![](https://i-blog.csdnimg.cn/direct/0b55fc31c5a7408a9fcc60bbd7f180d9.png) ![](https://i-blog.csdnimg.cn/direct/8486389cb3674587afa6a0dc70381093.png) ![](https://i-blog.csdnimg.cn/direct/d03c6ef3bdd14add96ca04444fb06634.png) ![](https://i-blog.csdnimg.cn/direct/17742f5eae0149f2bd0519c092646b3e.png) ![](https://i-blog.csdnimg.cn/direct/2afcacf108ef44288d00c6de0dd5ebf3.png) ![](https://i-blog.csdnimg.cn/direct/a6cc8b842984479da7bb94e86437cccf.png) ![](https://i-blog.csdnimg.cn/direct/9b590ca893824e4b8594e7bb1108edc9.png) ![](https://i-blog.csdnimg.cn/direct/22784f31ed924e4b8f6acf8f6a663621.png) ![](https://i-blog.csdnimg.cn/direct/3581cf6e4be04d2bb21dcffc7443d4a9.png) ![](https://i-blog.csdnimg.cn/direct/fc4baaf004774e5e9e8f116b09690230.png) ![](https://i-blog.csdnimg.cn/direct/e5af01a6ab4142c4bbf39657a63d1c88.png) ![](https://i-blog.csdnimg.cn/direct/8590dd76552747d0860746a58c359789.png) ![](https://i-blog.csdnimg.cn/direct/4544cbf10de34163bace45f8f854171f.png) ![](https://i-blog.csdnimg.cn/direct/e2ddec984cba4c9d8d65c97757b2e85c.png) ![](https://i-blog.csdnimg.cn/direct/ff7b2372af5449788a288edfabd93d90.png) ![](https://i-blog.csdnimg.cn/direct/c3d7daeee83c44ea99e6e77655f655df.png) ![](https://i-blog.csdnimg.cn/blog_migrate/e6cacf3546514978dce7f8ccda603406.png) ![](https://i-blog.csdnimg.cn/direct/4eb007e095974b6db6751fe05e559a66.png) ![](https://i-blog.csdnimg.cn/direct/4852352b047b4cd098ae559b03d9b99e.png) ![](https://i-blog.csdnimg.cn/direct/c986714009964f39b442b24eed8546fc.png) ![](https://i-blog.csdnimg.cn/direct/b42d93240a474bfb97accd817f70fe23.png) ![](https://i-blog.csdnimg.cn/direct/38f69b279abc44e884ec85dca2b4a50e.png) ![](https://i-blog.csdnimg.cn/direct/4b5fe160a65b4b1ea1cb703896e35feb.png) ![](https://i-blog.csdnimg.cn/direct/523d7e9f2d33449ea7621b7eea1c7c08.png) ![](https://i-blog.csdnimg.cn/direct/d937e37cfe5747d3858c627e741abeab.png) ![](https://i-blog.csdnimg.cn/direct/acfcdbb7f953490ea0cfe77d9cf1a1ee.png) ![](https://i-blog.csdnimg.cn/direct/6f86d5411923462bab88c306e5c63770.png) ![](https://i-blog.csdnimg.cn/direct/1d46409b6d5e49d1a1ad1e7a6ceaa14d.png) ![](https://i-blog.csdnimg.cn/direct/475b5f28d8d84350bc880bb3c239ada8.png) ![](https://i-blog.csdnimg.cn/direct/89d74d7ccc8d46dd9769b721ee667c51.png) ![](https://i-blog.csdnimg.cn/direct/975b22a09ba7463c8a0deae7e1a226d6.png) ![](https://i-blog.csdnimg.cn/direct/9d0a004972e147058a0c5ac64c648c45.png) ![](https://i-blog.csdnimg.cn/direct/64b8258f12e543a3b6080524d10dc9d4.png) ![](https://i-blog.csdnimg.cn/direct/2f4b095f2a044fbaa0169411aaa88381.png) ![](https://i-blog.csdnimg.cn/direct/d18972c8a510496a8942b337f536f671.png) ![](https://i-blog.csdnimg.cn/direct/dcd669e20a4746408c9be10b572ca787.png) ![](https://i-blog.csdnimg.cn/direct/025a46f71378475caa7696bcf671091e.png) ![](https://i-blog.csdnimg.cn/direct/1f74541e999a4f4a8bb4af6778e12c14.png) ![](https://i-blog.csdnimg.cn/direct/fb3d7863e62643fe91f787bd6fc72ba7.png) ![](https://i-blog.csdnimg.cn/direct/bb32cf9a90484c3e82c9f0cac236a6f2.png) ![](https://i-blog.csdnimg.cn/direct/303dc035c2e4465b8a9c11840020fc29.png) ![](https://i-blog.csdnimg.cn/direct/faa2d333b5b842ff9e1093b79a719715.png) ![](https://i-blog.csdnimg.cn/direct/b390519fdd54418298cd200607e09b16.png) ![](https://i-blog.csdnimg.cn/direct/51d8533f1f9545ce9fb8de54ea59f81f.png) ![](https://i-blog.csdnimg.cn/direct/ac7d4fedbdb5408caa208f71da42ac16.png) ![](https://i-blog.csdnimg.cn/direct/4c0d9d6be3614c3c926459ac04b1aa56.png) ![](https://i-blog.csdnimg.cn/direct/5fca53f4c96f4cea8a29f85d67ff950b.png) ![](https://i-blog.csdnimg.cn/direct/30923d04ad6144ae93a74bc4592bebc6.png) ![](https://i-blog.csdnimg.cn/direct/ca4eb26a58664be2a136e1f4265e4c4d.png) ![](https://i-blog.csdnimg.cn/direct/b772ed3b373440158c975031301addfb.png) ![](https://i-blog.csdnimg.cn/direct/1e2add470ee840559d9a704a1b1baa86.png) ![](https://i-blog.csdnimg.cn/direct/38035234cc8d4239acd64889efe5b136.png) ![](https://i-blog.csdnimg.cn/direct/352daa437ade433ab13b447e77f48c54.png) ![](https://i-blog.csdnimg.cn/direct/9bc097eedcb1448ba5200af8149341bb.png) ![](https://i-blog.csdnimg.cn/direct/3040d58b86db4e478eca4c9ea142320c.png) ![](https://i-blog.csdnimg.cn/direct/d8c552e7a31845ce9e299e67554188f4.png) ![](https://i-blog.csdnimg.cn/direct/dfa210cd399641f49959ddfd1cf3771d.png) ![](https://i-blog.csdnimg.cn/direct/289c08a3f9e8446d9b5c1e750be96a24.png) ![](https://i-blog.csdnimg.cn/direct/3d66d148cde34b06a35eba4893212de3.png) ![](https://i-blog.csdnimg.cn/direct/b90bf6d00dfc4708b0365bfa21005351.png) ![](https://i-blog.csdnimg.cn/direct/dc1a601b5a844440b05da4ab49a6266f.png) ![](https://i-blog.csdnimg.cn/direct/b5a5f20862aa49d583ba3a8a83381023.png) ![](https://i-blog.csdnimg.cn/direct/8f872f0b6d2d473e829bdc815cd327a1.png) ![](https://i-blog.csdnimg.cn/direct/53ecbc01812e4b5ca118a47daeeaa16a.png) ![](https://i-blog.csdnimg.cn/direct/80ec39cb0ec149c594af5d43238e56a7.png) ![](https://i-blog.csdnimg.cn/direct/49af25367f17411686d557292c0ff084.png) ![](https://i-blog.csdnimg.cn/direct/e8afa304061a4bd3b7ee932502f861d4.png) ![](https://i-blog.csdnimg.cn/direct/46f7d8770cc74424ae8284cf64d508bf.png) ![](https://i-blog.csdnimg.cn/direct/4e9eb8c5a2ff40a38824a8bda1b61e34.png) ![](https://i-blog.csdnimg.cn/direct/024d2a3d01d546f481c9c8cb9939ed45.png) ![](https://i-blog.csdnimg.cn/direct/4439352fcff44e9a9e1b99cc2c8193ac.png) ![](https://i-blog.csdnimg.cn/direct/b49914f5c21f4a29aedf79d6eb462d1d.png) ![](https://i-blog.csdnimg.cn/direct/be60a8c57494457abbaebe06b9af4a17.png) ![](https://i-blog.csdnimg.cn/direct/003390ac7c6f4a9c9b10c1be6b2f6646.png) ![](https://i-blog.csdnimg.cn/direct/cedf8f64db8a4bd2b92013d688e5ee31.png) ![](https://i-blog.csdnimg.cn/direct/b664c5c8d7fa4f0e951254014b75e947.png) ![](https://i-blog.csdnimg.cn/direct/e242347b5e84491ea22e410985bc1983.png) ![](https://i-blog.csdnimg.cn/direct/c0eff96189764955a25449b9fa6e90cc.png) ![](https://i-blog.csdnimg.cn/direct/9d943cf65e6d4daa8847f1637742820c.png) ![](https://i-blog.csdnimg.cn/direct/7f8eb775b4804927b21a0d04e868ed6f.png) ![](https://i-blog.csdnimg.cn/direct/0342baa8d92548f084cadbc1b0da8c0b.png) ![](https://i-blog.csdnimg.cn/direct/920a0f2552ac489c8f8cfcbb0a430d06.png) ![](https://i-blog.csdnimg.cn/direct/71320e68348e450aaf3320969c721ec8.png) ![](https://i-blog.csdnimg.cn/direct/1553bfc905364f01ae953e62bad4c6af.png) ![](https://i-blog.csdnimg.cn/direct/03a8f472181447ab8e7c33671a20c29a.png) ![](https://i-blog.csdnimg.cn/direct/243ff0f66ad74ccb9cd7fa65fbebcaf4.png) ![](https://i-blog.csdnimg.cn/direct/65ac9147f95c46fdb4a88f63fcd46ed8.png) ![](https://i-blog.csdnimg.cn/direct/b6d172fe86d64b17a64348af8aa368f0.png) ![](https://i-blog.csdnimg.cn/direct/f84c4606ada9411d914b47bd7eb37a1d.png) ![](https://i-blog.csdnimg.cn/direct/f0e6f3a94270403caf212bdd77d5da2f.png) ![](https://i-blog.csdnimg.cn/direct/5f0382923ffd416d8db09ed3d4453235.png) ![](https://i-blog.csdnimg.cn/direct/bab28e94e206436fb56cbb78e0f38ae7.png) ![](https://i-blog.csdnimg.cn/direct/d006d25758644154a1f1c68ca94fa462.png) ![](https://i-blog.csdnimg.cn/direct/4765cf79a9e54d7387a76890973b8bc3.png) ![](https://i-blog.csdnimg.cn/direct/5c78cc437f2b4469a4c2ccc580182be4.png) ![](https://i-blog.csdnimg.cn/direct/20dc66cd3ea34010921ac10f783d4125.png) ![](https://i-blog.csdnimg.cn/direct/1a8a48b62c2347c98919b9039e62fea5.png) ![](https://i-blog.csdnimg.cn/direct/393d26275de349e09da9458378a75f3c.png) ![](https://i-blog.csdnimg.cn/direct/91a3c78156454752ab9420e81dbece20.png) ![](https://i-blog.csdnimg.cn/direct/557dfee01f204073bce725bf70faed76.png) ![](https://i-blog.csdnimg.cn/direct/7c2bc37a756a49d5a68ff408c0b46395.png) ![](https://i-blog.csdnimg.cn/direct/8a73ba6a8a00426a82f6ff0a9f962c63.png) ![](https://i-blog.csdnimg.cn/direct/2d417a536e7645c8a77843aa9d5e01ee.png) ![](https://i-blog.csdnimg.cn/direct/dffa8b3a3e4741c1af4c3d99ef2a86b8.png) ![](https://i-blog.csdnimg.cn/direct/610b700dd64449809230715004e43cb6.png) ![](https://i-blog.csdnimg.cn/direct/0d80b82e4b964d5782107322ea9927ed.png) ![](https://i-blog.csdnimg.cn/direct/f0b3bcaf657f43deb69a1e7feb9d9f70.png) ![](https://i-blog.csdnimg.cn/direct/17d832ee34b6474ebd01441d5d6a7677.png) ![](https://i-blog.csdnimg.cn/direct/1830a54922fb4602bf13b24b0199262a.png) ![](https://i-blog.csdnimg.cn/direct/d3a034a6f2f94e679376dcea5b4f34e6.png) ![](https://i-blog.csdnimg.cn/direct/48c54fac642045bd816dbb1cf9ffe9eb.png) ![](https://i-blog.csdnimg.cn/direct/63ea3647e87f4aa9942a6b8db93538dd.png) ![](https://i-blog.csdnimg.cn/direct/3b8c59ce5b2d473d845cac6607000e1b.png) ![](https://i-blog.csdnimg.cn/direct/59bb4cafb72e45e498ae947db06db3f4.png) ![](https://i-blog.csdnimg.cn/direct/e89aa38fbf34408c86214caef7f946e1.png) ![](https://i-blog.csdnimg.cn/direct/51b217b033e74808aa5609a9a410c601.png) ![](https://i-blog.csdnimg.cn/direct/3cb980a8dc81476098b0458367f6106b.png) ![](https://i-blog.csdnimg.cn/direct/a2ed5ecdffc34420a87521145659a62b.png) ![](https://i-blog.csdnimg.cn/direct/7b924f49cf1445c5b8c043704fee9b3b.png) ![](https://i-blog.csdnimg.cn/direct/57dcf7c582b041b882a353e43c10eb01.png) ![](https://i-blog.csdnimg.cn/direct/34091b5cdb424b0c99aeca7d99a40fc3.png) ![](https://i-blog.csdnimg.cn/direct/106a4ac7c9be45c49db749a009d85a0f.png) ![](https://i-blog.csdnimg.cn/direct/3f8d078fd03748f2add3703e643a196b.png) ![](https://i-blog.csdnimg.cn/direct/a67b7e113310485cb531e5faa2c9c8c1.png) ![](https://i-blog.csdnimg.cn/direct/010f84b4f3d440ee936dfd07d4dc2d9e.png) ![](https://i-blog.csdnimg.cn/direct/674182f45d4040ddbf5c8844a908d330.png) ![](https://i-blog.csdnimg.cn/direct/df90a1ee288b4b14a8f00ce699bcb355.png) ![](https://i-blog.csdnimg.cn/direct/aafbaa2ec0a84759b2ddc815c9323bbd.png) ![](https://i-blog.csdnimg.cn/direct/a4c51638b9fc4df582c45ddd739ac983.png) ![](https://i-blog.csdnimg.cn/direct/77392ce16647416da8dc5ab7b452ba64.png) ![](https://i-blog.csdnimg.cn/direct/b3020d705ebf44f9af9fd3ab4b4daac4.png) ![](https://i-blog.csdnimg.cn/direct/9a1f057445ef4dde82e4ee25a831a454.png) ![](https://i-blog.csdnimg.cn/direct/75874a08616e4930ac935e637f0f7ff5.png) ![](https://i-blog.csdnimg.cn/direct/eb4fc209e6544e648826387349fc2e90.png) ![](https://i-blog.csdnimg.cn/direct/80b5102397e346cab33572e958a6e40e.png) ![](https://i-blog.csdnimg.cn/direct/afe11e16561e42aab4ab05f3225fbb5b.png) ![](https://i-blog.csdnimg.cn/direct/a2b2a7dab565401cbda464d1f1d8f9bf.png) ![](https://i-blog.csdnimg.cn/direct/a0e4cb66fc034df9b8dd632b3e147b19.png) ![](https://i-blog.csdnimg.cn/direct/a9b76f1911cf4e5b93fdc4afc0c78bc7.png) ![](https://i-blog.csdnimg.cn/direct/771931894600436cb837049cf6813da6.png) ![](https://i-blog.csdnimg.cn/direct/c087ace72b5c4e0191bcd859f19275df.png) ![](https://i-blog.csdnimg.cn/direct/21bb5c627b33437ba5bfe827b32e0df1.png) ![](https://i-blog.csdnimg.cn/direct/9be96c152a3241a4a038f679801716da.png) ![](https://i-blog.csdnimg.cn/direct/15598b5ed3c544c0952f4c5bf39854b9.png) ![](https://i-blog.csdnimg.cn/direct/a549715fdf334f91871cd5d64fd9b39e.png) ![](https://i-blog.csdnimg.cn/direct/dc6eb65b2ed0482f99663eec93819c21.png) ![](https://i-blog.csdnimg.cn/direct/d3fd284e254d4469a2363c79d2d7abdf.gif#pic_center) ![](https://i-blog.csdnimg.cn/direct/b09e988f928a4e0eaabcc069217b6030.png#pic_center)