---
title: 楼层函数与分块计数
tags:
  - AMC12
  - 知识点
---

# 楼层函数与分块计数

## 楼层函数的定义

楼层函数 $\lfloor x\rfloor$ 是不超过 $x$ 的最大整数：

$$
\lfloor x\rfloor\le x<\lfloor x\rfloor+1.
$$

等价地，

$$
n=\lfloor x\rfloor
\quad\Longleftrightarrow\quad
n\le x<n+1,
\qquad n\in\mathbb Z.
$$

对负数要特别小心：

$$
\lfloor-2.3\rfloor=-3,
\qquad
\lceil-2.3\rceil=-2.
$$

楼层函数不是“去掉小数部分”，而是向负无穷取整。

## 常用性质

对任意实数 $x$，

$$
x-1<\lfloor x\rfloor\le x.
$$

若 $n$ 为整数，则

$$
\lfloor x+n\rfloor=\lfloor x\rfloor+n.
$$

若 $n\ge1$ 为整数，则

$$
\left\lfloor\frac{\lfloor x\rfloor}{n}\right\rfloor
=\left\lfloor\frac xn\right\rfloor.
$$

但一般不能把楼层函数分配到乘法或加法上：

$$
\lfloor x+y\rfloor
\ne\lfloor x\rfloor+\lfloor y\rfloor,
\qquad
\lfloor xy\rfloor
\ne\lfloor x\rfloor\lfloor y\rfloor.
$$

可用分数部分

$$
\{x\}=x-\lfloor x\rfloor,\qquad 0\le\{x\}<1
$$

来记录取整后剩余的部分。

## 解楼层不等式

若

$$
\lfloor f(x)\rfloor=k,
$$

直接改写为

$$
k\le f(x)<k+1.
$$

例如

$$
\left\lfloor\frac x3\right\rfloor=5
\quad\Longleftrightarrow\quad
15\le x<18.
$$

如果题目给出 $\lfloor f(x)\rfloor\le k$ 或 $\ge k$，也可以利用整数值把它转成普通不等式：

$$
\lfloor f(x)\rfloor\le k
\quad\Longleftrightarrow\quad
f(x)<k+1,
$$

$$
\lfloor f(x)\rfloor\ge k
\quad\Longleftrightarrow\quad
f(x)\ge k.
$$

## 分块计数

许多计数题中，$\lfloor n/m\rfloor$ 表示把整数 $n$ 按大小为 $m$ 的区块分组。对整数 $n\ge0$，

$$
n=mq+r,\qquad 0\le r<m,
$$

其中

$$
q=\left\lfloor\frac nm\right\rfloor.
$$

因此每个完整区块贡献 $m$ 个对象，最后一个不完整区块贡献余数 $r$ 个对象。把计数范围按

$$
km\le n<(k+1)m
$$

分段，通常可以去掉楼层函数。

## 周期性与楼层函数

如果表达式含有 $\lfloor (n+c)/m\rfloor$，令 $n=mk+r$，其中 $0\le r<m$，可以把问题拆成 $m$ 种余数类。对每一类，楼层函数通常变成关于 $k$ 的简单线性式。

当题目只问一段有限范围内的计数时，先找周期长度，再计算完整周期和边界残段，注意端点是否重复。

## 常见陷阱

- 把 $\lfloor-2.3\rfloor$ 写成 $-2$。
- 将 $\lfloor x+y\rfloor$ 直接拆成两个楼层函数。
- 用 $\le$ 代替 $\lt$，导致边界被多算。
- 分块计数时忘记最后一个不完整区块。
- 计算完整周期后，漏掉开头或结尾的残段。
- 看到取整符号就逐个枚举，却没有先按余数或区间分块。

## 关联题目

- [[Problems/2022-B/Q06.zh-CN.md|2022-B-Q06]]
