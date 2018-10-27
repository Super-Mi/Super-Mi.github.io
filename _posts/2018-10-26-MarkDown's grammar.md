---
layout:     post
title:      "MarkDown语法"
subtitle:   "MarkDown's grammar"
author:     "Super-Mi"
header-img: "img/post-first-article.jpg"
header-mask: 0.3
catalog:    true
tags:
    - 笔记 
    - MarkDown
---

>在正式描述之前，先放个视频吧！


## 视频

<p align="center"> 
<video width="100%" height="100%" controls="controls">
  <source src="https://dn-shimo-attachment.qbox.me/kDRjMibHWjkE3Q3y/%E4%BB%80%E4%B9%88%E6%98%AF_markdown.MP4#t=10,650" type="video/mp4">
  <source src="视频/什么是_markdown.mp4" type="video/mp4">
Your browser does not support the video tag.
</video>
</p>

*视频来源:[youtube][i3]*


看完视频之后，相信你已经了解Markdown语法了。

如果还不懂......

~~多看两遍~~

那就往下看

## 图文
Markdown是一种极简的『标记语言』，将文本转为HTML，通常为我大码农所用。其不追求大而全，简洁至上，正所谓不求最贵，只求最好！

本文介绍Markdown基本语法，内容很少，一行语法一行示例，学会后可轻松写出高大上的文档，再也不需要各种编辑器去调文章格式。另外，网上有各平台下的Markdown工具可用，也有在线的，我直接使用sublime搞定，Markdown本来就是为了追求简洁，弄个工具岂不多此一举。

### 强调（粗体&斜体）
---
```html
星号与下划线都可以，单是斜体，双是粗体，符号可跨行，符号可加空格

**毫无疑问**

__毫无疑问__

*我做的馅饼
是全天下*
_最好吃的_
```
**毫无疑问**

__毫无疑问__

*我做的馅饼

是全天下*

_最好吃的_

### 分割线
---

```
三个或更多-_*，必须单独一行，可含空格

---
```

### 引用
---

```
翻译成html就是<blockquote></blockquote>，符号后的空格可不要

> 引用
```

>

```
内层符号前的空格必须要

>引用
 >>引用中的引用
```
>引用
 >>引用中的引用

### 大小标题（Atx方式）
---

```
# 一级标题
## 二级标题
### 三级标题
#### 四级标题
##### 五级标题
###### 六级标题
```

### 无序列表
---
```
符号之后的空格不能少，-+*效果一样，但不能混合使用，因混合是嵌套列表，内容可超长

- 无序列表
- 无序列表
- 无序列表
- 无序列表：我很长。我也很长！那比一比啊？比就比！我有这么长，你有我长吗？我有这么这么长！好吧，你赢了！
```
- 无序列表
- 无序列表
- 无序列表
- 无序列表：我很长。我也很长！那比一比啊？比就比！我有这么长，你有我长吗？我有这么这么长！好吧，你赢了！

```
符号之后的空格不能少，-+*效果一样，但不能混合使用，因混合是嵌套列表

+ 无序列表
+ 无序列表
+ 无序列表
```
+ 无序列表
+ 无序列表
+ 无序列表

```
符号之后的空格不能少，-+*效果一样，但不能混合使用，因混合是嵌套列表

* 无序列表
* 无序列表
* 无序列表
```
* 无序列表
* 无序列表
* 无序列表

### 有序列表
---
```
数字不能省略但可无序，点号之后的空格不能少

1. 有序列表
2. 有序列表
3. 有序列表
8. 有序列表
```
1. 有序列表
2. 有序列表
3. 有序列表
8. 有序列表

### 嵌套列表
---
```
-+*可循环使用，但符号之后的空格不能少，符号之前的空格也不能少

- 嵌套列表
 + 嵌套列表
 + 嵌套列表
  - 嵌套列表
   * 嵌套列表
- 嵌套列表
```
- 嵌套列表
 + 嵌套列表
 + 嵌套列表
   - 嵌套列表
     * 嵌套列表
- 嵌套列表

### 文字超链：Inline方式
---
```
Tooltips可省略

[Super-Mi](http://bruce-sha.github.io "Super-Mi的博客")
```
[Super-Mi](http://bruce-sha.github.io "Super-Mi的博客")

### 图片超链
---
```
比文字超链多个感叹号，Tooltips可省略，要设置大小只能借助HTML标记

![GitHub Mark](http://github.global.ssl.fastly.net/images/modules/logos_page/GitHub-Mark.png "GitHub Mark")
```

![GitHub Mark](http://github.global.ssl.fastly.net/images/modules/logos_page/GitHub-Mark.png "GitHub Mark")

### 索引超链：Reference方式
---
```
索引，1 2可以是任意字符

[Super-Mi][1]
![GitHub Octocat][2]

[1]:https://super-mi.github.io/
[2]:http://github.global.ssl.fastly.net/images/modules/logos_page/Octocat.png
```
[Super-Mi][1]
<br>
![GitHub Octocat][2]

### 自动链接
---
```
尖括号

<https://super-mi.github.io/>
<bu.ru@qq.com>
```
<https://super-mi.github.io/>

### 代码：行内代码
---
```
使用键盘上左上角数字1左边的按键，在行内代码左右两边均打上一个点即可。可以在第一行后指定编程语言，也可以不指定

val s = `hello Markdow`

println( s )
```

val s =`hello Markdow`

println( s )

### 代码：段落代码
---
```
使用键盘上左上角数字1左边的按键，在代码块前后均打上三个点即可。
可在第一行三个点右边写上语言的类型例如：

···html
val s = "hello Markdown"
println( s )
···
```
效果如下

```
val s = "hello Markdown"
println( s )

```
 
### 代码：段落代码
 ---
```
 可指定编程语言，『』代表左右大括号

『% codeblock [title] [lang:language] [url] [link text] %』
  code snippet
『% endcodeblock %』
 ```
 
### 注释
---

```
 用html的注释，好像只有这样？
<!-- 注释 -->
 ```
 
### 转义字符
---
```
 用html的注释，好像只有这样？
Markdown中的转义字符为\，转义的有：
\\ 反斜杠
\` 反引号
\* 星号
\_ 下划线
\{\} 大括号
\[\] 中括号
\(\) 小括号
\# 井号
\+ 加号
\- 减号
\. 英文句号
\! 感叹号
```
### 其它
--- 
```
 文本中可直接用html标签，但是要前后加上空行。
 
 ```
 
### one more thing：表格
---
```
Markdown的扩展语法，hexo不支持

|| *Year* || *Temperature (low)* || *Temperature (high)* ||
|| 1900 || -10 || 25 ||
|| 1910 || -15 || 30 ||
|| 1920 || -10 || 32 ||
```

|| *Year* || *Temperature (low)* || *Temperature (high)* ||
|| 1900 || -10 || 25 ||
|| 1910 || -15 || 30 ||
|| 1920 || -10 || 32 ||


### 结束语
---
 
 以上基本够用，更详尽的请[参考文献10][3]，另外Markdown+R可以干大事，请[参考文献7][4]。
 
 >[本文参考][5]

 <a href="#">
	<h3 align="center">返回顶部</h3></a>
 
[1]:https://super-mi.github.io/
[2]:http://github.global.ssl.fastly.net/images/modules/logos_page/Octocat.png
[3]:http://wowubuntu.com/markdown
[4]:http://jianshu.io/p/PpDNMG
[5]:http://ibruce.info/2013/11/26/markdown/
[i3]:https://www.youtube.com/watch?v=EigxHkpqJdA
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 