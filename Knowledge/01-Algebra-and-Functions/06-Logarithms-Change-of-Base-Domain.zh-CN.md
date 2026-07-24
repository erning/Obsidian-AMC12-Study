---
title: 对数运算、换底与定义域
tags:
  - AMC12
  - 知识点
---

# 对数运算、换底与定义域

## 对数的定义与基本性质

当 $a>0$ 且 $a\ne1$ 时，$a$ 的对数定义为

$$
\log_a x=y\quad\Longleftrightarrow\quad a^y=x.
$$

这里必须满足 $x>0$。因此，对数的三个基本条件是

$$
\boxed{a>0,\qquad a\ne1,\qquad x>0.}
$$

常用特殊值包括

$$
\log_a1=0,\qquad \log_aa=1,
$$

以及

$$
\log_a(a^t)=t,\qquad a^{\log_a x}=x.
$$

第二组公式中的输入必须先满足相应的定义域条件。特别是，$\log_a0$ 和 $\log_a(-x)$（当 $x>0$）在实数范围内没有定义。

> [!warning] 定义域优先
> 对数恒等式只能在各项都有定义时使用。解出方程后还要把候选解代回原式，排除使对数真数不正、对数底数不合法或分母为零的值。

## 对数运算法则

当 $M>0$、$N>0$ 时，

$$
\log_a(MN)=\log_aM+\log_aN,
$$

$$
\log_a\left(\frac MN\right)=\log_aM-\log_aN,
$$

$$
\log_a(M^r)=r\log_aM.
$$

因此，乘积、商和幂可以分别转化为对数的和、差和倍数。例如

$$
\log_2 20=\log_2(4\cdot5)=2+\log_2 5,
$$

$$
\log_2\left(1+\frac1n\right)
=\log_2\left(\frac{n+1}{n}\right)
=\log_2(n+1)-\log_2n.
$$

但一般不能拆分加法：

$$
\log_a(M+N)\ne\log_aM+\log_aN.
$$

也不能把 $\log_a(M^r)$ 误写成 $(\log_aM)^r$。

## 换底公式

对任意合法的新底数 $b$，有

$$
\log_a x=\frac{\log_bx}{\log_ba}.
$$

最常用的形式是

$$
\log_a x=\frac{\ln x}{\ln a}
=\frac{\log x}{\log a}.
$$

当题目中的多个对数底数不同时，可以先统一成同一个底数。换底公式还给出几个高频恒等式：

$$
\log_a b=\frac1{\log_ba},
$$

$$
\log_a b\cdot\log_b c=\log_a c,
$$

$$
\frac{\log_a x}{\log_a y}=\log_yx.
$$

其中每一个对数都必须有定义，分母还必须不为零。

### 复合分式的化简

设 $L$ 表示同一底数下的 $\log x$。例如在原式有定义且各底数合法时，

$$
\frac{\log_p x\cdot\log_q x}
{\log_p x+\log_q x}
=\log_{pq}x.
$$

验证方法是换成自然对数：

$$
\frac{\frac{\ln x}{\ln p}\cdot\frac{\ln x}{\ln q}}
{\frac{\ln x}{\ln p}+\frac{\ln x}{\ln q}}
=\frac{\ln x}{\ln p+\ln q}
=\frac{\ln x}{\ln(pq)}.
$$

这类题的关键不是把对数底数相加，而是先统一底数，再约去公共因子。

## 定义域与符号

### 单个对数与对数式

对于 $\log_a f(x)$，需要同时检查

$$
a>0,\qquad a\ne1,\qquad f(x)>0.
$$

如果对数出现在分母，还要加上

$$
\log_a f(x)\ne0
\quad\Longleftrightarrow\quad
f(x)\ne1.
$$

如果底数含有变量，例如 $\log_{7x}2023$，则必须满足

$$
x>0,\qquad 7x\ne1.
$$

换底后

$$
\log_{7x}2023
=\frac{\log_{2023}2023}{\log_{2023}(7x)}
=\frac1{\log_{2023}7+\log_{2023}x},
$$

还要保证换底后的分母不为零；这正对应原式底数 $7x\ne1$。

### 对数的正负

若 $a>1$，则

$$
0<x<1\Longrightarrow\log_ax<0,
\qquad
x>1\Longrightarrow\log_ax>0.
$$

若 $0<a<1$，上述正负关系反过来。这个判断常用于排除方程的候选解或判断某个根式是否可以拆开。

