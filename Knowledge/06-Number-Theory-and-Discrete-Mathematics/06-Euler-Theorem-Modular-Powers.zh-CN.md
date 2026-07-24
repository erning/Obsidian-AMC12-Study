---
title: Euler 定理与模意义下的幂
tags:
  - AMC12
  - 知识点
---

# Euler 定理与模意义下的幂

## Euler 函数

Euler 函数 $\varphi(n)$ 表示 $1,2,\ldots,n$ 中与 $n$ 互质的整数个数。若

$$
n=\prod_{i=1}^r p_i^{e_i},
$$

则

$$
\varphi(n)=n\prod_{p\mid n}\left(1-\frac1p\right).
$$

特别地，若 $p$ 为质数，则 $\varphi(p)=p-1$；若 $\gcd(a,b)=1$，则 $\varphi(ab)=\varphi(a)\varphi(b)$。

## Euler 定理与 Fermat 小定理

当 $\gcd(a,n)=1$ 时，Euler 定理给出

$$
a^{\varphi(n)}\equiv1\pmod n.
$$

若 $p$ 为质数且 $p\nmid a$，Fermat 小定理是它的特例：

$$
a^{p-1}\equiv1\pmod p.
$$

因此可将指数对 $\varphi(n)$ 或 $p-1$ 取模。不过若指数很小，直接计算也许更简单；若底数与模数不互质，不能无条件使用 Euler 定理。

## 模幂计算

使用快速幂，把指数写成二进制或拆成若干个二的幂：

$$
a^{13}=a^8a^4a.
$$

先依次求 $a^2,a^4,a^8$，每次平方后立即对模数取余。这样计算 $a^N\pmod n$ 的乘法次数只需 $O(\log N)$。

若能找到更小的周期 $t$，使 $a^t\equiv1\pmod n$，则指数可按 $t$ 化简。最小的此类正整数称为乘法阶，它一定整除 $\varphi(n)$（在互质条件成立时）。

## 非互质情形

当 $\gcd(a,n)\ne1$ 时，可以先分解模数：

1. 对每个质数幂模数 $p^e$ 分别计算；
2. 若 $p\mid a$ 且指数足够大，判断 $a^k$ 是否已经被 $p^e$ 整除；
3. 对互质部分使用 Euler 定理或周期；
4. 最后用中国剩余定理合并结果。

例如计算 $a^k\pmod{p^e}$ 时，若 $v_p(a)=s$，则 $v_p(a^k)=ks$。当 $ks\ge e$ 时，该部分余数为 $0$。

## 易错点

- 使用 Euler 定理前必须检查 $\gcd(a,n)=1$。
- 指数化简后，若余数为 $0$，不能直接把指数改成 $0$；应使用一个正指数周期，或单独处理指数为零的情况。
- $\varphi(n)$ 统计的是小于等于 $n$ 且与 $n$ 互质的数的个数，其中 $n$ 本身与 $n$ 不互质。
- 模数较大时，先分解成互质的质数幂通常比直接套公式更稳妥。

## 关联题目

- [[Problems/2024-B/Q14.zh-CN.md|2024-B-Q14]]
- [[Problems/2025-B/Q09.zh-CN.md|2025-B-Q09]]
- [[Problems/2022-B/Q15.zh-CN.md|2022-B-Q15]]
- [[Problems/2022-B/Q23.zh-CN.md|2022-B-Q23]]
