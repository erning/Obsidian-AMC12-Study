---
title: 复数、单位根与 De Moivre 定理
tags:
  - AMC12
  - 知识点
---

# 复数、单位根与 De Moivre 定理

## 复数的基本运算

复数写成

$$
z=a+bi,\qquad i^2=-1.
$$

实部为 $a$，虚部为 $b$，共轭为

$$
\bar z=a-bi.
$$

模长为

$$
|z|=\sqrt{a^2+b^2},
$$

并满足

$$
z\bar z=|z|^2.
$$

复数除法通常乘以分母的共轭：

$$
\frac{a+bi}{c+di}
=\frac{(a+bi)(c-di)}{c^2+d^2}.
$$

## 极坐标形式

非零复数可写为

$$
z=r(\cos\theta+i\sin\theta)
=r\,\operatorname{cis}\theta,
$$

其中 $r=|z|$，$\theta$ 是一个辐角。辐角只确定到 $2\pi$ 的整数倍：

$$
\arg z=\theta+2k\pi.
$$

乘法和除法在极坐标中分别对应模相乘、辐角相加，以及模相除、辐角相减。

## De Moivre 定理

$$
(\cos\theta+i\sin\theta)^n
=\cos(n\theta)+i\sin(n\theta).
$$

因此

$$
\bigl(r\,\operatorname{cis}\theta\bigr)^n
=r^n\operatorname{cis}(n\theta).
$$

它适合计算高次幂、比较实部虚部和求周期。若原数还带有模 $r$，不要只处理辐角而忘记 $r^n$。

## 单位根

方程

$$
z^n=1
$$

的 $n$ 个根为

$$
z_k=\operatorname{cis}\frac{2\pi k}{n},
\qquad k=0,1,\ldots,n-1.
$$

它们均匀分布在单位圆上，相邻根的圆心角为 $2\pi/n$。若 $\omega$ 是本原 $n$ 次单位根，则所有单位根为

$$
1,\omega,\omega^2,\ldots,\omega^{n-1}.
$$

其和为 $0$，且

$$
1+z+z^2+\cdots+z^{n-1}=0
\quad(z^n=1,\ z\ne1).
$$

## 复系数方程

求

$$
z^n=w
$$

时，先把 $w$ 写成极坐标：

$$
w=R\operatorname{cis}\phi.
$$

则解为

$$
z_k=R^{1/n}
\operatorname{cis}\left(\frac{\phi+2k\pi}{n}\right),
\qquad k=0,\ldots,n-1.
$$

解的模相同、辐角等间隔。

## 复根与实系数多项式

实系数多项式的非实根成共轭对。若已知根 $a+bi$，则 $a-bi$ 也是根，二次因子为

$$
(x-a-bi)(x-a+bi)
=(x-a)^2+b^2.
$$

这常用于把复根条件转化为实系数二次因子。

## 常见陷阱

- 复数乘法中漏掉 $i^2=-1$。
- 共轭只改变虚部符号，不改变实部。
- De Moivre 定理中忘记模长也要取 $n$ 次幂。
- 单位根下标重复或漏掉 $k=0$。
- 求 $n$ 次根时只写一个主值，漏掉其他 $n-1$ 个解。
- 辐角比较没有考虑 $2\pi$ 的整数倍。

## 关联题目

- [[Problems/2023-A/Q14.zh-CN.md|2023-A-Q14]]
- [[Problems/2023-A/Q25.zh-CN.md|2023-A-Q25]]
- [[Problems/2024-B/Q12.zh-CN.md|2024-B-Q12]]
- [[Problems/2025-A/Q09.zh-CN.md|2025-A-Q09]]
- [[Problems/2025-A/Q17.zh-CN.md|2025-A-Q17]]
- [[Problems/2025-B/Q03.zh-CN.md|2025-B-Q03]]
- [[Problems/2025-B/Q22.zh-CN.md|2025-B-Q22]]
- [[Problems/2022-A/Q13.zh-CN.md|2022-A-Q13]]
- [[Problems/2022-A/Q21.zh-CN.md|2022-A-Q21]]
- [[Problems/2022-A/Q22.zh-CN.md|2022-A-Q22]]
- [[Problems/2022-B/Q11.zh-CN.md|2022-B-Q11]]
- [[Problems/2022-B/Q24.zh-CN.md|2022-B-Q24]]
- [[Problems/2021-A/Q13.zh-CN.md|2021-A-Q13]]
- [[Problems/2021-A/Q15.zh-CN.md|2021-A-Q15]]
- [[Problems/2021-A/Q21.zh-CN.md|2021-A-Q21]]
- [[Problems/2021-A/Q22.zh-CN.md|2021-A-Q22]]
- [[Problems/2021-B/Q18.zh-CN.md|2021-B-Q18]]
- [[Problems/2021-B/Q23.zh-CN.md|2021-B-Q23]]
- [[Problems/2020-A/Q15.zh-CN.md|2020-A-Q15]]
- [[Problems/2020-A/Q22.zh-CN.md|2020-A-Q22]]
- [[Problems/2020-B/Q17.zh-CN.md|2020-B-Q17]]
- [[Problems/2020-B/Q23.zh-CN.md|2020-B-Q23]]