### 单调性与不等式

- 当 $a>1$ 时，$\log_a x$ 严格递增，故
  $$
  \log_a u<\log_a v\Longleftrightarrow u<v.
  $$
- 当 $0<a<1$ 时，$\log_a x$ 严格递减，故不等号方向反转：
  $$
  \log_a u<\log_a v\Longleftrightarrow u>v.
  $$

解对数不等式时，先确认底数是在 $1$ 的上方还是下方，不能机械地保留不等号方向。

## 常见对数方程

### 单个对数等于常数

$$
\log_a f(x)=c
\quad\Longleftrightarrow\quad
f(x)=a^c.
$$

解出 $x$ 后仍需检查 $f(x)>0$。例如

$$
\log_2(x-1)=3
\Longrightarrow x-1=8
\Longrightarrow x=9.
$$

### 同底对数相等

若 $a>0$ 且 $a\ne1$，则在定义域内

$$
\log_a f(x)=\log_a g(x)
\quad\Longleftrightarrow\quad
f(x)=g(x).
$$

### 先换元再化为代数方程

当多个对数的真数或底数是幂的关系时，设一个对数为新变量通常最有效。例如令

$$
y=\log_4n,
$$

则

$$
\log_{16}n=\frac12\log_4n=\frac y2.
$$

原来的对数方程可以转化为关于 $y$ 的代数方程。此时要保留 $y>0$ 等由原定义域带来的条件，避免把代数变形产生的增根留下。

## 对数的几何与代数模型

### 对数图像上的中点

若点 $A(x_1,\log_a x_1)$、$B(x_2,\log_a x_2)$ 位于曲线 $y=\log_a x$ 上，且中点为 $(h,k)$，则

$$
x_1+x_2=2h,
$$

并且

$$
\log_a x_1+\log_a x_2=2k
\quad\Longrightarrow\quad
x_1x_2=a^{2k}.
$$

于是无需解出 $x_1,x_2$，就可以使用

$$
(x_1-x_2)^2=(x_1+x_2)^2-4x_1x_2
$$

求两横坐标之差。这是把几何的中点条件转成“和与积”的典型方法。

### 对数化简幂模型

若一个量满足

$$
v=kn^am^b,
$$

对同一底数取对数可得

$$
\log v=\log k+a\log n+b\log m.
$$

此时幂指数 $a,b$ 变成 $\log n$、$\log m$ 的系数，可以通过比较系数或代入特殊条件求出。注意

$$
\log(kn^am^b)=\log k+a\log n+b\log m,
$$

而不是 $\log k+an^a+bm^b$。

### 变量出现在底数中

若方程含有 $\log_{cx}N$，可以选定一个固定的合法底数 $r$，并令

$$
t=\log_rx,
\qquad
\alpha=\log_rc.
$$

则

$$
\log_{cx}N
=\frac{\log_rN}{\log_r(cx)}
=\frac{\log_rN}{\alpha+t}.
$$

方程通常会因此化为关于 $t$ 的一次或二次方程。若得到根 $t_1,t_2$，对应的 $x$ 为 $r^{t_1},r^{t_2}$，所以

$$
x_1x_2=r^{t_1+t_2}.
$$

特别地，如果 $t_1+t_2=0$，则两个 $x$ 互为倒数，且 $x_1x_2=1$。最后必须检查所有原始底数和真数条件。

## 进制位数

对整数底数 $b\ge2$，正整数 $N$ 在 $b$ 进制下的位数为

$$
\boxed{\lfloor\log_bN\rfloor+1}.
$$

理由是：若有 $k$ 位，则

$$
b^{k-1}\le N<b^k.
$$

取以 $b$ 为底的对数可得 $k-1\le\log_bN<k$。即使 $N$ 恰好是 $b$ 的整数次幂，也应使用上面的下取整公式；例如 $N=b^3$ 时位数是 $4$，不是 $3$。

如果题目给的是常用对数，可以使用

$$
\log_bN=\frac{\log_{10}N}{\log_{10}b}.
$$

估算后要检查结果是否接近整数边界，因为下取整对误差很敏感。

## 裂项相消

对数的商法则常把求和转成裂项：令 $a_n=\log_b n$，则

$$
\log_b\left(1+\frac1n\right)=a_{n+1}-a_n.
$$

因此

