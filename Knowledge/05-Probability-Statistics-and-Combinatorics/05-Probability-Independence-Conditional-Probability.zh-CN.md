---
title: 概率、独立事件与条件概率
tags:
  - AMC12
  - 知识点
---

# 概率、独立事件与条件概率

## 概率的基本规则

对有限等可能样本空间：

$$
P(A)=\frac{|A|}{|\Omega|}.
$$

一般概率满足

$$
0\le P(A)\le1,\qquad P(\Omega)=1.
$$

补集：

$$
P(A^c)=1-P(A).
$$

互斥事件满足

$$
P(A\cup B)=P(A)+P(B).
$$

一般事件需减去交集：

$$
P(A\cup B)=P(A)+P(B)-P(A\cap B).
$$

## 条件概率

若 $P(B)>0$，则

$$
P(A\mid B)=\frac{P(A\cap B)}{P(B)}.
$$

乘法公式：

$$
P(A\cap B)=P(A\mid B)P(B).
$$

这表示先发生 $B$，再在已知 $B$ 的条件下发生 $A$。抽球、抽牌和分步选择中，后续概率的分母应使用更新后的样本空间。

## 独立事件

事件 $A,B$ 独立当且仅当

$$
P(A\cap B)=P(A)P(B).
$$

等价地，在概率非零时

$$
P(A\mid B)=P(A).
$$

独立与互斥不同：若两个事件都有正概率且互斥，则它们不可能独立。

## 全概率与贝叶斯

若 $B_1,\ldots,B_k$ 构成样本空间的互斥完备划分，则

$$
P(A)=\sum_{i=1}^{k}P(A\mid B_i)P(B_i).
$$

贝叶斯公式：

$$
P(B_j\mid A)
=\frac{P(A\mid B_j)P(B_j)}
{\sum_iP(A\mid B_i)P(B_i)}.
$$

使用时先画树状图或写联合概率，避免把 $P(A\mid B)$ 和 $P(B\mid A)$ 颠倒。

## 不放回抽样

不放回抽样通常不独立，因为第一次结果会改变第二次的组成。直接按顺序计算：

$$
P(\text{路径})
=P(\text{第一步})P(\text{第二步}\mid\text{第一步})\cdots.
$$

若只关心最终选出的集合，常用组合数；若关心颜色出现顺序，则按排列或路径计数。

## 条件概率中的状态

随机游走、抽球和分配过程可按状态分类。设状态 $i$ 的成功概率为 $p_i$，则

$$
p_i=\sum_jq_{ij}p_j,
$$

边界状态直接设为 $0$ 或 $1$。状态应包含所有影响下一步概率的信息，例如各颜色剩余数量，而不能只记录已进行的步数。

## 常见陷阱

- 将互斥误认为独立。
- 把 $P(A\mid B)$ 写成 $P(B\mid A)$。
- 不放回抽样仍使用相同分母。
- “至少一次”没有使用补集。
- 树状图分支不互斥或漏掉分支。
- 状态描述不完整，导致下一步概率无法确定。

## 关联题目

- [[Problems/2024-A/Q16.zh-CN.md|2024-A-Q16]]
- [[Problems/2024-A/Q20.zh-CN.md|2024-A-Q20]]
- [[Problems/2024-B/Q17.zh-CN.md|2024-B-Q17]]
- [[Problems/2024-B/Q25.zh-CN.md|2024-B-Q25]]
- [[Problems/2025-A/Q06.zh-CN.md|2025-A-Q06]]
- [[Problems/2025-A/Q13.zh-CN.md|2025-A-Q13]]
- [[Problems/2025-B/Q11.zh-CN.md|2025-B-Q11]]
- [[Problems/2023-A/Q05.zh-CN.md|2023-A-Q05]]
- [[Problems/2023-A/Q13.zh-CN.md|2023-A-Q13]]
- [[Problems/2023-A/Q17.zh-CN.md|2023-A-Q17]]
- [[Problems/2023-B/Q08.zh-CN.md|2023-B-Q08]]
- [[Problems/2023-B/Q19.zh-CN.md|2023-B-Q19]]
- [[Problems/2022-A/Q09.zh-CN.md|2022-A-Q09]]
- [[Problems/2022-B/Q12.zh-CN.md|2022-B-Q12]]
- [[Problems/2022-B/Q22.zh-CN.md|2022-B-Q22]]
- [[Problems/2021-A/Q06.zh-CN.md|2021-A-Q06]]
- [[Problems/2021-A/Q23.zh-CN.md|2021-A-Q23]]
- [[Problems/2021-B/Q19.zh-CN.md|2021-B-Q19]]
- [[Problems/2021-B/Q23.zh-CN.md|2021-B-Q23]]
- [[Problems/2020-A/Q11.zh-CN.md|2020-A-Q11]]
- [[Problems/2020-A/Q16.zh-CN.md|2020-A-Q16]]
- [[Problems/2020-A/Q23.zh-CN.md|2020-A-Q23]]
- [[Problems/2020-B/Q16.zh-CN.md|2020-B-Q16]]
- [[Problems/2020-B/Q25.zh-CN.md|2020-B-Q25]]
