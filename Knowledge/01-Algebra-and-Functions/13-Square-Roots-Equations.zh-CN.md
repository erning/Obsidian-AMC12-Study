---
title: 根式与平方根方程
tags:
  - AMC12
  - 知识点
---

# 根式与平方根方程

## 算术平方根

对 $A\ge0$，$\sqrt A$ 表示唯一的非负数 $r$，满足

$$
r^2=A,\qquad r\ge0.
$$

因此

$$
\sqrt{x^2}=|x|,
$$

而不是无条件等于 $x$。常用根式运算包括

$$
\sqrt{AB}=\sqrt A\sqrt B
\quad(A,B\ge0),
$$

以及

$$
\sqrt{\frac AB}=\frac{\sqrt A}{\sqrt B}
\quad(A\ge0,\ B>0).
$$

只有在相应非负条件成立时，才能拆分根式。

## 根式方程的等价变形

若方程为

$$
\sqrt{F(x)}=G(x),
$$

则原式等价于

$$
\begin{cases}
F(x)=G(x)^2,\\
G(x)\ge0,
\end{cases}
$$

并且还要有 $F(x)\ge0$。平方只得到必要条件；右边的非负性是保证逆向成立的关键。

若两边都是非负数，可以平方：

$$
\sqrt{A}=\sqrt{B}
\quad\Longleftrightarrow\quad
A=B,\qquad A,B\ge0.
$$

连续平方多次时，每一步都要保留当前两边非负的条件。

## 含参数的平方根等式

例如

$$
\sqrt{a}+\sqrt{b}=\sqrt{a+b+2\sqrt{ab}}
$$

成立的前提是 $a,b\ge0$，因为右侧是

$$
\sqrt{(\sqrt a+\sqrt b)^2}
=|\sqrt a+\sqrt b|
=\sqrt a+\sqrt b.
$$

若根式中出现 $|x|$，要按 $x\ge0$ 和 $x<0$ 分类，而不能直接去掉绝对值。

## 由平方得到的充要条件

如果题目要求某个等式与参数条件等价，不能只从原式平方得到一个必要条件。正确流程是：

1. 记录原式两边的符号；
2. 平方或移项得到代数条件；
3. 检查代数条件是否能保证原式两边的符号；
4. 写出必要且充分的条件。

例如

$$
\sqrt{u}+\sqrt{v}=0
$$

不仅要求 $uv=0$，还由于两个根式都非负，必须有

$$
u=0,\qquad v=0.
$$

若只知道平方后的乘积条件，仍需检查和的非负性或符号限制。

## 有理化

分母含有单个根式时，可以乘以同一个根式：

$$
\frac1{\sqrt a}=\frac{\sqrt a}{a}
\quad(a>0).
$$

分母是共轭式时使用平方差：

$$
\frac1{\sqrt a+\sqrt b}
\cdot
\frac{\sqrt a-\sqrt b}{\sqrt a-\sqrt b}
=\frac{\sqrt a-\sqrt b}{a-b}.
$$

有理化前要确认共轭因子不为零，结果中也应保留原分母的限制。

## 根式的估计

若只需判断大小，可以平方比较非负量：

$$
\sqrt A<\sqrt B
\quad\Longleftrightarrow\quad
A<B
\qquad(A,B\ge0).
$$

也可以利用相邻平方数：

$$
k^2\le N<(k+1)^2
\quad\Longrightarrow\quad
k\le\sqrt N<k+1.
$$

这与楼层函数、整数条件和范围计数经常结合出现。

## 常见陷阱

- 把 $\sqrt{x^2}$ 写成 $x$，忽略绝对值。
- 两边平方后不检查增根。
- 忘记 $\sqrt{F(x)}$ 的右侧必须非负。
- 未确认被开方数非负，就拆分或合并根式。
- 把“平方后成立”误当作“原式成立”，没有验证符号条件。

## 关联题目

- [[Problems/2021-A/Q02.zh-CN.md|2021-A-Q02]]