$$
\frac{\log_b\left(1+\frac1n\right)}
{(\log_bn)(\log_b(n+1))}
=\frac{a_{n+1}-a_n}{a_na_{n+1}}
=\frac1{a_n}-\frac1{a_{n+1}}.
$$

求和时中间项全部相消：

$$
\sum_{n=p}^{q}
\left(\frac1{a_n}-\frac1{a_{n+1}}\right)
=\frac1{a_p}-\frac1{a_{q+1}}.
$$

识别这种结构的关键是先把 $1+\dfrac1n$ 改写成 $\dfrac{n+1}{n}$，再使用商法则。

## 绝对值与对数距离

在数轴上，两个对数值之间的距离为

$$
\left|\log_a x-\log_a y\right|
=\left|\log_a\left(\frac xy\right)\right|.
$$

如果已知某个距离等于 $d$，则应拆成两个分支：

$$
\log_a x=\log_a y\pm d.
$$

当 $d$ 本身可以写成对数时，利用加减法则可以直接转回乘法或除法。例如

$$
\log_a x=\log_a y\pm\log_a r
\quad\Longrightarrow\quad
x=yr\quad\text{或}\quad x=\frac yr.
$$

不要把数轴上的数 $1$ 误读成 $\log_a1$；例如

$$
|\log_a10-1|=|\log_a10-\log_aa|.
$$

## 统一解题流程

遇到对数题时，可以按以下顺序检查：

1. 先写出所有定义域：每个真数大于 $0$，每个底数大于 $0$ 且不等于 $1$，分母还不能为 $0$；
2. 观察底数是否有幂、倒数或乘积关系；
3. 选择策略：直接用定义、合并对数、换底、换元、比较系数或裂项相消；
4. 变形时始终保留原式的限制条件；
5. 解出候选值后代回原式检查；
6. 最后检查题目问的是值、解的个数、所有解的和/积，还是进制位数。

## 常见陷阱

- 忘记对数真数必须为正，或忘记底数不能等于 $1$。
- 把 $\log_a(M+N)$ 错拆成 $\log_aM+\log_aN$。
- 把换底公式中的分母写反：正确的是 $\log_a x=\dfrac{\log_bx}{\log_ba}$。
- 把 $\log_{a^k}x$ 误写成 $k\log_ax$；正确的是 $\dfrac1k\log_ax$。
- 认为不同底数的对数可以直接相加，例如 $\log_2x+\log_3x\ne\log_5x$。
- 对数方程化成代数方程后不检查增根，尤其是把 $y=0$ 代回会导致分母或对数无定义的情况。
- 计算进制位数时使用 $\lceil\log_bN\rceil$，却没有检查 $N$ 是否恰好是 $b$ 的幂。
- 看到变量在对数底数中时，只检查 $x>0$，却漏掉底数不等于 $1$ 的限制。

## 关联题目

- [[Problems/2024-A/Q08.zh-CN.md|2024-A-Q08]]
- [[Problems/2024-B/Q06.zh-CN.md|2024-B-Q06]]
- [[Problems/2024-B/Q08.zh-CN.md|2024-B-Q08]]
- [[Problems/2024-B/Q15.zh-CN.md|2024-B-Q15]]
- [[Problems/2025-A/Q07.zh-CN.md|2025-A-Q07]]
- [[Problems/2025-B/Q07.zh-CN.md|2025-B-Q07]]
- [[Problems/2025-B/Q24.zh-CN.md|2025-B-Q24]]
- [[Problems/2023-A/Q06.zh-CN.md|2023-A-Q06]]
- [[Problems/2023-A/Q19.zh-CN.md|2023-A-Q19]]
- [[Problems/2023-B/Q07.zh-CN.md|2023-B-Q07]]
- [[Problems/2022-A/Q11.zh-CN.md|2022-A-Q11]]
- [[Problems/2022-A/Q14.zh-CN.md|2022-A-Q14]]
- [[Problems/2022-B/Q16.zh-CN.md|2022-B-Q16]]
- [[Problems/2021-A/Q14.zh-CN.md|2021-A-Q14]]
- [[Problems/2021-B/Q09.zh-CN.md|2021-B-Q09]]
- [[Problems/2021-B/Q21.zh-CN.md|2021-B-Q21]]
- [[Problems/2020-A/Q10.zh-CN.md|2020-A-Q10]]
- [[Problems/2020-A/Q17.zh-CN.md|2020-A-Q17]]
- [[Problems/2020-B/Q13.zh-CN.md|2020-B-Q13]]
