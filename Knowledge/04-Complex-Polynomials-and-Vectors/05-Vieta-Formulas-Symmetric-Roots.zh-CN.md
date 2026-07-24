---
title: 韦达定理与根的对称式
tags:
  - AMC12
  - 知识点
---

# 韦达定理与根的对称式

## 基本对称式

若二次方程的根为 $\alpha,\beta$，记

$$
s=\alpha+\beta,\qquad p=\alpha\beta.
$$

则

$$
\alpha^2+\beta^2=s^2-2p,
$$

$$
\frac1\alpha+\frac1\beta=\frac sp,
$$

$$
(\alpha-\beta)^2=s^2-4p.
$$

很多“根的复杂表达式”都可以先化为 $s,p$ 的函数。

## 幂和递推

令

$$
P_n=\alpha^n+\beta^n,
$$

若 $\alpha,\beta$ 是

$$
x^2-sx+p=0
$$

的根，则每个根满足 $x^2=sx-p$，从而

$$
P_n=sP_{n-1}-pP_{n-2}.
$$

初值为

$$
P_0=2,\qquad P_1=s.
$$

这比直接求根更适合计算高次幂和。

## 三个根的对称式

若根为 $\alpha,\beta,\gamma$，记

$$
s_1=\alpha+\beta+\gamma,
$$

$$
s_2=\alpha\beta+\beta\gamma+\gamma\alpha,
$$

$$
s_3=\alpha\beta\gamma.
$$

则

$$
\alpha^2+\beta^2+\gamma^2=s_1^2-2s_2,
$$

$$
\alpha^3+\beta^3+\gamma^3
=s_1^3-3s_1s_2+3s_3.
$$

更高次幂可用 Newton 递推逐步计算，而不必求出每个根。

## 根的倒数、平移和乘积

若根均非零，倒数根的基本对称量为

$$
\sum\frac1{\alpha_i}
=\frac{e_{n-1}}{e_n},
\qquad
\prod\frac1{\alpha_i}
=\frac1{e_n},
$$

其中 $e_k$ 是原根的基本对称和。

若每个根平移 $k$，可以将

$$
\prod_i(x-(\alpha_i+k))
$$

写成原多项式 $f(x-k)$，再读取新系数。

## 根的积与多项式常数项

首项系数为 $a_n$、常数项为 $a_0$ 的 $n$ 次多项式，所有根的积为

$$
\prod_i\alpha_i=(-1)^n\frac{a_0}{a_n}.
$$

如果只要求所有解的积，通常优先使用这个关系，而不是逐个求解。

## 变量换元

若方程中的变量是

$$
t=\log_a x
\quad\text{或}\quad
t=x+\frac1x,
$$

先在 $t$ 中求根，再利用根和根积恢复 $x$。若两个 $t$ 根互为相反数，则对应的指数变量可能互为倒数。

换元后必须检查每个 $t$ 是否能由允许的 $x$ 产生。

## 常见陷阱

- 把根的和、积与多项式系数的符号写反。
- 计算三次幂和时漏掉 $3s_3$。
- 对倒数根使用原来的积，而没有取倒数。
- 只找到根的一个对称量，却试图唯一确定非对称表达式。
- 换元解出候选根后没有恢复原变量或检查定义域。

## 关联题目

- [[Problems/2024-A/Q15.zh-CN.md|2024-A-Q15]]
- [[Problems/2024-B/Q17.zh-CN.md|2024-B-Q17]]
- [[Problems/2025-A/Q12.zh-CN.md|2025-A-Q12]]
- [[Problems/2025-A/Q19.zh-CN.md|2025-A-Q19]]
- [[Problems/2025-B/Q08.zh-CN.md|2025-B-Q08]]
- [[Problems/2023-A/Q19.zh-CN.md|2023-A-Q19]]
- [[Problems/2023-B/Q06.zh-CN.md|2023-B-Q06]]
- [[Problems/2023-B/Q14.zh-CN.md|2023-B-Q14]]
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
