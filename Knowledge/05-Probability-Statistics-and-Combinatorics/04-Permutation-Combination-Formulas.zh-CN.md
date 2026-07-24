---
title: 排列与组合计算公式
tags:
  - AMC12
  - 知识点
---

# 排列与组合计算公式

## 阶乘与排列

$$
n!=1\cdot2\cdots n,\qquad 0!=1.
$$

从 $n$ 个不同对象中排列 $k$ 个：

$$
P(n,k)=n(n-1)\cdots(n-k+1)
=\frac{n!}{(n-k)!}.
$$

全排列为 $n!$。若有重复对象，除以各重复类别的阶乘：

$$
\frac{n!}{m_1!m_2!\cdots}.
$$

## 组合与恒等式

$$
\binom nk=\frac{n!}{k!(n-k)!}.
$$

常用恒等式：

$$
\binom nk=\binom n{n-k},
$$

$$
\sum_{k=0}^{n}\binom nk=2^n,
$$

$$
\sum_{k=0}^{n}k\binom nk=n2^{n-1}.
$$

最后一个等式可由对 $(1+x)^n$ 求导并令 $x=1$ 得到。

## 多项式系数

多项式展开

$$
(x_1+\cdots+x_m)^n
$$

中，$x_i$ 分别出现 $n_i$ 次且 $\sum n_i=n$ 时，系数为

$$
\binom n{n_1,n_2,\ldots,n_m}
=\frac{n!}{n_1!\cdots n_m!}.
$$

如果对象分成不可区分的小组，先确定每组人数，再使用多项式系数；若组有不同职务，职务会使对象重新区分。

## 星与条

把 $n$ 个相同物品分给 $k$ 个有标签盒子，允许空盒，方案数为

$$
\binom{n+k-1}{k-1}.
$$

若每盒至少一个，先给每盒一个，再分配剩余物品：

$$
\binom{n-1}{k-1}.
$$

若有上界，通常使用容斥或生成函数处理。

## 受限排列

对于首位限制、相邻限制或指定数字集合：

1. 先选择特殊位置；
2. 再排列剩余对象；
3. 对重复对象除以重复阶乘；
4. 检查不同分类是否重复。

若一个位置固定，剩余位置数减少；若某对象必须出现，常用总数减去不出现它的补集。

## 勒让德公式

阶乘中素数 $p$ 的指数为

$$
v_p(n!)
=\left\lfloor\frac np\right\rfloor
+\left\lfloor\frac{n}{p^2}\right\rfloor
+\left\lfloor\frac{n}{p^3}\right\rfloor+\cdots.
$$

因此

$$
v_p\left(\binom nk\right)
=v_p(n!)-v_p(k!)-v_p((n-k)!).
$$

若只问组合数末尾的零、能否被某个素数整除或素因数指数，使用素数赋值比直接计算大阶乘更快。

## 常见陷阱

- 忘记 $0!=1$。
- 计算组合时把 $k!$ 漏掉。
- 多项式计数中忽略不可区分分组或不同职务。
- 星与条没有区分允许空盒和每盒至少一个。
- 受限排列中首位为零或指定位置条件处理错误。
- 使用勒让德公式时漏掉 $p^2,p^3$ 等更高次幂。

## 关联题目

- [[Problems/2024-A/Q16.zh-CN.md|2024-A-Q16]]
- [[Problems/2024-B/Q01.zh-CN.md|2024-B-Q01]]
- [[Problems/2024-B/Q16.zh-CN.md|2024-B-Q16]]
- [[Problems/2024-B/Q17.zh-CN.md|2024-B-Q17]]
- [[Problems/2024-B/Q25.zh-CN.md|2024-B-Q25]]
- [[Problems/2025-A/Q06.zh-CN.md|2025-A-Q06]]
- [[Problems/2025-A/Q13.zh-CN.md|2025-A-Q13]]
- [[Problems/2025-A/Q18.zh-CN.md|2025-A-Q18]]
- [[Problems/2025-A/Q23.zh-CN.md|2025-A-Q23]]
- [[Problems/2025-B/Q13.zh-CN.md|2025-B-Q13]]
- [[Problems/2025-B/Q17.zh-CN.md|2025-B-Q17]]
- [[Problems/2023-A/Q07.zh-CN.md|2023-A-Q07]]
- [[Problems/2023-A/Q13.zh-CN.md|2023-A-Q13]]
- [[Problems/2023-A/Q21.zh-CN.md|2023-A-Q21]]
- [[Problems/2023-A/Q24.zh-CN.md|2023-A-Q24]]
- [[Problems/2023-B/Q05.zh-CN.md|2023-B-Q05]]
- [[Problems/2023-B/Q08.zh-CN.md|2023-B-Q08]]
- [[Problems/2023-B/Q14.zh-CN.md|2023-B-Q14]]
- [[Problems/2023-B/Q23.zh-CN.md|2023-B-Q23]]
- [[Problems/2022-A/Q07.zh-CN.md|2022-A-Q07]]
- [[Problems/2022-A/Q10.zh-CN.md|2022-A-Q10]]
- [[Problems/2022-A/Q19.zh-CN.md|2022-A-Q19]]
- [[Problems/2022-A/Q24.zh-CN.md|2022-A-Q24]]
- [[Problems/2022-B/Q06.zh-CN.md|2022-B-Q06]]
- [[Problems/2022-B/Q17.zh-CN.md|2022-B-Q17]]
- [[Problems/2021-A/Q15.zh-CN.md|2021-A-Q15]]
- [[Problems/2021-B/Q02.zh-CN.md|2021-B-Q02]]
- [[Problems/2021-B/Q19.zh-CN.md|2021-B-Q19]]
- [[Problems/2021-B/Q23.zh-CN.md|2021-B-Q23]]
- [[Problems/2020-A/Q04.zh-CN.md|2020-A-Q04]]
- [[Problems/2020-A/Q20.zh-CN.md|2020-A-Q20]]
- [[Problems/2020-B/Q15.zh-CN.md|2020-B-Q15]]
- [[Problems/2020-B/Q23.zh-CN.md|2020-B-Q23]]
