---
title: 关于 MarkDown 语法使用回顾
tags:
  - Blog
  - MarkDown
categories:
  - 写作
keywords: 'markdown, 个人博客'
cover: 'https://cdn.jsdelivr.net/gh/Caczhtus/Caczhtus-imgs/images/article/1.jpg'
toc: true
abbrlink: 0x01
---

# 前言
MarkDown 是一种文本标记语言，它是一种能够渲染你所写的文本的工具，前提是你按该语言约定的方式填上相应标签。如果你有前端开发的基础，这种语言其实可以理解成已经链接好 CSS 的 HTML 代码，你只需编写内容以及设置对应样式即可。

为什么写这篇文章？本人之前是在 CSDN 平台写博客，使用过富文本编辑器，后来觉得当时 MarkDwon 渲染出来的代码块比较好看，于是就开始使用 MarkDown 了。但由于现在自己搭的博客不但支持 MarkDown 语法，还拓展了许多标签外挂，为了防止将来遗忘以及自己便于回顾等原因，于是记录此文。其中，LaTeX公式不在本文进行介绍。

---
# 文字
这部分是关于文字方面的标记，例如：标题、加粗、换色、删除线、代码块等。

## 标题
最前面有个#紧接着一个空格，之后就可以写标题内容。n个#代表n级标题。
例如：

```
# 一级标题
## 二级标题
### 三级标题
#### 四级标题
```

## 内容加粗
在要加粗的文本两侧分别打上**两个**星号 * 或者下划线 _ 表示加粗。
例如：
> **加粗的文本**

## 内容斜体
在要进行斜体的文本两侧分别打上**一个**下划线 _ 或者是星号 * 表示斜体。
例如：
> *斜体的文本*

## 删除线
在要进行划删除线的文本两侧分别打上**两个**波浪线 ~ 表示划删除线。
例如：
> ~~划删除线的文本~~

## 下标号
在要进行打下标的文本两侧分别打上**一个**波浪线 ~ 表示下标。(Ps：这个方式 CSDN 可以完成，不过有的地方不支持)
例如：
> H~2~O

## 上标号
在要进行打上标的文本两侧分别打上**一个**上尖括号 ^  表示上标。(Ps：这个方式 CSDN 可以完成，不过有的地方不支持)
例如：
> 2^2^

## 引用文本
在最前面打上**一个**右尖括号 > 和一个空格表示引用文本，连续的符号越多表示越往右打 Tab 。
例如：
> 一个
> > 两个
> >
> > > 三个

## 标记文本
出现黄色底纹的文本。在文本两侧分别打上**两个**等号 = 和一个空格表示标记文本。(Ps：这个方式 CSDN 可以完成，不过有的地方不支持)
例如：
> ==代标记文本==

## 链接
使用 HTML 的 a 标签或 MarkDown 语法。
例如：
```html
<a href="https://caczhtus.github.io/"></a>
```
或者
```
[link](https://caczhtus.github.io/).
```

## 颜色文本
使用 HTML 的 font 标签。
例如：
```html
<font color="red">这里是想改变颜色的文本</font>
```

## 换行
有时候 MarkDown 无法解析多个换行，此时用 HTML 的 br 标签可以达到多次换行的效果。

## 注脚
CSDN 平台支持。

语法：

```
[^txt]
[^txt]: 前言
```
例如：

> [^mark]
>
> [^mark]: 前言

## 待办事项
注意的点是待办事项括号中有个空格，而已办事项括号中有个 x 。

语法：

```
- [x] A
- [ ] B
- [ ] C
```
例如：

- [x] A
- [ ] B
- [ ] C

## 代码片
把代码上下行分别用三个 ` 号包裹。
例如：
```C++
#include <bits/stdc++.h>
using namespace std;
int main() {
  cout << "Hello, MarkDown!" << endl;
  return 0;
}
```


## 待补充
未完待续

---
# 图表
这部分是关于图标方面的标记，例如：表格、列表、甘特图、UML图、Mermaid流程图、序列图等。

## 表格
包括表头、和内部文字的对齐方式，注意冒号再哪边表示向哪边对齐。默认居中对齐。

语法

```
| item1 | item2 | item3 |
| :-- | --:| :--: |
| A | 1 | 2 |
| B | 3 | 4 |
| C | 5 | 6 |
```
例如：

| item1 | item2 | item3 |
| :-- | --:| :--: |
| A | 1 | 2 |
| B | 3 | 4 |
| C | 5 | 6 |

## 图片
插入默认大小的图片以居中的形式展现。
语法：
```
![描述](https://cdn.jsdelivr.net/gh/Caczhtus/Caczhtus-imgs/images/other/ic_1.jpg)
```
例如：
![描述](https://cdn.jsdelivr.net/gh/Caczhtus/Caczhtus-imgs/images/other/ic_1.jpg)

## 列表
### 有序列表
在首部添加数字以及一个点外加一个空格即可。
例如：
```
1. A
2. B
  3. b1
  4. b2
5. C
```
1. A
2. B
	3. b1
	4. b2
5. C
### 无序列表
在首部添加 - 以及一个点外加一个空格即可。
例如：
```
- A
- B
  - b1
  - b2
- C
```
- A
- B
  - b1
  - b2
- C

## 待补充
未完待续

---
# 其他
## 补充资料
1. [【简明版】有道云笔记Markdown指南](http://note.youdao.com/iyoudao/?p=2411)
2. [【进阶版】有道云笔记Markdown指南](http://note.youdao.com/iyoudao/?p=2445)
3. [Markdown指南](https://blog.csdn.net/u014653854/article/details/80723427?ops_request_misc=%257B%2522request%255Fid%2522%253A%2522159506320919195162517149%2522%252C%2522scm%2522%253A%252220140713.130102334..%2522%257D&request_id=159506320919195162517149&biz_id=0&utm_medium=distribute.pc_search_result.none-task-blog-2~blog~sobaiduend~default-3-80723427.pc_v2_rank_blog_v1&utm_term=markdown)
4. [CSDN Markdown首次使用教程（新版）](https://blog.csdn.net/Void_worker/article/details/83548492)

## 参考
1. [【简明版】有道云笔记Markdown指南](http://note.youdao.com/iyoudao/?p=2411)
2. [CSDN 平台 MarkDown 的帮助文档 ](https://www.csdn.net/)

---