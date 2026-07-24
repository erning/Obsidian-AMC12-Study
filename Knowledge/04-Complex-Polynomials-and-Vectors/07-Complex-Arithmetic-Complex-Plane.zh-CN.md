---
title: 复数运算与复平面几何
tags:
  - AMC12
  - 知识点
---

# 复数运算与复平面几何

## 复平面

复数

$$
z=x+iy
$$

对应平面点 $(x,y)$。实部是横坐标，虚部是纵坐标。模长是到原点的距离：

$$
|z|=\sqrt{x^2+y^2}.
$$

复数差的模

$$
|z-w|
$$

是点 $z,w$ 之间的欧氏距离。

## 共轭与模

共轭为

$$
\bar z=x-iy,
$$

并且

$$
z\bar z=|z|^2.
$$

常用性质：

$$
\overline{z+w}=\bar z+\bar w,
\qquad
\overline{zw}=\bar z\,\bar w,
\qquad
|\bar z|=|z|.
$$

若 $z\ne0$，则

$$
\frac1z=\frac{\bar z}{|z|^2}.
$$

## 极坐标与旋转

写成

$$
z=r\operatorname{cis}\theta
=r(\cos\theta+i\sin\theta)
$$

后，乘以

$$
\operatorname{cis}\phi
$$

表示绕原点旋转 $\phi$；乘以实数 $r$ 表示缩放。

若

$$
z_2=\lambda z_1,
\qquad
\lambda=\rho\operatorname{cis}\phi,
$$

则 $z_1$ 到 $z_2$ 的长度按 $\rho$ 缩放，方向旋转 $\phi$。

## 轨迹

常见复平面轨迹：

$$
|z-z_0|=r
$$

是圆；

$$
|z-z_0|\le r
$$

是圆盘；

$$
|z-a|=|z-b|
$$

是线段 $ab$ 的垂直平分线。

若

$$
|z-a|+|z-b|=\text{常数},
$$

轨迹通常是椭圆；若为距离差的绝对值固定，则通常是双曲线。

## 面积与缩放

复数乘以复数 $\lambda$ 是相似变换，长度乘以 $|\lambda|$，面积乘以

$$
|\lambda|^2.
$$

因此由复数变换得到的新三角形或多边形面积，应按模长的平方缩放，而不是只乘 $|\lambda|$。

## 复数方程与共轭

若方程系数为实数，非实根成共轭对。若根为 $a+bi$ 和 $a-bi$，则对应实二次因子

$$
(x-a)^2+b^2.
$$

在复平面中，配对共轭点时实部相同、虚部符号相反。

## 常见陷阱

- 把虚部 $y$ 当作模长。
- 将复数乘法误解成坐标逐项相乘。
- 面积只按 $|\lambda|$ 而不是 $|\lambda|^2$ 缩放。
- 距离条件中漏掉绝对值。
- 复根没有与共轭根配对。
- 旋转方向、辐角符号或 $2\pi$ 周期处理错误。

## 关联题目

- [[Problems/2024-A/Q15.zh-CN.md|2024-A-Q15]]
- [[Problems/2024-B/Q12.zh-CN.md|2024-B-Q12]]
- [[Problems/2025-A/Q09.zh-CN.md|2025-A-Q09]]
- [[Problems/2025-A/Q17.zh-CN.md|2025-A-Q17]]
- [[Problems/2025-B/Q03.zh-CN.md|2025-B-Q03]]
- [[Problems/2025-B/Q22.zh-CN.md|2025-B-Q22]]
- [[Problems/2023-A/Q14.zh-CN.md|2023-A-Q14]]
- [[Problems/2023-A/Q16.zh-CN.md|2023-A-Q16]]
- [[Problems/2023-A/Q25.zh-CN.md|2023-A-Q25]]
- [[Problems/2023-B/Q12.zh-CN.md|2023-B-Q12]]
- [[Problems/2022-A/Q13.zh-CN.md|2022-A-Q13]]
- [[Problems/2022-A/Q21.zh-CN.md|2022-A-Q21]]
- [[Problems/2022-A/Q22.zh-CN.md|2022-A-Q22]]
- [[Problems/2022-B/Q11.zh-CN.md|2022-B-Q11]]
- [[Problems/2021-A/Q13.zh-CN.md|2021-A-Q13]]
- [[Problems/2021-A/Q21.zh-CN.md|2021-A-Q21]]
- [[Problems/2021-A/Q22.zh-CN.md|2021-A-Q22]]
- [[Problems/2021-B/Q18.zh-CN.md|2021-B-Q18]]
- [[Problems/2020-A/Q15.zh-CN.md|2020-A-Q15]]
- [[Problems/2020-A/Q22.zh-CN.md|2020-A-Q22]]
- [[Problems/2020-B/Q17.zh-CN.md|2020-B-Q17]]
- [[Problems/2020-B/Q23.zh-CN.md|2020-B-Q23]]
