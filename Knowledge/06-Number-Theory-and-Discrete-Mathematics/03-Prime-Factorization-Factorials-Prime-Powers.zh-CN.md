---
title: 质因数分解、阶乘与质数幂
tags:
  - AMC12
  - 知识点
---

# 质因数分解、阶乘与质数幂

## 唯一分解与指数记账

每个大于 $1$ 的整数都能唯一写成质数幂的乘积：

$$
n=\prod_p p^{v_p(n)},
$$

其中 $v_p(n)$ 表示质数 $p$ 在 $n$ 的质因数分解中的指数。乘法、最大公因数和最小公倍数分别对应指数的加法、取小值和取大值：

$$
v_p(xy)=v_p(x)+v_p(y),\qquad v_p(\gcd(x,y))=\min(v_p(x),v_p(y)).
$$

若 $n=\prod p_i^{e_i}$，则正因数个数为

$$
\tau(n)=\prod_i(e_i+1),
$$

正因数和为

$$
\sigma(n)=\prod_i\frac{p_i^{e_i+1}-1}{p_i-1}.
$$

## 阶乘中的质数指数

Legendre 公式给出

$$
v_p(n!)=\left\lfloor\frac np\right\rfloor+\left\lfloor\frac{n}{p^2}\right\rfloor+\left\lfloor\frac{n}{p^3}\right\rfloor+\cdots.
$$

当 $p^k>n$ 时后面的项全部为 $0$。它的含义是：第一项数出 $p$ 的倍数，第二项补上这些数中额外含有的一个 $p$，依此类推。

二项式系数中的指数可由

$$
v_p\left(\binom nr\right)=v_p(n!)-v_p(r!)-v_p((n-r)!)
$$

计算。若只需判断是否被 $p$ 整除，比较指数是否至少为 $1$ 即可。

## 末尾零与最大质数幂

十进制 $n!$ 的末尾零个数是 $\min(v_2(n!),v_5(n!))$。通常 $v_5(n!)<v_2(n!)$，因此只需计算

$$
v_5(n!)=\left\lfloor\frac n5\right\rfloor+\left\lfloor\frac{n}{25}\right\rfloor+\cdots.
$$

若要找 $n!$ 中最大的 $p$ 的幂，答案是 $p^{v_p(n!)}$。对于一个乘积或商，先分别统计每个质数的指数，最后再比较或还原，通常比直接展开数字可靠。

## 完全幂与因数条件

整数 $n=\prod p_i^{e_i}$ 是完全 $k$ 次幂，当且仅当每个 $e_i$ 都是 $k$ 的倍数。若题目要求最小的正整数 $m$ 使 $mn$ 成为完全平方数，只需把 $n$ 中指数为奇数的质因子各补一次：

$$
m=\prod_{e_i\text{ 为奇数}}p_i.
$$

对于“有多少个因数”“因数乘积”“公因数个数”等问题，先完成质因数分解，再进行指数层面的组合计数。

## 易错点

- $v_p(n!)$ 不是 $\lfloor n/p\rfloor$，还要继续计算 $p^2,p^3,\ldots$ 的贡献。
- 计算组合数的质因子指数时，分子和分母的指数必须相减，不能把阶乘数值直接展开。
- “恰有 $k$ 个因数”要求解 $\prod(e_i+1)=k$，不要把指数和误当成因数个数。
- 质因数分解默认讨论正整数；若题目包含 $0$ 或负数，要单独处理其定义和符号。

## 关联题目

- [[Problems/2024-A/Q04.zh-CN.md|2024-A-Q04]]
- [[Problems/2024-B/Q02.zh-CN.md|2024-B-Q02]]
- [[Problems/2024-B/Q14.zh-CN.md|2024-B-Q14]]
- [[Problems/2024-B/Q16.zh-CN.md|2024-B-Q16]]
- [[Problems/2025-B/Q06.zh-CN.md|2025-B-Q06]]
- [[Problems/2025-B/Q23.zh-CN.md|2025-B-Q23]]
- [[Problems/2023-A/Q03.zh-CN.md|2023-A-Q03]]
- [[Problems/2023-A/Q04.zh-CN.md|2023-A-Q04]]
- [[Problems/2023-A/Q22.zh-CN.md|2023-A-Q22]]
- [[Problems/2023-B/Q23.zh-CN.md|2023-B-Q23]]
- [[Problems/2023-B/Q24.zh-CN.md|2023-B-Q24]]
- [[Problems/2022-A/Q04.zh-CN.md|2022-A-Q04]]
- [[Problems/2022-A/Q23.zh-CN.md|2022-A-Q23]]
- [[Problems/2022-B/Q03.zh-CN.md|2022-B-Q03]]
- [[Problems/2022-B/Q15.zh-CN.md|2022-B-Q15]]
- [[Problems/2022-B/Q23.zh-CN.md|2022-B-Q23]]
- [[Problems/2021-A/Q18.zh-CN.md|2021-A-Q18]]
- [[Problems/2021-A/Q25.zh-CN.md|2021-A-Q25]]
- [[Problems/2021-B/Q07.zh-CN.md|2021-B-Q07]]
- [[Problems/2020-A/Q21.zh-CN.md|2020-A-Q21]]
- [[Problems/2020-B/Q04.zh-CN.md|2020-B-Q04]]
- [[Problems/2020-B/Q06.zh-CN.md|2020-B-Q06]]
- [[Problems/2020-B/Q07.zh-CN.md|2020-B-Q07]]
- [[Problems/2020-B/Q13.zh-CN.md|2020-B-Q13]]
- [[Problems/2020-B/Q24.zh-CN.md|2020-B-Q24]]
