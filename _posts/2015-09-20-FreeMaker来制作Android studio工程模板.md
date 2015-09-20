---
layout: post
title: 利用FreeMaker来制作Android studio项目工程模板，定制自己的项目框架。
description: 自定义Android studio项目工程和文件模板
keywords: Android
categories : [Android]
tags : [Android]
---

利用FreeMaker来制作Android studio项目工程模板，定制自己的项目框架。

---


* 模板文件位置 

  模板位置：在Android Studio安装目录下\plugins\android\lib\templates 常用的集中在activities和other里面。
   ![](/images/androidTemplates.png)

* 如何使用: 

  我们只需要复制一份原有已经存在的模板，比如activities文件夹里面我们经常用的BlankActivity文件夹，复制粘贴，修改文件夹名字，比如:MyBlankActivity。 目前感觉没有需要使用FreeMarker插件之类的必要。直接使用UE即可。

* 文件组织结构

    * root 文件夹，里面放的就是代码文件，我们需要把生成到项目里的java、xml、资源...文件放进这里。
    * globals.xml.ftl 放的全局变量，这些全局变量其它模板文件都可能引用到。
    * recipe.xml.ftl freeMaker根据这个文件去生成最终的项目文件。比如:instantiate标签就是将root文件夹某个文件模板生成到工程中目标文件夹。template.xml 包含了：元数据、名字、描述、类别和用户可见参数。同时也指出了配置文件recipe.xml.ftl、全局变量文件global.xml.ftl


` 需要注意的是文件都按照utf-8保存，这样子才能在android studio问不会中文显示为乱码。 UE如果看不到文件浏览目录，可以重新打开：点击[视图]--[视图/列表]--[文件树视图]就可以了。`

---
参考:[Android记录自定义ADT模板](http://my.oschina.net/xesam/blog/143985)
