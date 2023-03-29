[toc]



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

[toc]

# Span元素







# Others

< ---- `&lt;`

& ---- `&amp;`

*test* ---- `*test*` italic

**test** ---- `**test**` bold
