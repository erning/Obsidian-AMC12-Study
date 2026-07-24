---
title: 向量与空间几何
tags:
  - AMC12
  - 知识点
---

# 向量与空间几何

## 向量基本运算

向量可写成

$$
\mathbf v=(v_1,v_2,v_3).
$$

加法和数乘逐坐标进行。长度为

$$
|\mathbf v|=\sqrt{v_1^2+v_2^2+v_3^2}.
$$

点 $A,B$ 的位移向量为

$$
\overrightarrow{AB}=B-A.
$$

## 点积与角度

$$
\mathbf u\cdot\mathbf v
=u_1v_1+u_2v_2+u_3v_3
=|\mathbf u||\mathbf v|\cos\theta.
$$

因此

$$
\mathbf u\perp\mathbf v
\Longleftrightarrow
\mathbf u\cdot\mathbf v=0.
$$

点积也能计算投影：

$$
\operatorname{proj}_{\mathbf v}\mathbf u
=\frac{\mathbf u\cdot\mathbf v}{|\mathbf v|^2}\mathbf v.
$$

## 叉积与面积

三维叉积 $\mathbf u\times\mathbf v$ 垂直于两向量所在平面，长度为

$$
|\mathbf u\times\mathbf v|
=|\mathbf u||\mathbf v|\sin\theta.
$$

平行四边形面积为 $|\mathbf u\times\mathbf v|$，三角形面积为

$$
\frac12|\mathbf u\times\mathbf v|.
$$

若只在二维中，可以使用行列式替代叉积。

## 空间直线与平面

经过点 $P_0$、方向向量 $\mathbf v$ 的直线为

$$
\mathbf r=P_0+t\mathbf v.
$$

平面可由一点 $P_0$ 和法向量 $\mathbf n$ 表示：

$$
\mathbf n\cdot(\mathbf r-P_0)=0.
$$

若两条直线方向向量点积为 $0$，则方向垂直；若方向向量成比例，则两直线平行或重合。

## 三棱锥与混合积

三个向量 $\mathbf u,\mathbf v,\mathbf w$ 张成的平行六面体体积为

$$
|\mathbf u\cdot(\mathbf v\times\mathbf w)|.
$$

对应的三棱锥体积为

$$
\frac16|\mathbf u\cdot(\mathbf v\times\mathbf w)|.
$$

如果四个点中一个作为顶点、其余三个作为底面点，先把三个边向量从同一顶点出发，再使用混合积。

## 对称与向量和

关于某个中心对称的点满足

$$
A+B=2O.
$$

若多个点按对称方式配对，向量和常可直接计算。需要注意向量有方向；线段长度之和与向量和的长度不是一回事。

## 常见陷阱

- 将点积和叉积的几何意义混淆。
- 计算三棱锥体积时忘记除以 $6$。
- 方向向量未从同一顶点出发。
- 把向量和的长度当作各向量长度之和。
- 平面法向量与平面内方向向量混用。

## 关联题目

- [[Problems/2024-A/Q07.zh-CN.md|2024-A-Q07]]
- [[Problems/2024-A/Q24.zh-CN.md|2024-A-Q24]]
- [[Problems/2025-A/Q20.zh-CN.md|2025-A-Q20]]
- [[Problems/2025-B/Q12.zh-CN.md|2025-B-Q12]]
- [[Problems/2025-B/Q15.zh-CN.md|2025-B-Q15]]
- [[Problems/2022-B/Q14.zh-CN.md|2022-B-Q14]]
