---
title: 对称性、反射、旋转与 Burnside 引理
tags:
  - AMC12
  - 知识点
---

# 对称性、反射、旋转与 Burnside 引理

## 几何变换的基本性质

平移、旋转和反射都保持距离与角度，因此也保持图形的形状和面积。旋转的中心与角度决定变换；反射由一条对称轴决定。两个点关于直线对称时，对称轴是连接这两点的垂直平分线；点在对称轴上时保持不动。

在坐标中，常用变换包括：

$$
(x,y)\xrightarrow{\text{关于 }x\text{ 轴反射}}(x,-y),
$$

$$
(x,y)\xrightarrow{90^\circ\text{ 逆时针旋转}}(-y,x).
$$

连续变换按从右到左的顺序执行。两个反射的复合通常等价于旋转；关于相交直线反射两次，旋转角是两直线夹角的两倍。

## 对称图形与等价计数

题目若把旋转或反射后的图案视为同一个，应先确定对称群，再计算等价类。仅允许旋转时群大小为 $n$；允许旋转和反射时，正 $n$ 边形的对称群大小为 $2n$。

对于染色或标记问题，可以用 Burnside 引理：

$$
\#\text{不同图案}=\frac1{|G|}\sum_{g\in G}\#\text{被 }g\text{ 固定的图案}.
$$

固定图案的核心是分析变换产生的位置循环。一个循环中的位置必须拥有相同颜色；若有相邻不同色等条件，还要把变换后的邻接关系一起检查。

## 轨道大小与稳定子

一个图案的稳定子是保持它不变的对称变换集合。轨道大小满足

$$
|\operatorname{Orb}(x)|=\frac{|G|}{|\operatorname{Stab}(x)|}.
$$

完全不对称的图案轨道最大；具有额外旋转或反射对称的图案轨道较小。因此直接除以 $|G|$ 只适用于每个图案都没有非恒等对称的情况。

## 易错点

- 先区分“图形作为位置集合的对称性”和“染色方案被视为相同”这两个层次。
- 旋转角方向、反射轴和复合变换的顺序不能凭直觉省略。
- 计算反射固定数时，要分别考虑轴上位置和被轴成对交换的位置。
- 题目若要求颜色全部出现、相邻不同色或特定位置固定，Burnside 中每个固定数都要加入这些条件。

## 关联题目

- [[Problems/2024-A/Q07.zh-CN.md|2024-A-Q07]]
- [[Problems/2024-A/Q13.zh-CN.md|2024-A-Q13]]
- [[Problems/2024-A/Q18.zh-CN.md|2024-A-Q18]]
- [[Problems/2024-A/Q25.zh-CN.md|2024-A-Q25]]
- [[Problems/2024-B/Q19.zh-CN.md|2024-B-Q19]]
- [[Problems/2025-A/Q18.zh-CN.md|2025-A-Q18]]
- [[Problems/2025-A/Q22.zh-CN.md|2025-A-Q22]]
- [[Problems/2025-B/Q11.zh-CN.md|2025-B-Q11]]
- [[Problems/2025-B/Q17.zh-CN.md|2025-B-Q17]]
- [[Problems/2025-B/Q25.zh-CN.md|2025-B-Q25]]
- [[Problems/2023-A/Q18.zh-CN.md|2023-A-Q18]]
- [[Problems/2023-A/Q21.zh-CN.md|2023-A-Q21]]
- [[Problems/2023-B/Q09.zh-CN.md|2023-B-Q09]]
- [[Problems/2022-A/Q18.zh-CN.md|2022-A-Q18]]
- [[Problems/2022-B/Q05.zh-CN.md|2022-B-Q05]]
- [[Problems/2022-B/Q10.zh-CN.md|2022-B-Q10]]
- [[Problems/2022-B/Q18.zh-CN.md|2022-B-Q18]]
- [[Problems/2022-B/Q24.zh-CN.md|2022-B-Q24]]
- [[Problems/2021-A/Q11.zh-CN.md|2021-A-Q11]]
- [[Problems/2021-B/Q05.zh-CN.md|2021-B-Q05]]
- [[Problems/2021-B/Q08.zh-CN.md|2021-B-Q08]]
- [[Problems/2021-B/Q15.zh-CN.md|2021-B-Q15]]
- [[Problems/2021-B/Q17.zh-CN.md|2021-B-Q17]]
- [[Problems/2020-A/Q06.zh-CN.md|2020-A-Q06]]
- [[Problems/2020-A/Q11.zh-CN.md|2020-A-Q11]]
- [[Problems/2020-A/Q14.zh-CN.md|2020-A-Q14]]
- [[Problems/2020-A/Q20.zh-CN.md|2020-A-Q20]]
- [[Problems/2020-B/Q14.zh-CN.md|2020-B-Q14]]
- [[Problems/2020-B/Q15.zh-CN.md|2020-B-Q15]]
- [[Problems/2020-B/Q19.zh-CN.md|2020-B-Q19]]
- [[Problems/2020-B/Q20.zh-CN.md|2020-B-Q20]]
