---
title: 三角函数恒等式与方程
tags:
  - AMC12
  - 知识点
---

# 三角函数恒等式与方程

## 基本恒等式

最基本的恒等式为

$$
\sin^2x+\cos^2x=1,
$$

$$
\tan x=\frac{\sin x}{\cos x}
\qquad(\cos x\ne0).
$$

倒数关系为

$$
\sec x=\frac1{\cos x},
\qquad
\csc x=\frac1{\sin x}.
$$

由此得到

$$
1+\tan^2x=\sec^2x,
\qquad
1+\cot^2x=\csc^2x.
$$

化简时应尽量把所有函数统一成 $\sin x,\cos x$，并记录分母不能为零的条件。

## 和差与倍角公式

和差公式：

$$
\sin(A\pm B)=\sin A\cos B\pm\cos A\sin B,
$$

$$
\cos(A\pm B)=\cos A\cos B\mp\sin A\sin B.
$$

倍角公式：

$$
\sin2x=2\sin x\cos x,
$$

$$
\cos2x=\cos^2x-\sin^2x
=1-2\sin^2x
=2\cos^2x-1.
$$

常用半角形式为

$$
\sin^2\frac x2=\frac{1-\cos x}{2},
\qquad
\cos^2\frac x2=\frac{1+\cos x}{2}.
$$

半角开平方时要结合角所在象限判断正负。

## 合并正弦与余弦

对

$$
a\sin x+b\cos x
$$

令

$$
R=\sqrt{a^2+b^2},
\qquad
\cos\phi=\frac aR,\quad
\sin\phi=\frac bR,
$$

则

$$
a\sin x+b\cos x=R\sin(x+\phi).
$$

因此其值域为

$$
[-R,R].
$$

这比逐个试角更适合判断方程解的存在性、最值或解的个数。

## 三角方程

常见基本解：

$$
\sin x=\sin\alpha
\Longleftrightarrow
x=\alpha+2k\pi
\quad\text{或}\quad
x=\pi-\alpha+2k\pi,
$$

$$
\cos x=\cos\alpha
\Longleftrightarrow
x=\pm\alpha+2k\pi,
$$

$$
\tan x=\tan\alpha
\Longleftrightarrow
x=\alpha+k\pi.
$$

若题目限制 $x$ 在某个区间，先写一般解，再筛选区间内的整数 $k$，不要只写主值。

## 因式分解与代换

若方程含有

$$
\sin^2x,\quad\sin x,\quad\cos^2x
$$

等结构，可以设 $t=\sin x$ 或 $t=\cos x$，但必须保留 $-1\le t\le1$。若出现 $\sin2x$ 和 $\cos2x$，可以统一改写成一个角的正弦余弦，或利用倍角公式因式分解。

例如

$$
\sin^2x-\cos^2x=0
\quad\Longleftrightarrow\quad
\cos2x=0.
$$

除以 $\sin x$、$\cos x$ 或其他三角因子前，必须单独检查该因子等于零的情形。

## 特殊角与值域

常用值：

$$
\sin30^\circ=\frac12,\quad
\cos60^\circ=\frac12,\quad
\sin45^\circ=\cos45^\circ=\frac{\sqrt2}{2},
$$

$$
\sin60^\circ=\cos30^\circ=\frac{\sqrt3}{2}.
$$

如果一个乘积等于 $1$，而每个因子都不超过 $1$，则必须每个因子都等于 $1$。类似地，先用 $-1\le\sin x,\cos x\le1$ 限制范围，常可直接排除不存在的情形。

## 周期与交点计数

周期为：

$$
\sin(x+2\pi)=\sin x,\qquad
\cos(x+2\pi)=\cos x,\qquad
\tan(x+\pi)=\tan x.
$$

若方程含有周期函数与单调函数，先用值域限制定义域，再按每个周期或半周期分析交点。半波长度是周期的一半，不能把完整周期和单调分支混用。

## 常见陷阱

- 把 $\sin(A+B)$ 的符号或 $\cos(A+B)$ 的中间符号写错。
- 除以可能为零的 $\sin x$ 或 $\cos x$ 后漏掉解。
- 只求主值，漏掉指定区间内的其他周期解。
- 使用半角公式时忽略象限导致符号错误。
- 看到乘积等于 $1$，却没有使用每个因子的值域。
- 计数时把周期长度当成半波长度，或重复计算端点交点。

## 关联题目

- [[Problems/2024-A/Q08.zh-CN.md|2024-A-Q08]]
- [[Problems/2024-A/Q10.zh-CN.md|2024-A-Q10]]
- [[Problems/2024-A/Q18.zh-CN.md|2024-A-Q18]]
- [[Problems/2024-A/Q23.zh-CN.md|2024-A-Q23]]
- [[Problems/2024-B/Q11.zh-CN.md|2024-B-Q11]]
- [[Problems/2024-B/Q19.zh-CN.md|2024-B-Q19]]
- [[Problems/2024-B/Q21.zh-CN.md|2024-B-Q21]]
- [[Problems/2024-B/Q22.zh-CN.md|2024-B-Q22]]
- [[Problems/2025-A/Q08.zh-CN.md|2025-A-Q08]]
- [[Problems/2025-A/Q16.zh-CN.md|2025-A-Q16]]
- [[Problems/2025-A/Q24.zh-CN.md|2025-A-Q24]]
- [[Problems/2025-B/Q16.zh-CN.md|2025-B-Q16]]
- [[Problems/2025-B/Q21.zh-CN.md|2025-B-Q21]]
- [[Problems/2025-B/Q24.zh-CN.md|2025-B-Q24]]
- [[Problems/2023-A/Q11.zh-CN.md|2023-A-Q11]]
- [[Problems/2023-A/Q15.zh-CN.md|2023-A-Q15]]
- [[Problems/2023-A/Q25.zh-CN.md|2023-A-Q25]]
- [[Problems/2023-B/Q11.zh-CN.md|2023-B-Q11]]
- [[Problems/2023-B/Q17.zh-CN.md|2023-B-Q17]]
- [[Problems/2023-B/Q20.zh-CN.md|2023-B-Q20]]
- [[Problems/2022-A/Q12.zh-CN.md|2022-A-Q12]]
- [[Problems/2022-A/Q17.zh-CN.md|2022-A-Q17]]
- [[Problems/2022-A/Q18.zh-CN.md|2022-A-Q18]]
- [[Problems/2022-B/Q14.zh-CN.md|2022-B-Q14]]
- [[Problems/2022-B/Q24.zh-CN.md|2022-B-Q24]]
- [[Problems/2021-A/Q19.zh-CN.md|2021-A-Q19]]
- [[Problems/2021-B/Q13.zh-CN.md|2021-B-Q13]]
- [[Problems/2021-B/Q21.zh-CN.md|2021-B-Q21]]
- [[Problems/2020-A/Q09.zh-CN.md|2020-A-Q09]]
- [[Problems/2020-A/Q14.zh-CN.md|2020-A-Q14]]
- [[Problems/2020-A/Q18.zh-CN.md|2020-A-Q18]]
- [[Problems/2020-A/Q24.zh-CN.md|2020-A-Q24]]
- [[Problems/2020-B/Q04.zh-CN.md|2020-B-Q04]]
- [[Problems/2020-B/Q07.zh-CN.md|2020-B-Q07]]
- [[Problems/2020-B/Q09.zh-CN.md|2020-B-Q09]]
- [[Problems/2020-B/Q23.zh-CN.md|2020-B-Q23]]
- [[Problems/2020-B/Q25.zh-CN.md|2020-B-Q25]]
