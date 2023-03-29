title: "Array - Input"
subtitle: "数组输入"
layout: post
author: "Lianz"
header-style: text
hidden: false
tags:

  - 笔记
  - 基础
  - Python

## 一维数组

``` python
arr = input()

以空格作为间隔

nums = [int(n) for n in arr.split()]

```



## 二维数组

``` python
n = int(input()) # 输入二维数组的行数和列数

line = [[0]*n]*n # 初始化二维数组

for i in range(n):
	line[i] = input().split(" ") # 输入二维数组，同行数字用空格分隔，不同行则用回车换行
	line[i] = [int(j) for j in line[i]] # 将数组中的每一行转换成整型
  
print(line) # 打印二维数组
```

