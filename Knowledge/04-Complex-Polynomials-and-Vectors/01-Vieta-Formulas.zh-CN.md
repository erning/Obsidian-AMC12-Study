---
title: 韦达定理
tags:
  - AMC12
  - 知识点
---

# 韦达定理

## 二次方程

若

$$
ax^2+bx+c=0,\qquad a\ne0
$$

的根为 $\alpha,\beta$，则

$$
\alpha+\beta=-\frac ba,
\qquad
\alpha\beta=\frac ca.
$$

因此不必求出两个根，就能计算它们的和、积、差的平方：

$$
(\alpha-\beta)^2
=(\alpha+\beta)^2-4\alpha\beta.
$$

若题目给出根的条件，先写和与积，再把条件转成关于这两个对称量的方程。

## 三次与一般多项式

若三次多项式

$$
ax^3+bx^2+cx+d
$$

的根为 $\alpha,\beta,\gamma$，则

$$
\alpha+\beta+\gamma=-\frac ba,
$$

$$
\alpha\beta+\beta\gamma+\gamma\alpha=\frac ca,
$$

$$
\alpha\beta\gamma=-\frac da.
$$

一般地，首项系数为 $a_n$ 的多项式

$$
a_nx^n+a_{n-1}x^{n-1}+\cdots+a_0
$$

的根的基本对称和满足交替符号关系：

$$
e_k=(-1)^k\frac{a_{n-k}}{a_n}.
$$

## 根的代入与因式定理

若 $f(r)=0$，则 $x-r$ 是 $f(x)$ 的因子：

$$
f(x)=(x-r)q(x).
$$

余式定理给出

$$
f(x)\div(x-r)
\quad\text{的余数为}\quad f(r).
$$

若已知一个根，先因式分解降次，再使用韦达定理处理剩余根。

## 根的变换

若 $\alpha,\beta$ 是原方程的根，则新根

$$
\alpha+k,\quad\beta+k
$$

的和为

$$
(\alpha+\beta)+2k,
$$

积为

$$
\alpha\beta+k(\alpha+\beta)+k^2.
$$

类似地，倒数根（根不为零）的和与积为

$$
\frac1\alpha+\frac1\beta
=\frac{\alpha+\beta}{\alpha\beta},
\qquad
\frac1{\alpha\beta}.
$$

遇到新方程的根是原根的平方、倒数或平移时，先用对称量变换，比重新求根更快。

## 复根与共轭

若多项式系数为实数，非实根成共轭对：

$$
\alpha=u+vi
\quad\Longrightarrow\quad
\bar\alpha=u-vi.
$$

共轭根的和与积为实数：

$$
\alpha+\bar\alpha=2u,
\qquad
\alpha\bar\alpha=u^2+v^2.
$$

这常与韦达定理结合求未知实根或多项式系数。

## 常见陷阱

- 忘记先除以首项系数，直接把系数当作根的和与积。
- 三次项的符号写错。
- 只用根的和，漏掉根的乘积。
- 复根没有按共轭成对处理。
- 根的变换后仍把原来的对称和当作新对称和。

## 关联题目

- [[Problems/2023-B/Q14.zh-CN.md|2023-B-Q14]]
- [[Problems/2024-B/Q17.zh-CN.md|2024-B-Q17]]
- [[Problems/2025-A/Q12.zh-CN.md|2025-A-Q12]]
- [[Problems/2025-A/Q19.zh-CN.md|2025-A-Q19]]
- [[Problems/2025-B/Q08.zh-CN.md|2025-B-Q08]]
- [[Problems/2022-A/Q15.zh-CN.md|2022-A-Q15]]
- [[Problems/2022-A/Q22.zh-CN.md|2022-A-Q22]]
- [[Problems/2022-B/Q04.zh-CN.md|2022-B-Q04]]
- [[Problems/2021-A/Q12.zh-CN.md|2021-A-Q12]]
- [[Problems/2021-A/Q20.zh-CN.md|2021-A-Q20]]
- [[Problems/2021-A/Q22.zh-CN.md|2021-A-Q22]]
- [[Problems/2021-B/Q16.zh-CN.md|2021-B-Q16]]
- [[Problems/2020-A/Q15.zh-CN.md|2020-A-Q15]]
- [[Problems/2020-A/Q20.zh-CN.md|2020-A-Q20]]
- [[Problems/2020-A/Q22.zh-CN.md|2020-A-Q22]]
- [[Problems/2020-B/Q12.zh-CN.md|2020-B-Q12]]
- [[Problems/2020-B/Q17.zh-CN.md|2020-B-Q17]]
