---
layout: post
title: Android studio配置
description: Android studio提高效率的配置
keywords: Android
categories : [Android]
tags : [Android]
---

个人觉得比较能提高开发效率的配置:

---

- 主题修改：选择菜单栏“File--settings--apperance--theme”，主题选择Darcula
- 代码字体修改：选择菜单栏““File--settings--Editor--Colors&Fonts--Font”增大字体到18，同时也可修改“Console Font”字体到16。
- 添加文档悬浮提示：AS默认是没有API文档悬浮提示的，只有按住【Ctrl+Q】才会出现提示。设置如下“Editor--General--Other--Show quick doc on mouse move Delay(ms) 500”。
- 修改默认代码提示**大小写敏感**。设置如下“Editor--General--Code Completion--Case sensitive completion” 设置为None。
- 自动导入引用包。设置如下“Editor--General--Auto Import--"  
Optimize imports on the fly” 设置为TRUE。  
Add unambiguous imports on the fly” 设置为TRUE。
- 显示代码行数。设置如下“File--settings--apperance--show line numbers” 设置为TRUE。
- 禁止自动打开上次的工程。设置如下“Apperance & Behavior --System Settings-Reopen last project on startup” 设置为TRUE。
- 代码折叠 “Editor--General--Code Folding--”  
  "One-line menthods"   
  "Closures"  
  "Generic construct and method parameters"  
  设置为FALSE
- 修改注释位置， “Editor--General--Code Style--Java--Wrapping and Braces”   
Comment at first column  
Control statement in one line    
 设置为FALSE  
Braces placement  
下面都设置为 “Next Line”
" 'try' statement"  
'catch' on new line  
'finally' on new line  
设置为TURE
- 修改文件编码为UTF-8  
"Editor--file and Code Templates"    
  IDE Encodeing、Project Encoding、Default encoding for properties files都设置为**UTF-8**

---

参考:

[第一次使用Android Studio时你应该知道的一切配置](http://www.cnblogs.com/smyhvae/p/4390905.html)