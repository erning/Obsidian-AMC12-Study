---
title: 坐标几何、斜率与向量
tags:
  - AMC12
  - 知识点
---

# 坐标几何、斜率与向量

## 两点距离与中点

点 $A(x_1,y_1)$、$B(x_2,y_2)$ 的距离为

$$
AB=\sqrt{(x_2-x_1)^2+(y_2-y_1)^2}.
$$

中点为

$$
M=\left(\frac{x_1+x_2}{2},\frac{y_1+y_2}{2}\right).
$$

已知中点时可以反推

$$
B=2M-A.
$$

如果点成对关于某个中心对称，坐标和恒定，配对求和通常比逐点计算简单。

## 斜率与直线

非竖直直线斜率为

$$
m=\frac{y_2-y_1}{x_2-x_1}.
$$

点斜式为

$$
y-y_1=m(x-x_1).
$$

两条直线：

- 平行：斜率相等；
- 垂直：$m_1m_2=-1$，前提是两条斜率都有限且非零；
- 竖直线与水平线需单独处理。

点 $(x_0,y_0)$ 到直线 $Ax+By+C=0$ 的距离为

$$
\frac{|Ax_0+By_0+C|}{\sqrt{A^2+B^2}}.
$$

## 向量与点积

向量

$$
\overrightarrow{AB}=(x_B-x_A,y_B-y_A)
$$

的长度为

$$
|\mathbf v|=\sqrt{v_x^2+v_y^2}.
$$

点积为

$$
\mathbf u\cdot\mathbf v=u_xv_x+u_yv_y
=|\mathbf u||\mathbf v|\cos\theta.
$$

因此：

$$
\mathbf u\perp\mathbf v
\Longleftrightarrow
\mathbf u\cdot\mathbf v=0.
$$

二维行列式

$$
\det(\mathbf u,\mathbf v)=u_xv_y-u_yv_x
$$

的绝对值是平行四边形面积，三角形面积为其一半。

## 内分点与外分点

点 $P$ 将 $AB$ 按 $AP:PB=m:n$ 内分时，

$$
P=\frac{nA+mB}{m+n}.
$$

坐标形式为

$$
P=\left(
\frac{nx_A+mx_B}{m+n},
\frac{ny_A+my_B}{m+n}
\right).
$$

系数与对面的长度成反比；写完后应检查 $P$ 是否落在线段内部。

## 圆与轨迹

圆心 $(h,k)$、半径 $r$ 的方程为

$$
(x-h)^2+(y-k)^2=r^2.
$$

到两个定点距离相等的点在垂直平分线上；到一个定点距离固定的点在圆上；到两条相交直线距离相等的点在角平分线上。

含有绝对值的距离条件，例如

$$
|z-z_0|=r,
$$

可以看作复平面或坐标平面中的圆。对圆与直线联立时，判别式能判断相交、相切或无交点。

## 坐标变换与对称

常见对称变换：

$$
(x,y)\xrightarrow{\text{关于 }x\text{ 轴}}(x,-y),
$$

$$
(x,y)\xrightarrow{\text{关于 }y\text{ 轴}}(-x,y),
$$

$$
(x,y)\xrightarrow{\text{关于原点}}(-x,-y).
$$

绕原点旋转 $\theta$：

$$
\begin{pmatrix}x'\\y'\end{pmatrix}
=
\begin{pmatrix}
\cos\theta&-\sin\theta\\
\sin\theta&\cos\theta
\end{pmatrix}
\begin{pmatrix}x\\y\end{pmatrix}.
$$

## 常见陷阱

- 斜率公式中交换分子分母。
- 忘记竖直线没有有限斜率。
- 用斜边中线代替指向指定边的中线。
- 点积为零与行列式为零的几何意义混淆：前者表示垂直，后者表示平行或共线。
- 求线段交点后没有检查参数是否落在 $[0,1]$。
- 坐标变换时旋转方向或正负号写反。
- 用面积比代替长度比，或忘记面积对应行列式的一半。

## 关联题目

- [[Problems/2024-A/Q07.zh-CN.md|2024-A-Q07]]
- [[Problems/2024-B/Q07.zh-CN.md|2024-B-Q07]]
- [[Problems/2024-B/Q15.zh-CN.md|2024-B-Q15]]
- [[Problems/2025-A/Q11.zh-CN.md|2025-A-Q11]]
- [[Problems/2025-B/Q10.zh-CN.md|2025-B-Q10]]
- [[Problems/2025-B/Q12.zh-CN.md|2025-B-Q12]]
- [[Problems/2025-B/Q19.zh-CN.md|2025-B-Q19]]
- [[Problems/2023-A/Q06.zh-CN.md|2023-A-Q06]]
- [[Problems/2023-A/Q11.zh-CN.md|2023-A-Q11]]
- [[Problems/2023-A/Q18.zh-CN.md|2023-A-Q18]]
- [[Problems/2023-B/Q09.zh-CN.md|2023-B-Q09]]
- [[Problems/2023-B/Q10.zh-CN.md|2023-B-Q10]]
- [[Problems/2023-B/Q13.zh-CN.md|2023-B-Q13]]
- [[Problems/2022-A/Q05.zh-CN.md|2022-A-Q05]]
- [[Problems/2022-A/Q18.zh-CN.md|2022-A-Q18]]
- [[Problems/2022-A/Q20.zh-CN.md|2022-A-Q20]]
- [[Problems/2022-B/Q05.zh-CN.md|2022-B-Q05]]
- [[Problems/2022-B/Q10.zh-CN.md|2022-B-Q10]]
- [[Problems/2022-B/Q13.zh-CN.md|2022-B-Q13]]
- [[Problems/2022-B/Q14.zh-CN.md|2022-B-Q14]]
- [[Problems/2022-B/Q25.zh-CN.md|2022-B-Q25]]
- [[Problems/2021-A/Q11.zh-CN.md|2021-A-Q11]]
- [[Problems/2021-A/Q20.zh-CN.md|2021-A-Q20]]
- [[Problems/2021-B/Q05.zh-CN.md|2021-B-Q05]]
- [[Problems/2021-B/Q11.zh-CN.md|2021-B-Q11]]
- [[Problems/2021-B/Q15.zh-CN.md|2021-B-Q15]]
- [[Problems/2021-B/Q24.zh-CN.md|2021-B-Q24]]
- [[Problems/2021-B/Q25.zh-CN.md|2021-B-Q25]]
- [[Problems/2020-A/Q02.zh-CN.md|2020-A-Q02]]
- [[Problems/2020-A/Q12.zh-CN.md|2020-A-Q12]]
- [[Problems/2020-A/Q18.zh-CN.md|2020-A-Q18]]
- [[Problems/2020-A/Q24.zh-CN.md|2020-A-Q24]]
- [[Problems/2020-B/Q05.zh-CN.md|2020-B-Q05]]
- [[Problems/2020-B/Q07.zh-CN.md|2020-B-Q07]]
- [[Problems/2020-B/Q10.zh-CN.md|2020-B-Q10]]
- [[Problems/2020-B/Q11.zh-CN.md|2020-B-Q11]]
- [[Problems/2020-B/Q12.zh-CN.md|2020-B-Q12]]
- [[Problems/2020-B/Q18.zh-CN.md|2020-B-Q18]]
- [[Problems/2020-B/Q23.zh-CN.md|2020-B-Q23]]
