---
layout:       post
title:        "Usage of Typora"
author:       "Lianz"
header-style: text
catalog:      true
tags:
    - Tools
    - Typora
---

> Simple usage of typora

# 块元素

## 段落

Use `Return` to create a new paragraph 

单个换行`shift+return`  

## 标题

#一级标题
##二级标题
######六级标题

## 引用

> ">"即可添加引用，
>
> > 允许嵌套，添加空格即可

## 列表

* 使用来创建**无序列表**
* 或者+ 或者 -

1. 可以用来创建**有序列表**
2. 前面加数字.

**任务列表**

- [ ] [ ]表示未完成
- [ ] [x]

## 代码块（栅栏式）

输入```之后输入一个可选的语言标识符，然后按return键后输入代码

```python
function test(){
	console.log("notice the blank line before this function?");
}
```

```ruby
require 'redcarpet'
markdown = Redcarpet.new("Hello World!")
puts markdown.to_html
```

## 数学公式

输入 `$$`, 然后“return”键将触发一个接受*Tex / LaTex*源代码的输入区域
$$
\mathbf{V}_1 \times \mathbf{V}_2 =  \begin{vmatrix} 
\mathbf{i} & \mathbf{j} & \mathbf{k} \\
\frac{\partial X}{\partial u} &  \frac{\partial Y}{\partial u} & 0 \\
\frac{\partial X}{\partial v} &  \frac{\partial Y}{\partial v} & 0 \\
\end{vmatrix}
$$

## 表格

输入 `| First Header | Second Header |` 并按下 `return` 键
notes：无法合并单元格，可以用html实现，但无法插入数学公式

| 列A  | 列B  |
| :--: | :--: |
|      |      |

## 脚注

`[^footnote]`   创建脚注举例[^1]

[^1]: 这是脚注

## 水平线

`***` 或 `---`  然后`return`

***

---

## 目录

`[toc]` 然后 `return`

随着内容更新会自动更新

[toc]

# Span元素

## 链接

`[显示的链接名称](实际的链接地址)`   （分为内联和引用，以下的例子为内联）

`This is [an example](http://example.com/) inline link.`

This is [an example](http://example.com/) inline link.

## 内部链接

Command+ 单击 [此链接](#目录) 将跳转到标题 `目录`处，在Windows上以Ctrl代替Command

## URL网址

在< >中插入需要跳转的URL网址即可

`<https://lianz-lit.github.io/>`

https://lianz-lit.github.io/

## 图片

与链接类似，只需在前面添加`!`，可以直接拖放来插入图片，会自动生成类似下面的链接

`![显示的链接名称](图片地址)`  

## 段中代码

使用 \`  \` 包围代码部分

调用`printf()`函数

## 删除线

在需要添加删除线的文字前后加上`~~`，注意是英文输入下的~~，而非～～

`这是~~需要删除~~的文字`

这是~~需要删除~~的文字

## 下划线

在需要添加下划线的文字前后分别加上`<u>`和`</u>`

`这是<u>需要下划线</u>的文字`

这是<u>需要下划线</u>的文字

## 表情符号

以英文`:`开头，会显示可以选择的表情

`:smile:`

:smile:

## 高亮

在需要高亮的文字前后加上`==`

`这是==需要高亮==的文字`

这是==需要高亮==的文字



# Others

< ---- `&lt;`

& ---- `&amp;`

*test* ---- `*test*` 或者`_test_` 均可实现斜体强调，建议使用前者

**test** ---- `**test**` 或者`__test__`均可实现加粗强调，建议使用前者

\*test*----`\*test\*`通过反斜杠`\`转义

内联数学公式、高亮、markdown自带的上标、下标等需要在偏好设置面板的markdown扩展语法中启用。
