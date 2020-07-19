---
title: 【未完待续】关于 Hexo-ButterFly 主题的使用记录
tags:
  - Blog
  - Hexo-ButterFly
categories:
  - 写作
keywords: 'Hexo, 个人博客, 主题'
cover: 'https://cdn.jsdelivr.net/gh/Caczhtus/Caczhtus-imgs/images/article/2.jpg'
toc: true
abbrlink: 0x02
sticky: 10
---

# 前言
本文主要针对 butterfly 主题中除 MarkDown 语法外的特殊标签以及配置进行记录。

---
# 文件头
这部分是在博客根目录的source文件夹中每个 md 文件，也就是 markdown 文件中的一个文件头，通过这个文件可以对本文件进行单独配置。相当于如果你没有过多修改该位置的东西，那么默认是全局的熟悉，否则优先渲染你当前文件所配置的选项。

## Page Front-Matter
页面的文件头配置文件，区别于文章的部分，文章的文件存放在 \_Post 目录下。

| Type | Explanation | Example |
| :-: | :-: | :-: |
|title|标题|title: hello, world|
|date|创建日期，默认系统时间|date: 2020-7-19|
|updated|更新日期，默认再次创建日期|update: 2020-7-20|
|type|页面类型，tags、link、categories 这三个页面需要配置|type: tags|
|comments|是否显示评论，默认 true|comments: false|
|description|描述，没使用过，暂时不太清楚效果|--|
|top_img|顶部图，默认为系统default配置的图|top_img: 图片URL或者博客相对路径|
|mathjax|数学公式是否显示，默认为 false ，不显示|mathjax: true|
|katex|数学公式是否显示，默认为 false ，不显示|mathjax: true|
|aside|true 表示显示右边信息卡片，默认值；false 表示不显示|aside: true|
|aplayer|在需要的页面加载 aplayer 的 js 和 css, 请参考文章下面的音乐 配置|--|
|highlight_shrink|配置代码框是否展开，默认为设置中 highlight_shrink 的配置|--|

## Post Front-Matter
文章的文件头配置文件。

| Type | Explanation | Example |
| :-: | :-: | :-: |
|title|标题|title: Hello,World！|
|       date       |                    创建日期，默认系统时间                    |date: 2020-7-19|
|updated|更新日期，默认再次创建日期|update: 2020-7-20|
|tags|标签，用 \- 列出标签，一个 \- 表示一个标签，注意换行以及 \- 后面有个空格|--|
|categories|分类，同样用 \- 区别多个分类，注意换行以及 \- 后面有个空格|--|
|keywords|关键字|keywords: 'a, b'|
|description|描述，没使用过，暂时不太清楚效果|--|
|top_img|顶部图，可选项，不写则按缩略图的图片显示|top_img: 图片URL或者博客中图片的相对路径|
|comments|是否显示评论，默认 true。|comments: false|
|cover|缩略图|cover: 图片URL或者博客中图片的相对路径|
|toc|是否显示 toc ，默认 true 显示|toc: false|
|toc_number|是否显示 toc 数字，默认 true 显示|toc_number: false|
|auto_open|是否自动打开 TOC (默认为设置中 toc 的 auto_open 配置)|--|
|copyright|是否显示版权，默认 true 显示|copyright: false|
|mathjax|数学公式是否显示，默认为 false ，不显示|mathjax: true|
|katex|数学公式是否显示，默认为 false ，不显示|mathjax: true|
|hidden或hide|                 是否隐藏，需安装hide或者indexed插件，true表示隐藏                |hidden: true|
|sticky|文章置顶，数值越大越靠前，需安装indexed插件，默认值为0|sticky: 10|
|top|文章置顶，需安装index-pin-top 插件，默认值为false，同时为置顶则按时间先后顺序|top: true|
|aplayer|在需要的页面加载 aplayer 的 js 和 css, 请参考文章下面的音乐 配置|--|
|highlight_shrink|配置代码框是否展开，默认为设置中 highlight_shrink 的配置|--|



# 未完待续



---