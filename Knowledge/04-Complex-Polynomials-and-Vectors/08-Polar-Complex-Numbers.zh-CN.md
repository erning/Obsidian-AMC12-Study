---
title: 极坐标复数
tags:
  - AMC12
  - 知识点
---

# 极坐标复数

## 极坐标形式

非零复数可写为

$$
z=r(\cos\theta+i\sin\theta)
=r\operatorname{cis}\theta,
$$

其中

$$
r=|z|>0
$$

是模长，$\theta$ 是辐角。辐角不是唯一的：

$$
\theta+2k\pi
\qquad(k\in\mathbb Z)
$$

表示相同方向。

## 乘法、除法与幂

极坐标中

$$
r_1\operatorname{cis}\theta_1
\cdot
r_2\operatorname{cis}\theta_2
=r_1r_2\operatorname{cis}(\theta_1+\theta_2),
$$

$$
\frac{r_1\operatorname{cis}\theta_1}
{r_2\operatorname{cis}\theta_2}
=\frac{r_1}{r_2}
\operatorname{cis}(\theta_1-\theta_2).
$$

De Moivre 定理给出

$$
(r\operatorname{cis}\theta)^n
=r^n\operatorname{cis}(n\theta).
$$

因此高次幂的辐角只需模 $2\pi$ 化简。若指数很大，先对周期取模，不要直接展开。

## 单位根与周期

若 $z$ 是 $n$ 次单位根，则

$$
z^n=1,\qquad |z|=1.
$$

其辐角为

$$
\frac{2\pi k}{n},\qquad k=0,1,\ldots,n-1.
$$

若表达式中出现 $z^m$，只需将 $m$ 对 $n$ 取模：

$$
z^m=z^{m\bmod n}.
$$

要先确认 $z$ 确实是所给阶数的单位根，不能把任意复数都按单位根周期处理。

## 由极坐标恢复直角坐标

$$
x=r\cos\theta,\qquad y=r\sin\theta.
$$

如果要求实部或虚部，先完成幂的辐角和模长计算，再读取对应坐标。不要在幂运算前直接比较原数的实部，因为旋转会改变实部和虚部。

## 常见陷阱

- 把辐角当成唯一值，没有考虑 $2\pi$ 周期。
- 单位根幂次没有先取模。
- 忘记模长也要进行幂运算。
- 计算 $z^n$ 时比较了 $z$ 的实部，而题目问的是 $z^n$ 的实部。
- 将角度制和弧度制混用。

## 关联题目

- [[Problems/2022-B/Q11.zh-CN.md|2022-B-Q11]]
